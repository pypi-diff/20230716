# Comparing `tmp/sayswho-0.1.1.tar.gz` & `tmp/sayswho-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayswho-0.1.1.tar", max compression
+gzip compressed data, was "sayswho-0.1.2.tar", max compression
```

## Comparing `sayswho-0.1.1.tar` & `sayswho-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     5550 2023-07-13 20:59:18.464577 sayswho-0.1.1/README.md
--rw-r--r--   0        0        0      505 2023-07-13 21:12:45.529345 sayswho-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 15:12:54.639435 sayswho-0.1.1/src/sayswho/__init__.py
--rw-r--r--   0        0        0     9717 2023-07-12 21:53:15.324024 sayswho-0.1.1/src/sayswho/attribution_helpers.py
--rw-r--r--   0        0        0     2540 2023-07-07 00:46:44.215252 sayswho-0.1.1/src/sayswho/constants.py
--rw-r--r--   0        0        0     5292 2023-07-12 22:02:43.820694 sayswho-0.1.1/src/sayswho/quote_helpers.py
--rw-r--r--   0        0        0     7670 2023-07-12 20:55:04.784484 sayswho-0.1.1/src/sayswho/quotes.py
--rw-r--r--   0        0        0     5884 2023-07-13 01:25:00.345184 sayswho-0.1.1/src/sayswho/sayswho.py
--rw-r--r--   0        0        0     6341 1970-01-01 00:00:00.000000 sayswho-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5267 2023-07-15 21:17:54.348528 sayswho-0.1.2/README.md
+-rw-r--r--   0        0        0      523 2023-07-15 20:40:09.241683 sayswho-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9943 2023-07-16 00:40:03.229641 sayswho-0.1.2/src/sayswho/__init__.py
+-rw-r--r--   0        0        0     2540 2023-07-15 20:14:27.794617 sayswho-0.1.2/src/sayswho/constants.py
+-rw-r--r--   0        0        0    13743 2023-07-16 00:27:39.870034 sayswho-0.1.2/src/sayswho/helpers.py
+-rw-r--r--   0        0        0     7665 2023-07-15 20:59:33.663389 sayswho-0.1.2/src/sayswho/quote_finder.py
+-rw-r--r--   0        0        0     1780 2023-07-16 00:32:31.931359 sayswho-0.1.2/src/sayswho/template.html
+-rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 sayswho-0.1.2/PKG-INFO
```

### Comparing `sayswho-0.1.1/README.md` & `sayswho-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # SaysWho
 **SaysWho** is a Python package for identifying and attributing quotes in text. It uses a combination of logic and grammer to find quotes and their speakers, then uses a [coreferencing model](https://explosion.ai/blog/coref) to better clarify who is speaking. It's built on [Textacy](https://textacy.readthedocs.io/en/latest/) and [SpaCy](https://spacy.io/).
 
-
-
 ## Notes
 - Corefencing is an experimental feature not fully integrated into SpaCy, and the current pipeline is built on SpaCy 3.4. I haven't had any problems using it with SpaCy 3.5+, but it takes some finesse to navigate the different versions.
 
+- SaysWho grew out of a larger project for analyzing newspaper articles from Lexis between ~250 and ~2000 words, and it is optimized to navitage the syntax and common errors particular to that text.
 
-- I wrote this package as part of a larger project with a better-defined goal. The output of this version is kind of open-ended, and possible not as useful as it could be. HTML viz is coming, but I'm open to any suggestions about how this could be more useful!
+- The output of this version is kind of open-ended, and possibly not as useful as it could be. HTML viz is coming, but I'm open to any suggestions about how this could be more useful!
 
 ## Installation
 Install and update using [pip](https://pip.pypa.io/en/stable/):
 
 ```
 $ pip install sayswho
 ```
 
-You will probably need to install the coreferencing model manually, then re-update SpaCy. (see [Notes](#notes))
+You will probably need to do this to navigate some versioning issues (see [Notes](#notes))
 
 ```
-$ pip install pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
+$ pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
 $ pip install spacy -U
-```
-
-You also might need to download the main large SpaCy english model.
-
-```
 $ spacy download en_core_web_lg
 ```
 
 ## A Simple Example
 
 ##### Sample text adapted from [here](https://sports.yahoo.com/nets-jacque-vaughn-looking-forward-150705556.html):
 > Nets Coach Jacque Vaughn was optimistic when discussing Ben Simmons's prospects on NBA TV.
@@ -39,33 +33,28 @@
 > "He has an innate ability to impact the basketball game on both ends of the floor. So, we missed that in the Philly series and looking forward to it.”
 > 
 > Simmons arrived in Brooklyn during the 2021-22 season, but did not play that year after a back injury. The 26-year-old would make 42 appearances (33 starts) during a tumult-filled season for Brooklyn.
 > 
 > “He is on the court. No setbacks," Vaughn later told reporters about Simmons' workouts. “We’ll continue to see him improve through the offseason.”
 
 
-#### Prep text with `prep_text_for_quote_detection()`, instantiate `Attributor` and run `.attribute` on target text.
-`prep_text_for_quote_detection()` tweaks the text to avoid some common errors and generally improve results.
+#### Instantiate `SaysWho` and run `.attribute` on target text.
 
 ```python
-from sayswho.sayswho import Attributor
-from sayswho import quote_helpers
-
-prepped_text = quote_helpers.prep_text_for_quote_detection(text)
+from sayswho import SaysWho
 
-a = Attributor()
-a.attribute(prepped_text)
+sw = SaysWho(text)
 ```
 
 
 #### See speaker, cue and content of every quote with `.quotes`.
 
 
 ```python
-print(a.quotes)
+print(sw.quotes)
 ```
 
 ```
 [DQTriple(speaker=[Vaughn], cue=[said], content=“It’s been great, being able to check in with Ben,"),
  DQTriple(speaker=[Vaughn], cue=[said], content=“I look forward to coaching a healthy Ben Simmons. The team is excited to have him healthy, being part of our program and moving forward."),
  DQTriple(speaker=[Vaughn], cue=[told], content=“He is on the court. No setbacks,"),
  DQTriple(speaker=[Vaughn], cue=[told], content=“We’ll continue to see him improve through the offseason.”)]
@@ -73,15 +62,15 @@
 
 
 
 #### See resolved entity clusters with `.clusters`.
 
 
 ```python
-print(a.clusters)
+print(sw.clusters)
 ```
 
 ```
 [[Ben Simmons's,
   Ben,
   a healthy Ben Simmons,
   him,
@@ -102,15 +91,15 @@
 
 
 
 #### Use `.print_clusters()` to see unique text in each cluster, easier to read.
 
 
 ```python
-a.print_clusters()
+sw.print_clusters()
 ```
 ```
 0 {'Ben', 'He', 'The 26-year-old', 'a healthy Ben Simmons', "Simmons'x", "Ben Simmons's", 'Simmons', 'him'}
 1 {'I', 'Nets Coach Jacque Vaughn', 'Vaughn'}
 2 {'The team', 'our', 'we', 'Nets'}
 3 {'it', 'an innate ability to impact the basketball game on both ends of the floor', 'that'}
 4 {'that year', 'the 2021-22 season'}
@@ -118,30 +107,30 @@
 ```
 
 
 #### Quote/cluster matches are saved to `.quote_matches` as `namedtuples`.
 
 
 ```python
-for qm in a.quote_matches:
+for qm in sw.quote_matches:
     print(qm)
 ```
 ```
 QuoteClusterMatch(quote_index=0, cluster_index=1)
 QuoteClusterMatch(quote_index=1, cluster_index=1)
 QuoteClusterMatch(quote_index=2, cluster_index=1)
 QuoteClusterMatch(quote_index=3, cluster_index=1)
 ```
 
 
 #### Use `.expand_match()` to view and interpret quote/cluster matches.
 
 
 ```python
-a.expand_match()
+sw.expand_match()
 ```
 ```
 QUOTE : 0
  DQTriple(speaker=[Vaughn], cue=[said], content=“It’s been great, being able to check in with Ben,") 
 
 CLUSTER : 1
  ['Nets Coach Jacque Vaughn', 'Vaughn']
```

### Comparing `sayswho-0.1.1/src/sayswho/attribution_helpers.py` & `sayswho-0.1.2/src/sayswho/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,321 +1,270 @@
-from .constants import (
-    MIN_ENTITY_DIFF,
-    MIN_SPEAKER_DIFF,
-    Boundaries,
-    QuoteClusterMatch,
-)
-from .quote_helpers import DQTriple
-from spacy.tokens import Span, SpanGroup, Token, Doc
-from typing import Union, Literal, Tuple, Iterable
-import statistics
-from rapidfuzz import fuzz
+import spacy
 import numpy as np
+import regex as re
+from .quote_finder import quote_finder
+from . import constants
+from . import helpers
+from jinja2 import Environment, FileSystemLoader
 
-
-def get_cluster_people_scores(
-    cluster: SpanGroup, scorer: Literal["prat", "cos"] = "prat"
-) -> Tuple[list, float]:
-    """
-    Calculates average similarity between any two PERSONS in the cluster.
-    These scores are used to exclude "odd man out" cluster members.
-
-    TODO: tweak cutoff value, or at least make it flexible
-
-    Input:
-        cluster (SpanGroup) - coref cluster
-        scorer (str) - what score to use to determine similarity. can be 'prat' (partial ratio) or 'cos' (cosine similarity).
-
-    Output:
-        list(tuple) - index, span, average score for each span in the cluster
-        cutoff (float) - minimum score for keeping cluster member (mean - 2stdev)
-    """
-    if scorer == "prat":
-        score_func = lambda s1, s2: fuzz.partial_ratio(s1.text, s2.text)
-    elif scorer == "cos":
-        score_func = lambda s1, s2: s1.similarity(s2)
-
-    # filter out non-persons
-    cluster_ = [span for span in cluster if person_check(span)]
-
-    all_scores = []
-    for n, span in enumerate(cluster_):
-        scores = [score_func(span, span_) for span_ in cluster_]
-        if scores:
-            all_scores.append((n, span, sum(scores) / len(scores)))
-    if len(all_scores) > 1:
-        cutoff = statistics.mean([c[-1] for c in all_scores]) - 2 * statistics.stdev(
-            [c[-1] for c in all_scores]
-        )
-        return sorted(all_scores, key=lambda k: k[-1]), cutoff
-    else:
-        return [], None
-
-
-def prune_cluster_people(cluster: SpanGroup, scorer="prat") -> list:
-    """
-    Removes outlier PERSONS from a cluster, based on provided score.
-    TODO: SpanGroup instead of list?
-
-    Input:
-        cluster (SpanGroup) - a coref cluster
-
-    Output:
-        list - coref cluster with outlier PERSONS removed
-    """
-    scores, cutoff = get_cluster_people_scores(cluster, scorer=scorer)
-    filtered = [c[1] for c in scores if c[-1] < cutoff]
-    return [c for c in cluster if c not in filtered]
-
-
-def clone_cluster(cluster: SpanGroup, destination_doc: Doc):
-    """
-    For copying a coref cluster to a different Doc.
-
-    Necessary because I'm using multiple models (of different sizes) to do coreferencing and other NLP tasks.
-    It's easier to consolidate the clusters than to combine the tasks into one model.
-    """
-    return SpanGroup(
-        doc=destination_doc,
-        spans=([destination_doc[span.start : span.end] for span in cluster]),
-    )
-
-
-def filter_duplicate_ents(ents) -> tuple:
-    """
-    Removes duplicate entities by text.
-    """
-    ent_bucket = []
-
-    for e in ents:
-        if e.text in [e.text for e in ent_bucket]:
-            continue
-        else:
-            ent_bucket.append(e)
-
-    return ent_bucket
-
-
-def get_boundaries(t: Union[Token, Span, list, DQTriple]) -> Boundaries:
-    """
-    Convenience function that returns a Boundaries tuple with the start and the end character of t.
-
-    Necessary because Token and Span have differently named attributes.
-
-    Input:
-        t (Token or Span) - spacy token or span object
-
-    Output:
-        Boundares(start, end) with start character and end character of t.
-    """
-    if isinstance(t, Token):
-        return Boundaries(t.idx, t.idx + len(t))
-
-    elif isinstance(t, Span):
-        return Boundaries(t.start_char, t.end_char)
-
-    elif isinstance(t, tuple):  # isinstance won't recognize DQTriple
-        return Boundaries(
-            get_boundaries(t.speaker[0]).start,
-            get_boundaries(t.speaker[-1]).end,
-        )
-
-    else:
-        raise TypeError("input needs to be Token, Span or DQTriple!")
-
-
-def get_text(t: Union[Token, Span, list]) -> str:
-    """
-    Convenience function, because quote speakers are lists of tokens.
-    """
-    if isinstance(t, Token) or isinstance(t, Span):
-        return t.text
-    if isinstance(t, list):
-        return " ".join([t_.text for t_ in t])
-
-
-def span_contains(
-    t1: Union[Span, Token, DQTriple], t2: Union[Span, Token, DQTriple]
-) -> bool:
+class SaysWho:
     """
-    Does t1 contain t2 or v/v? Assumes both are from the same doc, or at least same index.
-
-    Uses get_boundaries beacuse quote speakers are tokens but entities are spans.
-
-    TODO: verify same doc
+    Main class for package. Instantiation loads spacy models so they don't have to be loaded again for repeat use.
 
     Input:
-        t1 and t2 - spacy spans or tokens
-
-    Output:
-        bool - whether either t1 contains the other t2
-
+        text (str) - if provided, text will be analyzed on instantiation
+        coref_nlp (str) - name of coref model
+        base_nlp (str) - name of base model (for everything but coref) ... using en_core_web_lg because results are better than smaller models.
+        prune (bool) - if True, outlying PERSONS will be removed from coref clusters via helpers.prune_cluster_people
+        prep_text (bool) if True, text will be prepped for analysis via helpers.prep_text_for_quote_detection
     """
-    b1, b2 = tuple([get_boundaries(t) for t in [t1, t2]])
 
-    if (b1.start <= b2.start and b1.end >= b2.end) or (
-        b2.start <= b1.start and b2.end >= b1.end
+    def __init__(
+        self,
+        text: str = None,
+        coref_nlp: str = "en_coreference_web_trf",
+        base_nlp: str = "en_core_web_lg",
+        prune: bool = True,
+        prep_text: bool = True
     ):
-        return True
-
-    else:
-        return False
-
-
-def format_cluster(cluster):
-    return list(set([c.text for c in cluster if c[0].pos_ != "PRON"]))
-
-
-def pronoun_check(t: Span, doc: Doc = None):
-    """
-    Checks to see if t is a single pronoun.
-    """
-    if len(t) == 1:
-        if doc:
-            return doc[t[0].i].pos_ == "PRON"
+        self.coref_nlp = spacy.load(coref_nlp)
+        self.base_nlp = spacy.load(base_nlp)
+        self.prune = prune
+        self.prep_text = prep_text
+        if text:
+            self.attribute(text)
+
+    def expand_match(self, match=None):
+        """
+        Makes QuoteClusterMatch (or a list of QuoteClusterMatches) human-interpretable.
+
+        Input:
+            match (None, QuoteClusterMatch or list[QuoteClusterMatch]) - the QuoteClusterMatch(s) to be interpreted. Uses self.quote_matches if nothing is proivded.
+        """
+        if not match:
+            match = self.quote_matches
+            
+        if isinstance(match, list):
+            for m in match:
+                self.expand_match(m)
         else:
-            return t[0].pos_ == "PRON"
-    return False
-
-
-def person_check(span: Span):
-    """
-    Convenience function.
-    """
-    try:
-        return span.ents[0].label_ == "PERSON"
-    except IndexError:
-        return False
-
-
-def get_manual_speaker_cluster(quote, cluster):
-    """
-    If the match doesn't have a cluster, find any speakers in clusters that match manually.
-
-    The idea here is if the speaker is "Rosenberg" to pull "Detective Jeff Rosenberg" from the clusters.
-
-    TODO: Add this back into attribution code, and a test.
-    """
-    if any([len(quote.speaker) > 1, quote.speaker[0].pos_ != "PRON"]):
-        speaker = " ".join([s.text for s in quote.speaker])
-        for span in cluster:
-            if speaker in span.text:
-                return True
-    else:
-        return False
-
-
-def compare_quote_to_cluster(
-    quote: DQTriple,
-    cluster: SpanGroup,
-):
-    """
-    Finds first span in cluster that matches (according to compare_quote_to_cluster_member) with provided quote.
-
-    TODO: Doesn't consider further matches. Is this a problem?
-
-    Input:
-        quote - textacy quote object
-        cluster - coref cluster
-
-    Output:
-        cluster_index (int) - index of cluster member that matches quote (or -1, if none match)
-    """
-    try:
-        return next(
-            cluster_index
-            for cluster_index, cluster_member in enumerate(cluster)
-            if compare_quote_to_cluster_member(quote, cluster_member)
+            for m_ in ["quote", "cluster", "person"]:
+                if getattr(match, f"{m_}_index", None) is not None:
+                    i = eval(f"self.{m_}s")
+                    v = getattr(match, f"{m_}_index")
+                    data = (
+                        helpers.format_cluster(i[v])
+                        if m_ == "cluster"
+                        else i[v]
+                    )
+                    print(m_.upper(), f": {v}" "\n", data, "\n")
+        return
+
+    def attribute(self, text: str):
+        """
+        Top level function. Parses text, matches quotes to clusters and gets ent matches.
+        Input:
+            t (str) - text file to be analyzed and attributed
+
+        Output:
+            self.quote_matches (list[QuoteClusterMatch]) - list of quote/coref cluster match tuples
+        """
+        if self.prep_text:
+            text = helpers.prep_text_for_quote_detection(text)
+        self.parse_text(text)
+        self.quote_matches = self.get_matches()
+        return
+
+    def parse_text(self, text: str):
+        """
+        Imports text, gets coref clusters, copies coref clusters, finds PERSONS and gets NER matches.
+
+        Input:
+            text (string) - text to be analyzed
+
+        Ouput:
+            self.coref_doc - spacy coref-parsed doc
+            self.doc - spacy doc with coref clusters
+            self.clusters - coref clusters
+            self.quotes - list of textacy-extracted quotes
+            self.persons - list of PERSON entities
+        """
+        # instantiate spacy doc
+        self.coref_doc = self.coref_nlp(text)
+        self.doc = self.base_nlp(text)
+
+        # extract quotations
+        self.quotes = [q for q in quote_finder(self.doc)]
+
+        # extract coref clusters and clone to doc
+        self.clusters = [
+            helpers.clone_cluster(cluster, self.doc)
+            for k, cluster in self.coref_doc.spans.items()
+            if k.startswith("coref")
+        ]
+        if self.prune:
+            self.clusters = [helpers.prune_cluster_people(cluster)
+                for cluster in self.clusters
+            ]
+
+        self.persons = [e for e in self.doc.ents if e.label_ == "PERSON"]
+        return
+
+    def get_matches(self):
+        """
+        Master function to match quotes with coref clusters via matrix multiplication.
+
+        Output:
+            results (list) - list of QuoteClusterMatch tuples.
+        """
+        pairs_dicto = self.make_pairs()
+        arrays = {k: self.make_matrix(k, v) for k, v in pairs_dicto.items()}
+
+        big_matrix = np.concatenate(
+            (
+                np.transpose(
+                np.nonzero(
+                    arrays["quotes_persons"].dot(
+                        arrays["clusters_persons"].T
+                    )
+                )
+            ),
+            np.transpose(np.nonzero(arrays["quotes_clusters"])),
+            )
         )
-    except StopIteration:
-        return -1
-
-
-def compare_quote_to_cluster_member(quote: DQTriple, span: Span):
-    """
-    Compares the starting character of the quote speaker and the cluster member as well as the quote speaker sentence and the cluster member sentence to determine equivalence.
-
-    Input:
-        q (quote triple) - one textacy quote triple
-        cluster_member - one spacy-parsed entity cluster member
-
-    Output:
-        bool
-    """
-    # filters out very short strings
-    if span[0].pos_ != "PRON" and len(span) < 2 and len(span[0]) < 4:
-        return False
-    if abs(quote.speaker[0].sent.start_char - span.sent.start_char) < MIN_SPEAKER_DIFF:
-        if abs(quote.speaker[0].idx - span.start_char) < MIN_SPEAKER_DIFF:
-            return True
-    if span.start_char <= quote.speaker[0].idx:
-        if span.end_char >= (quote.speaker[-1].idx + len(quote.speaker[-1])):
-            return True
-    return False
-
-
-def compare_spans(
-    s1: Span,
-    s2: Span,
-) -> bool:
-    """
-    Compares two spans to see if their starts and ends are less than min_entity_diff.
-
-    If compare
 
-    Input:
-        s1 and s2 - spacy spans
-        min_entity_diff (int) - threshold for difference in start and ends
-    Output:
-        bool - whether the two spans start and end close enough to each other to be "equivalent"
-
-    """
-    return all(
-        [
-            abs(getattr(s1, attr) - getattr(s2, attr)) < MIN_ENTITY_DIFF
-            for attr in ["start", "end"]
+        results = sorted(list(set(
+            [constants.QuoteClusterMatch(i,j) for i,j in big_matrix]
+            )), key=lambda m: m.quote_index)
+
+        return results
+
+    def make_pairs(self) -> dict:
+        """
+        Creates quote/person, quote/cluster and cluster/person pairs for resolution and cleaning.
+
+        TODO: Ensure pronouns aren't being skipped!
+        TODO: Make ratio threshold a variable
+        """
+        pairs_dicto = {
+            p: []
+            for p in [
+                "quotes_persons",
+                "quotes_clusters",
+            ]
+        }
+
+        for quote_index, quote in enumerate(self.quotes):
+            pairs_dicto["quotes_clusters"] += [
+                (quote_index, cluster_index)
+                for cluster_index, cluster in enumerate(self.clusters)
+                for span in cluster
+                if helpers.compare_quote_to_cluster_member(quote, span)
+            ]
+
+            pairs_dicto["quotes_persons"] += [
+                (quote_index, person_index)
+                for person_index, person in enumerate(self.persons)
+                if helpers.span_contains(quote, person)
+            ]
+
+            pairs_dicto["quotes_clusters"] += [
+                (quote_index, cluster_index)
+                for cluster_index, cluster in enumerate(self.clusters)
+                if quote_index
+                not in [m[0] for m in set(pairs_dicto["quotes_clusters"])]
+                if quote.speaker[0].text in [p.text for p in self.persons]
+                if helpers.get_manual_speaker_cluster(quote, cluster)
+            ]
+
+        pairs_dicto["clusters_persons"] = [
+            (cluster_index, person_index)
+            for person_index, person in enumerate(self.persons)
+            for cluster_index, cluster in enumerate(self.clusters)
+            for span in cluster
+            if helpers.span_contains(person, span)
+            if not helpers.pronoun_check(span)
         ]
-    )
-
-
-def quick_ent_analyzer(
-    quote_person_pairs,
-    quote_cluster_pairs,
-    quote_ent_pairs,
-    cluster_ent_pairs,
-    cluster_person_pairs,
-    person_ent_pairs,
-):
-    def attributed_quote_filter(idx, ent_matches):
-        return idx in [m.quote_index for m in ent_matches]
-
-    ent_matches = []
-    quote_matches = []
-
-    for qe in quote_ent_pairs:
-        ent_matches.append(QuoteEntMatch(qe[0], None, None, qe[1]))
-
-    for qp in quote_person_pairs:
-        for pe in person_ent_pairs:
-            if qp[1] == pe[0] and not attributed_quote_filter(qp[0], ent_matches):
-                ent_matches.append(QuoteEntMatch(qp[0], None, pe[0], pe[1]))
-
-    for qc in quote_cluster_pairs:
-        if qc[1] == None and not attributed_quote_filter(qc[0], ent_matches):
-            ent_matches.append(QuoteEntMatch(qc[0]))
-        else:
-            quote_matches.append(QuoteClusterMatch(qc[0], qc[1]))
-            for ce in cluster_ent_pairs:
-                if qc[1] == ce[0] and not attributed_quote_filter(qc[0], ent_matches):
-                    ent_matches.append(QuoteEntMatch(qc[0], ce[0], None, ce[1]))
-
-            for cp in cluster_person_pairs:
-                if qc[1] == cp[0]:
-                    for pe in person_ent_pairs:
-                        if cp[1] == pe[0] and not attributed_quote_filter(
-                            qc[0], ent_matches
-                        ):
-                            ent_matches.append(
-                                QuoteEntMatch(qc[0], cp[0], pe[0], pe[1])
-                            )
+        return pairs_dicto
 
-    return sorted(list(set(ent_matches)), key=lambda m: m.quote_index)
+    def make_matrix(self, key: str, pairs: list[tuple]) -> np.array:
+        """
+        Convenience function for converting quote/cluster, quote/person and cluster/person pairs into binary matrices.
+
+        Input: 
+            key (str) - data types in pairs, connected by "_" (ie "quotes_clusters" means the pairs data is (quote, cluster))
+            pairs (list[tuple]) - (data type 1, data type 2) matches
+
+        Output:
+            m (np.array) - binary matrix of existing data type matches
+        """
+        x, y = key.split("_")
+        m = np.zeros([len(self.__getattribute__(_)) for _ in [x, y]])
+        for i, j in pairs:
+            m[i, j] = 1
+        return m
+    
+    def print_clusters(self):
+        """
+        Print clusters with duplicate text removed. For easier interpretation!
+        """
+        for n, cluster in enumerate(self.clusters):
+            print(n, set(t.text for t in cluster))
+
+    # VIZ CODE
+    def process_quote_for_rendering(self, quote_match):
+        quote = {
+            "content": self.quotes[quote_match.quote_index].content,
+            "cue": "".join([t.text_with_ws for t in self.quotes[quote_match.quote_index].cue]),
+            "cluster": ', '.join(
+                set([c.text for c in self.clusters[quote_match.cluster_index] if c[0].pos_ !="PRON"])) 
+        }
+        return quote
+    
+    def yield_quotes(self):
+        for quote_index in range(len(self.quotes)):
+            for m in (qm for qm in self.quote_matches if qm.quote_index==quote_index):
+                base_dict = self.process_quote_for_rendering(m)
+                base_dict['cluster_index'] = m.cluster_index
+                base_dict['cluster'] = ', '.join(
+                    set([c.text for c in self.clusters[m.cluster_index] if c[0].pos_ !="PRON"])
+                )
+            yield(base_dict)
+    
+    def process_text_into_html(self):
+        quote_indexes = [((q.content.start, q.content.end), "QUOTE", n) for n, q in enumerate(self.quotes)]
+        html_output = "<p>"
+        color_key = {}
+        for token in self.doc:
+            coded = False
+            if token.text == "\n":
+                token_text = "<br>"
+            else:
+                token_text = token.text_with_ws
+            for index_match in (i_ for i_ in quote_indexes if token.i in i_[0]):
+                coded = True
+                match_indexes, label, n = index_match
+                start = not match_indexes.index(token.i)
+                html_output += helpers.generate_code(n, label, start, color_key)
+                html_output += token_text
+            if not coded:
+                html_output += token_text
+
+        html_output += "</p>"
+        return html_output
+    
+    def render_to_html(self, file_name: str = "temp.html"):
+        metadata = {
+            "title": "my article",
+            "bodytext": self.process_text_into_html(),
+            "quotes": list(self.yield_quotes())
+        }
+        rendered = Environment(
+            loader=FileSystemLoader("./")
+        ).get_template('template.html').render(metadata)
+
+        with open(f"{file_name}.html", "w+") as f:
+            try:
+                f.write(rendered)
+            except UnicodeDecodeError:
+                rendered = re.sub("\u2014", "-", rendered)
+                f.write(rendered)
```

### Comparing `sayswho-0.1.1/src/sayswho/constants.py` & `sayswho-0.1.2/src/sayswho/constants.py`

 * *Files identical despite different names*

### Comparing `sayswho-0.1.1/src/sayswho/quotes.py` & `sayswho-0.1.2/src/sayswho/quote_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 This is just my version of the Textacy quote attributor. Will remove this if/when it gets implemented in Textacy!
 """
 
 from . import constants
-from spacy.tokens import Doc, Token, Span
-from spacy.symbols import VERB, PUNCT
 from operator import attrgetter
 import regex as re
 from typing import Literal, Iterable
+from spacy.tokens import Doc, Token, Span
+from spacy.symbols import VERB, PUNCT
 
-def direct_quotations(doc: Doc):
+def quote_finder(doc: Doc):
     """
     
     """
     qtoks = [tok for tok in doc if tok.is_quote or (re.match(r"\n", tok.text))]
     qtok_idx_pairs = [(-1, -1)]
     for n, q in enumerate(qtoks):
         if (
```

### Comparing `sayswho-0.1.1/PKG-INFO` & `sayswho-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 Metadata-Version: 2.1
 Name: sayswho
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quote identification, attribution and resolution.
 Home-page: https://github.com/afriedman412/sayswho
 License: MIT
 Keywords: nlp,natural-language-processing,spacy
 Author: Andy Friedman
 Author-email: afriedman412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: spacy (>=3.6.0,<4.0.0)
 Project-URL: Repository, https://github.com/afriedman412/sayswho
 Description-Content-Type: text/markdown
 
 # SaysWho
 **SaysWho** is a Python package for identifying and attributing quotes in text. It uses a combination of logic and grammer to find quotes and their speakers, then uses a [coreferencing model](https://explosion.ai/blog/coref) to better clarify who is speaking. It's built on [Textacy](https://textacy.readthedocs.io/en/latest/) and [SpaCy](https://spacy.io/).
 
-
-
 ## Notes
 - Corefencing is an experimental feature not fully integrated into SpaCy, and the current pipeline is built on SpaCy 3.4. I haven't had any problems using it with SpaCy 3.5+, but it takes some finesse to navigate the different versions.
 
+- SaysWho grew out of a larger project for analyzing newspaper articles from Lexis between ~250 and ~2000 words, and it is optimized to navitage the syntax and common errors particular to that text.
 
-- I wrote this package as part of a larger project with a better-defined goal. The output of this version is kind of open-ended, and possible not as useful as it could be. HTML viz is coming, but I'm open to any suggestions about how this could be more useful!
+- The output of this version is kind of open-ended, and possibly not as useful as it could be. HTML viz is coming, but I'm open to any suggestions about how this could be more useful!
 
 ## Installation
 Install and update using [pip](https://pip.pypa.io/en/stable/):
 
 ```
 $ pip install sayswho
 ```
 
-You will probably need to install the coreferencing model manually, then re-update SpaCy. (see [Notes](#notes))
+You will probably need to do this to navigate some versioning issues (see [Notes](#notes))
 
 ```
-$ pip install pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
+$ pip install https://github.com/explosion/spacy-experimental/releases/download/v0.6.0/en_coreference_web_trf-3.4.0a0-py3-none-any.whl
 $ pip install spacy -U
-```
-
-You also might need to download the main large SpaCy english model.
-
-```
 $ spacy download en_core_web_lg
 ```
 
 ## A Simple Example
 
 ##### Sample text adapted from [here](https://sports.yahoo.com/nets-jacque-vaughn-looking-forward-150705556.html):
 > Nets Coach Jacque Vaughn was optimistic when discussing Ben Simmons's prospects on NBA TV.
@@ -60,33 +55,28 @@
 > "He has an innate ability to impact the basketball game on both ends of the floor. So, we missed that in the Philly series and looking forward to it.”
 > 
 > Simmons arrived in Brooklyn during the 2021-22 season, but did not play that year after a back injury. The 26-year-old would make 42 appearances (33 starts) during a tumult-filled season for Brooklyn.
 > 
 > “He is on the court. No setbacks," Vaughn later told reporters about Simmons' workouts. “We’ll continue to see him improve through the offseason.”
 
 
-#### Prep text with `prep_text_for_quote_detection()`, instantiate `Attributor` and run `.attribute` on target text.
-`prep_text_for_quote_detection()` tweaks the text to avoid some common errors and generally improve results.
+#### Instantiate `SaysWho` and run `.attribute` on target text.
 
 ```python
-from sayswho.sayswho import Attributor
-from sayswho import quote_helpers
-
-prepped_text = quote_helpers.prep_text_for_quote_detection(text)
+from sayswho import SaysWho
 
-a = Attributor()
-a.attribute(prepped_text)
+sw = SaysWho(text)
 ```
 
 
 #### See speaker, cue and content of every quote with `.quotes`.
 
 
 ```python
-print(a.quotes)
+print(sw.quotes)
 ```
 
 ```
 [DQTriple(speaker=[Vaughn], cue=[said], content=“It’s been great, being able to check in with Ben,"),
  DQTriple(speaker=[Vaughn], cue=[said], content=“I look forward to coaching a healthy Ben Simmons. The team is excited to have him healthy, being part of our program and moving forward."),
  DQTriple(speaker=[Vaughn], cue=[told], content=“He is on the court. No setbacks,"),
  DQTriple(speaker=[Vaughn], cue=[told], content=“We’ll continue to see him improve through the offseason.”)]
@@ -94,15 +84,15 @@
 
 
 
 #### See resolved entity clusters with `.clusters`.
 
 
 ```python
-print(a.clusters)
+print(sw.clusters)
 ```
 
 ```
 [[Ben Simmons's,
   Ben,
   a healthy Ben Simmons,
   him,
@@ -123,15 +113,15 @@
 
 
 
 #### Use `.print_clusters()` to see unique text in each cluster, easier to read.
 
 
 ```python
-a.print_clusters()
+sw.print_clusters()
 ```
 ```
 0 {'Ben', 'He', 'The 26-year-old', 'a healthy Ben Simmons', "Simmons'x", "Ben Simmons's", 'Simmons', 'him'}
 1 {'I', 'Nets Coach Jacque Vaughn', 'Vaughn'}
 2 {'The team', 'our', 'we', 'Nets'}
 3 {'it', 'an innate ability to impact the basketball game on both ends of the floor', 'that'}
 4 {'that year', 'the 2021-22 season'}
@@ -139,30 +129,30 @@
 ```
 
 
 #### Quote/cluster matches are saved to `.quote_matches` as `namedtuples`.
 
 
 ```python
-for qm in a.quote_matches:
+for qm in sw.quote_matches:
     print(qm)
 ```
 ```
 QuoteClusterMatch(quote_index=0, cluster_index=1)
 QuoteClusterMatch(quote_index=1, cluster_index=1)
 QuoteClusterMatch(quote_index=2, cluster_index=1)
 QuoteClusterMatch(quote_index=3, cluster_index=1)
 ```
 
 
 #### Use `.expand_match()` to view and interpret quote/cluster matches.
 
 
 ```python
-a.expand_match()
+sw.expand_match()
 ```
 ```
 QUOTE : 0
  DQTriple(speaker=[Vaughn], cue=[said], content=“It’s been great, being able to check in with Ben,") 
 
 CLUSTER : 1
  ['Nets Coach Jacque Vaughn', 'Vaughn']
```


# Comparing `tmp/PyROA-3.1.0.tar.gz` & `tmp/PyROA-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyROA-3.1.0.tar", last modified: Mon Feb 27 15:03:26 2023, max compression
+gzip compressed data, was "PyROA-3.2.0.tar", last modified: Sun Jul 16 17:49:58 2023, max compression
```

## Comparing `PyROA-3.1.0.tar` & `PyROA-3.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-02-27 15:03:26.283856 PyROA-3.1.0/
--rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-02-27 15:03:26.281928 PyROA-3.1.0/PKG-INFO
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-02-27 15:03:25.720302 PyROA-3.1.0/PyROA/
--rw-rw-r--   0 donnanf    (503) staff       (20)   110281 2023-02-27 13:58:10.000000 PyROA-3.1.0/PyROA/PyROA.py
--rw-rw-r--   0 donnanf    (503) staff       (20)    40792 2023-02-27 13:58:10.000000 PyROA-3.1.0/PyROA/Utils.py
--rw-rw-r--   0 donnanf    (503) staff       (20)      204 2023-02-27 13:58:10.000000 PyROA-3.1.0/PyROA/__init__.py
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-02-27 15:03:26.279160 PyROA-3.1.0/PyROA.egg-info/
--rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-02-27 15:03:25.000000 PyROA-3.1.0/PyROA.egg-info/PKG-INFO
--rw-r--r--   0 donnanf    (503) staff       (20)      182 2023-02-27 15:03:25.000000 PyROA-3.1.0/PyROA.egg-info/SOURCES.txt
--rw-r--r--   0 donnanf    (503) staff       (20)        1 2023-02-27 15:03:25.000000 PyROA-3.1.0/PyROA.egg-info/dependency_links.txt
--rw-r--r--   0 donnanf    (503) staff       (20)        6 2023-02-27 15:03:25.000000 PyROA-3.1.0/PyROA.egg-info/top_level.txt
--rw-rw-r--   0 donnanf    (503) staff       (20)    15163 2023-02-27 13:58:10.000000 PyROA-3.1.0/README.md
--rw-r--r--   0 donnanf    (503) staff       (20)       38 2023-02-27 15:03:26.284261 PyROA-3.1.0/setup.cfg
--rw-rw-r--   0 donnanf    (503) staff       (20)      647 2023-02-27 13:58:10.000000 PyROA-3.1.0/setup.py
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-16 17:49:58.733981 PyROA-3.2.0/
+-rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-16 17:49:58.732476 PyROA-3.2.0/PKG-INFO
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-16 17:49:58.709333 PyROA-3.2.0/PyROA/
+-rw-r--r--   0 donnanf    (503) staff       (20)   111218 2023-05-26 11:57:59.000000 PyROA-3.2.0/PyROA/PyROA.py
+-rw-r--r--   0 donnanf    (503) staff       (20)    42132 2023-03-21 15:13:42.000000 PyROA-3.2.0/PyROA/Utils.py
+-rw-r--r--   0 donnanf    (503) staff       (20)      228 2023-05-26 12:03:09.000000 PyROA-3.2.0/PyROA/__init__.py
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-16 17:49:58.730747 PyROA-3.2.0/PyROA.egg-info/
+-rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/PKG-INFO
+-rw-r--r--   0 donnanf    (503) staff       (20)      182 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/SOURCES.txt
+-rw-r--r--   0 donnanf    (503) staff       (20)        1 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/dependency_links.txt
+-rw-r--r--   0 donnanf    (503) staff       (20)        6 2023-07-16 17:49:58.000000 PyROA-3.2.0/PyROA.egg-info/top_level.txt
+-rw-rw-r--   0 donnanf    (503) staff       (20)    15163 2023-02-27 13:58:10.000000 PyROA-3.2.0/README.md
+-rw-r--r--   0 donnanf    (503) staff       (20)       38 2023-07-16 17:49:58.734230 PyROA-3.2.0/setup.cfg
+-rw-rw-r--   0 donnanf    (503) staff       (20)      647 2023-05-26 12:04:29.000000 PyROA-3.2.0/setup.py
```

### Comparing `PyROA-3.1.0/PyROA/PyROA.py` & `PyROA-3.2.0/PyROA/PyROA.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,17 +458,17 @@
             w_sum = np.nansum(w)
             #Calculate optimal average
             model[j] = np.nansum(Flux_use*w)/w_sum
             #Calculate error
             errs[j] = np.sqrt(1.0/w_sum)
         
 
-       # Ps[j] = 1.0/((Flux_err[j]**2)*np.nansum(conv_use/(Flux_err_use**2)))
-        Ps[j] = 1.0/((Flux_err[j]**2)*w_sum)  
-    P = np.nansum(Ps)
+    #     Ps[j] = 1.0/((Flux_err[j]**2)*w_sum)  
+    # P = np.nansum(Ps)
+    P=1
     return mjd, model, errs, P
 
 
 
 
 
 
@@ -791,15 +791,16 @@
         else:
             P = P_func(delta)
          
     #Calculate no. of paramters for delay_dist==True here, actual ROA calcualted in loop per lightcurve   
     else:
         factors, conv, x, d = CalcWinds(merged_mjd, merged_flux, merged_err, delta, rmss, len(data), sizes,  taus, psi_types, wavelengths, T1, b, integral)
         t,m,errs, P = RunningOptimalAverageConv(merged_mjd, merged_flux, merged_err, d, factors, conv, x) 
-        
+        P=CalculateP(merged_mjd, merged_flux, merged_err, delta)
+
 
 
 
 
     #Calculate chi-squared for each lightcurve and sum
     lps=[0]*len(data)
     prev=0
@@ -926,15 +927,15 @@
         return BIC
     
     
     
     
  
 #Priors
-def log_prior(params, priors, add_var, data, delay_dist, AccDisc, wavelengths):
+def log_prior(params, priors, add_var, data, delay_dist, AccDisc, wavelengths, init_params_chunks):
     Nchunk = 2
     if (AccDisc == False):
         Nchunk+=1
     
     if (add_var == True):
         Nchunk +=1
     if (delay_dist == True and AccDisc == False):
@@ -979,40 +980,40 @@
     check=[]
     #V_priors=np.empty(len(data))
     #Loop over lightcurves
     pr=[]
     
 
     for i in range(len(data)):
-        A = params_chunks[i][0]
-        B = params_chunks[i][1]
+        A = params_chunks[i][0]/init_params_chunks[i][0] # Check A as a fraction of inital value to compare with prior
+        B = params_chunks[i][1]/init_params_chunks[i][1]
         if (AccDisc == False):
             tau = params_chunks[i][2]
         
         if (add_var == True):
-            V =  params_chunks[i][-1]
+            V =  params_chunks[i][-1]/(init_params_chunks[i][-1]*5)
             
             
         if (delay_dist == True and i>0):
             if (params_chunks[i][3]>=0.0):
                 tau_rms = params_chunks[i][3]
                 #pr.append(2.0*np.log((1.0/np.sqrt(2.0*np.pi*(rms_prior_width**2)))*np.exp(-0.5*(tau_rms/rms_prior_width)**2)))
                 check.append(0.0)
             else:
                 check.append(1.0)
 
             
         #Force peak delays to be larger than blurring reference
-        if (delay_dist == True):
-            if (tau >=params_chunks[0][2]):
-                check.append(0.0)
-            else:
-                check.append(1.0)
-        else:
-            pr.append(0.0)
+        # if (delay_dist == True):
+        #     if (tau >=params_chunks[0][2]):
+        #         check.append(0.0)
+        #     else:
+        #         check.append(1.0)
+        # else:
+        #     pr.append(0.0)
 
 
         if (AccDisc == True):
             if T1_prior[0] <= T1 <= T1_prior[1] and b_prior[0] <= b <= b_prior[1]:
                 check.append(0.0)
             else:
                 check.append(1.0)
@@ -1049,15 +1050,15 @@
         return -np.inf
 
     
 
     
     
 #Probability
-def log_probability(params, data, priors, add_var, size, sig_level, include_slow_comp, slow_comp_delta,P_func, slow_comps, P_slow, init_delta, delay_dist, psi_types, pos_ref, AccDisc, wavelengths, integral, integral2):
+def log_probability(params, data, priors, add_var, size, sig_level, include_slow_comp, slow_comp_delta,P_func, slow_comps, P_slow, init_delta, delay_dist, psi_types, pos_ref, AccDisc, wavelengths, integral, integral2, init_params_chunks):
 
 
         
         
     #Insert t1 as zero for syntax
     Nchunk = 2
     if (AccDisc == False):
@@ -1080,15 +1081,15 @@
     pos = pos_ref*Nchunk + 2
     if (AccDisc == False):
         params=np.insert(params, pos, [0.0])    #Insert zero for reference delay 
     
     
     
     
-    lp = log_prior(params, priors, add_var, data, delay_dist,  AccDisc, wavelengths)
+    lp = log_prior(params, priors, add_var, data, delay_dist,  AccDisc, wavelengths, init_params_chunks)
     if not np.isfinite(lp):
         return -np.inf
     return lp - BIC(params, data, add_var, size, sig_level, include_slow_comp, slow_comp_delta,P_func, slow_comps, P_slow, init_delta, delay_dist,psi_types, pos_ref, AccDisc, wavelengths, integral, integral2)
 
     
     
 
@@ -1135,14 +1136,15 @@
     
     #Choose intial conditions from mean and rms of data
     pos = [0]*Npar
     labels = [None]*Npar
     chunk_size = Nchunk#int((Npar - 1)/len(data))
     
     pos_chunks = [pos[i:i + chunk_size] for i in range(0, len(pos), chunk_size)]
+
     labels_chunks = [labels[i:i + chunk_size] for i in range(0, len(labels), chunk_size)]
     
 
         
     size = 0
     merged_mjd = []
     merged_flux = []
@@ -1158,26 +1160,29 @@
      
         if (include_slow_comp==True):
             t_slow, m_slow, errs_slow = RunningOptimalAverage(mjd,flux,err, slow_comp_delta)
             m_slow = m_slow - np.mean(m_slow)
             m_s = interpolate.interp1d(t_slow, m_slow, kind="linear", fill_value="extrapolate")
             pos_chunks[i][0] = np.std(flux - m_s(mjd)) #Set intial A to rms of data
             pos_chunks[i][1] = np.mean(flux- m_s(mjd)) #Set initial B to mean of data
+
+
         else:        
             pos_chunks[i][0] = pos_chunks[i][0] + np.std(flux)# - m_s(mjd)) #Set intial A to rms of data
             pos_chunks[i][1] = np.mean(flux)#- m_s(mjd)) #Set initial B to mean of data
             
+
             
 
         
 
         
 
         if(add_var == True):
-            pos_chunks[i][-1] =  0.01 #Set initial V
+            pos_chunks[i][-1] =  np.mean(err)/5.0 #0.01 #Set initial V
             labels_chunks[i][-1] = "\u03C3"+str(i)
             
             
         if (delay_dist == True and AccDisc == False):
             pos_chunks[i][3] = 1.0
             labels_chunks[i][3]="\u0394"+str(i)
        
@@ -1257,14 +1262,17 @@
         
     else:
         pos_chunks[-1][0] = init_delta#Initial delta
         labels_chunks[-1][0] = "\u0394"
         integral=None
         integral2=None
         
+    #Store initial values for use in prior
+    init_params_chunks = pos_chunks
+
     pos = list(chain.from_iterable(pos_chunks))#Flatten into single array
     labels = list(chain.from_iterable(labels_chunks))#Flatten into single array
 
     
     pos_rem = pos_ref*Nchunk + 2
     if (AccDisc == False):
 
@@ -1283,37 +1291,48 @@
 
 
     print("Initial Parameter Values")
 
     table = [pos]
     print(tabulate(table, headers=labels))        
     
-   
+
     
 
     #Define starting position
     
-    pos = 1e-4 * np.random.randn(int(2.0*Npar), int(Npar - param_delete)) + pos
+    pos = 0.2*pos* np.random.randn(int(2.0*Npar), int(Npar - param_delete)) + pos
+
     nwalkers, ndim = pos.shape
     print("NWalkers="+str(int(2.0*Npar)))
-    
+    # Make sure initial positions aren't outside priors
+    # priors_upper=[]
+    # priors_lower=[]
+    # for i in range(len(priors)):
+    #     priors_upper.append(priors[i][0])
+    #     priors_lower.append(priors[i][1])
+
+    # for i in range(nwalkers):
+    #     pos[i,:][ pos[i,:] > priors_upper] = priors_upper[pos[i,:] > priors_upper]
+    #     pos[i,:][ pos[i,:] < priors_lower] = priors_lower[pos[i,:] < priors_lower]
+
     
     #Backend
     if (use_backend == True):
         filename = "Fit.h5"
         backend = emcee.backends.HDFBackend(filename)
         if (resume_progress == True):
             print("Backend size: {0}".format(backend.iteration))
             pos = None
     else:
         backend = None
     
     with Pool() as pool:
 
-        sampler = emcee.EnsembleSampler(nwalkers, ndim, log_probability, args=[data, priors, add_var, size,sig_level, include_slow_comp, slow_comp_delta, P_func, slow_comps, P_slow, init_delta, delay_dist, psi_types, pos_ref, AccDisc, wavelengths, integral, integral2], pool=pool, backend=backend)
+        sampler = emcee.EnsembleSampler(nwalkers, ndim, log_probability, args=[data, priors, add_var, size,sig_level, include_slow_comp, slow_comp_delta, P_func, slow_comps, P_slow, init_delta, delay_dist, psi_types, pos_ref, AccDisc, wavelengths, integral, integral2, init_params_chunks], pool=pool, backend=backend)
         sampler.run_mcmc(pos, Nsamples, progress=True);
 
     #Extract samples with burn-in of 1000
     samples_flat = sampler.get_chain(discard=Nburnin, thin=15, flat=True)
 
          
     samples = sampler.get_chain()
@@ -1389,34 +1408,34 @@
         if (delay_dist == True and AccDisc == False):
             smpls = samples_chunks[i][2]
             if (psi_types[i] == "TruncGaussian"):
                 smpls = peaktomean(samples_chunks[i][2], samples_chunks[0][2], samples_chunks[i][3])
             mean_delay = np.percentile(smpls, [16, 50, 84])
             if (i != pos_ref):
                 print("Filter: " + str(filters[i]))
-                print('Mean Delay, error: %10.5f  (+%10.5f -%10.5f)'%(mean_delay[1], mean_delay[1] - mean_delay[0], mean_delay[2] - mean_delay[1]))
+                print('Mean Delay, error: %10.5f  (+%10.5f -%10.5f)'%(mean_delay[1], mean_delay[2] - mean_delay[1], mean_delay[1] - mean_delay[0]))
             else:
                 print("Filter: " + str(filters[i]))
                 print("Mean Delay, error: 0.00 (fixed)")
         elif(delay_dist == False and AccDisc == False):
             delay = np.percentile(samples_chunks[i][2], [16, 50, 84])
             if (i != pos_ref):
                 print("Filter: " + str(filters[i]))
-                print('Delay, error: %10.5f  (+%10.5f -%10.5f)'%(delay[1], delay[1] - delay[0], delay[2] - delay[1]))  
+                print('Delay, error: %10.5f  (+%10.5f -%10.5f)'%(delay[1], delay[2] - delay[1], delay[1] - delay[0]))  
             else:
                 print("Filter: " + str(filters[i]))
                 print("Delay, error: 0.00 (fixed)")
                 
         if (AccDisc == True):
             tau_0_samples =  (l_0*1e-10*1.3806e-23*samples_chunks[-1][0]/(6.63e-34*3e8))**(1.0/samples_chunks[-1][1])
             tau_samples = tau_0_samples*((l/l_0)**(1.0/samples_chunks[-1][1]))*8.0*(np.pi**4)/(15.0*integral(samples_chunks[-1][1])) - tau_0_samples*((l_delay_ref/l_0)**(1.0/samples_chunks[-1][1]))*8.0*(np.pi**4)/(15.0*integral(samples_chunks[-1][1]))
             mean_delay = np.percentile(tau_samples, [16, 50, 84])
             if (i != pos_ref):
                 print("Filter: " + str(filters[i]))
-                print('Mean Delay, error: %10.5f  (+%10.5f -%10.5f)'%(mean_delay[1], mean_delay[1] - mean_delay[0], mean_delay[2] - mean_delay[1]))
+                print('Mean Delay, error: %10.5f  (+%10.5f -%10.5f)'%(mean_delay[1], mean_delay[2] - mean_delay[1], mean_delay[1] - mean_delay[0]))
             else:
                 print("Filter: " + str(filters[i]))
                 print("Mean Delay, error: 0.00 (fixed)")
             
                 
             
         if (delay_dist == True and AccDisc == False):
@@ -1892,15 +1911,15 @@
             slow_comp = Fit.slow_comps[j]
             axs[j][0].plot(t, slow_comp(t)+B, linestyle="dashed", color="black")          
         
         length=abs(max(flux)-min(flux))
         axs[j][0].set_ylim(min(flux)-0.2*length, max(flux)+0.2*length)
         axs[j][0].set_xlabel("MJD")
         
-        axs[j][0].annotate(filters[j], xy=(0.85, 0.85), xycoords='axes fraction', size=15.0, color=band_colors[j], fontsize=20) 
+        axs[j][0].annotate(filters[j], xy=(0.85, 0.85), xycoords='axes fraction', color=band_colors[j], fontsize=20) 
         
         
       #  if (i>0 and i!=Fit.delay_ref_pos):
          #   smpls = peaktomean(samples_chunks[j][2], samples_chunks[0][2], samples_chunks[j][3])
        # else:
         smpls = tau_samples
         if (Fit.psi_types[j] == "TruncGaussian" and Fit.AccDisc == False):
@@ -2122,15 +2141,15 @@
     BIC =  lprob + Penalty
 
     return -1.0*BIC
     
     
  
 #Priors
-def log_prior2(params, priors, s):
+def log_prior2(params, priors, s, init_params_chunks):
     #Break params list into chunks of 3 i.e A, B, tau in each chunk
     params_chunks = [params[i:i + 3] for i in range(0, len(params), 3)]
     
     #Extract delta and extra variance parameters as last in params list
     delta = params_chunks[-1][0]
 
         
@@ -2144,15 +2163,15 @@
     check=[]
     A_prior = []
     B_prior=[]
     #Loop over lightcurves
     for i in range(s):
         A = params_chunks[i][0]
         B = params_chunks[i][1]
-        sig = params_chunks[i][2]
+        sig = params_chunks[i][2]/(init_params_chunks[i][2]*5.0)
         
         B_prior_width=0.5 # mJy
         lnA_prior_width=0.02 # 0.02 = 2%
         
         A_prior.append(-2.0*np.log(lnA_prior_width*A*np.sqrt(2.0*np.pi)) - (np.log(A)/lnA_prior_width)**2.0)
         B_prior.append(2.0*np.log((1.0/np.sqrt(2.0*np.pi*(B_prior_width**2)))*np.exp(-0.5*(B/B_prior_width)**2)))
         
@@ -2170,16 +2189,16 @@
         return -np.inf
 
     
 
     
     
 #Probability
-def log_probability2(params, data, priors, sig_level):
-    lp = log_prior2(params, priors, len(data))
+def log_probability2(params, data, priors, sig_level, init_params_chunks):
+    lp = log_prior2(params, priors, len(data), init_params_chunks)
     if not np.isfinite(lp):
         return -np.inf
     return lp + log_likelihood2(params, data, sig_level)
     
     
     
         
@@ -2200,38 +2219,41 @@
     for i in range(len(data)):
         mjd = data[i][:,0]
         flux = data[i][:,1]
         err = data[i][:,2]
                 
         pos_chunks[i][0] = pos_chunks[i][0] + 1.0 #Set intial A to one
         pos_chunks[i][1] = pos_chunks[i][1] + 0.0 #Set initial B to zero  
-        pos_chunks[i][2] = pos_chunks[i][1] + 0.01#2 #Set initial V to 0.02   
+        pos_chunks[i][2] = np.mean(err)/5.0#2 #Set initial V to 1/5 of mean error
         
         labels_chunks[i][0] = "A"+str(i+1)
         labels_chunks[i][1] = "B"+str(i+1)        
         labels_chunks[i][2] = "\u03C3"+str(i+1)                
         
     pos_chunks[-1][0] = init_delta#Initial delta
     labels_chunks[-1][0] = "\u0394"
+    #Store initial values for use in prior
+    init_params_chunks = pos_chunks
+
     pos = list(chain.from_iterable(pos_chunks))#Flatten into single array
     labels = list(chain.from_iterable(labels_chunks))#Flatten into single array     
     
 
     print("Initial Parameter Values")
     table = [pos]
     print(tabulate(table, headers=labels))
 
     #Define starting position
-    pos = 1e-4 * np.random.randn(int(2.0*Npar), int(Npar)) + pos
+    pos = 0.2*pos * np.random.randn(int(2.0*Npar), int(Npar)) + pos
     print("NWalkers="+str(int(2.0*Npar)))
     nwalkers, ndim = pos.shape
     with Pool() as pool:
 
         sampler = emcee.EnsembleSampler(nwalkers, ndim, log_probability2, 
-                                        args=(data, priors, sig_level), pool=pool)
+                                        args=(data, priors, sig_level, init_params_chunks), pool=pool)
         sampler.run_mcmc(pos, Nsamples, progress=True);
     
     #Extract samples with burn-in of 1000
     samples_flat = sampler.get_chain(discard=Nburnin, thin=15, flat=True)
             
     samples = sampler.get_chain()
```

### Comparing `PyROA-3.1.0/PyROA/Utils.py` & `PyROA-3.2.0/PyROA/Utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from matplotlib import gridspec#
 import scipy.interpolate as interpolate
 import corner
 import matplotlib.ticker as mtick
 import matplotlib.ticker as ticker
 import astropy.units as u
 import astropy.constants as ct
+from pandas import DataFrame
 
 def Chains(nparam,filters,delay_ref,
 				outputdir = './',
 				samples_file='samples_flat.obj',
                 initial=0,burnin=0,
                 savefig=True):
 	"""
@@ -715,15 +716,15 @@
     samples_flat = pickle.load(file)
     samples_flat = samples_flat[burnin:,:]
     file = open(outputdir+lc_file,'rb')
     models = pickle.load(file)
     
     file = open(outputdir+xt_file,'rb')
     norm_lc = pickle.load(file)
-
+    wave = np.array(wavelengths)
 
     #Split samples into chunks, 4 per lightcurve i.e A, B, tau, sig
     chunk_size=4
     transpose_samples = np.transpose(samples_flat)
     #Insert zero where tau_0 would be 
     transpose_samples = np.insert(transpose_samples, [ss*4+2], np.array([0.0]*len(transpose_samples[1])), axis=0)
     samples_chunks = [transpose_samples[i:i + chunk_size] for i in range(0, len(transpose_samples), chunk_size)] 
@@ -753,15 +754,15 @@
                 mc_pl[lo] = cnu_mcmc[jj] + xx * snu_mcmc[jj]
             
             if filters[i] == gal_ref: 
                 x_gal_mcmc = -cnu_mcmc/snu_mcmc
                 x_gal = np.median(x_gal_mcmc)
                 x_gal_error = np.std(-cnu_mcmc/snu_mcmc)
                 
-            gal_spectrum_mcmc = np.median(cnu_mcmc) +  x_gal_mcmc+x_gal_mcmc.std() * np.median(snu_mcmc)
+            gal_spectrum_mcmc = np.median(cnu_mcmc) +  (x_gal_mcmc+x_gal_mcmc.std()) * np.median(snu_mcmc)
             
             gal_spectrum.append(gal_spectrum_mcmc.mean())
             gal_spectrum_err.append(gal_spectrum_mcmc.std())
             
             fnu_f_mcmc = snu_mcmc * (np.min(norm_lc[1]) - x_gal_mcmc)
             fnu_b_mcmc = snu_mcmc * (np.max(norm_lc[1]) - x_gal_mcmc)
     
@@ -821,14 +822,23 @@
             			yerr=np.sqrt(data[:,2]**2+sig**2)*fac_flux[i+kk],
             			color=band_colors[i],
                         ls='None',alpha=0.8)
             plt.plot(xx,lin_fit*fac_flux[i+kk],color=band_colors[i],lw=3)
             max_flux = np.max([max_flux,np.max(data[:,1]*fac_flux[i+kk])])
         else:
         	kk = -1
+    fnu_f = np.array(fnu_f)
+    fnu_f_err = np.array(fnu_f_err)
+    fnu_b = np.array(fnu_b)
+    fnu_b_err = np.array(fnu_b_err)
+    slope = np.array(slope)
+    slope_err = np.array(slope_err)
+    gal_spectrum = np.array(gal_spectrum)
+    gal_spectrum_err = np.array(gal_spectrum_err)
+
     plt.axvline(x=np.median(x_gal_mcmc+x_gal_mcmc.std()),color='r',
     			linestyle='-.',label=r'Galaxy')
     plt.axvline(x=np.min(norm_lc[1]),color='k',
     			linestyle='--',label=r'F$_{\rm faint}$')
     plt.axvline(x=np.max(norm_lc[1]),color='grey',
     			linestyle='--',label=r'F$_{\rm bright}$')
 
@@ -839,17 +849,17 @@
     if limits != None: plt.ylim(-0.04,limits[1])
     
     plt.xlabel(r'$X_0 (t)$, Normalised driving light curve flux')
     plt.ylabel(ylab)
     plt.tight_layout()
 
     if savefig:
-        if figname == None: figname = 'pyroa_fluxflux.pdf'
+        if figname == None: figname = 'pyroa'
         plt.savefig(figname+'_fluxflux.pdf')
-
+	
 
     if wavelengths != None:
         wave = np.array(wavelengths)
         fig = plt.figure(figsize=(10,7))
         ax = fig.add_subplot(111)
         xxx = np.arange(2000,9300)
         #plt.plot(xxx, 0.2*(xxx/3800)**(-7/3.)*(xxx**2/2.998e18)/1e-9*1000,'-',color='#6ab04c',
@@ -874,15 +884,15 @@
         plt.errorbar(wave/(1+redshift),unred(wave,gal_spectrum,ebv)*fac_flux,
                  yerr=gal_spectrum_err*fac_flux,
                  marker='s',color='r',label='Galaxy',linestyle='-.')
 
         #print(fac_flux)
         plt.xscale('log')
         plt.yscale('log')
-        plt.xlim(np.min(wave)-100,np.max(wave)+100)
+        plt.xlim(np.min(wave/(1+redshift))-100,np.max(wave/(1+redshift))+100)
         #print(np.min(np.array(unred(wave,slope,ebv)))*0.7,max_flux*1.2)
         plt.ylim(np.min(np.array(unred(wave,slope,ebv)))*0.7*fac_flux[-1],max_flux*1.2)
         if limits != None: plt.ylim(limits[0],limits[1])
         lg = plt.legend(ncol=2)
         if redshift > 0:
             plt.xlabel(r'Rest Wavelength / $\mathrm{\AA}$')
         else:
@@ -895,14 +905,37 @@
         ax.xaxis.set_minor_locator(ticker.MultipleLocator(2000))
         plt.tight_layout()
         if savefig:
             if figname == None: figname = 'pyroa_SED.pdf'
             plt.savefig(figname+'_SED.pdf')
     else:
         print(' [PyROA] No wavelength list. Skipping SED plot.')
+        # Create output file from flux-flux analysis
+    #print(wave)
+    d = {'wave': wave, 
+    	'agn_b': np.array(fnu_b),
+    	'agn_b_err': np.array(fnu_b_err),
+    	'agn_f': np.array(fnu_f),
+    	'agn_f_err': np.array(fnu_f_err),
+    	'agn_rms': np.array(slope),
+    	'agn_rms_err':np.array(slope_err),
+    	'gal': np.array(gal_spectrum),
+    	'gal_err': np.array(gal_spectrum_err),
+    	'unred_agn_b': np.array(unred(wave,fnu_b,ebv)),
+    	'unred_agn_b_err': np.array(unred(wave,fnu_b_err,ebv)),
+    	'unred_agn_f': np.array(unred(wave,fnu_f,ebv)),
+    	'unred_agn_f_err': np.array(unred(wave,fnu_f_err,ebv)),
+    	'unred_agn_rms': np.array(unred(wave,slope,ebv)),
+    	'unred_agn_rms_err':np.array(unred(wave,slope_err,ebv)),
+    	'unred_gal': np.array(unred(wave,gal_spectrum,ebv)),
+    	'unred_gal_err': np.array(unred(wave,gal_spectrum_err,ebv))}
+    df = DataFrame(data=d)
+    if figname == None: figname = 'pyroa' 
+    df.to_csv(figname+'_fluxflux.csv',index=False)
+
 
 def Convergence(outputdir='./',samples_file='samples_flat.obj',burnin=0,
 				init_chain_length=100,savefig=True):
 
 	if outputdir[-1] != '/': outputdir += '/'
 	file = open(outputdir+samples_file,'rb')
 	samples = pickle.load(file)
```

### Comparing `PyROA-3.1.0/README.md` & `PyROA-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PyROA-3.1.0/setup.py` & `PyROA-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # upload to pip
 # pip install .
 # python3 setup.py sdist bdist_wheel
 # twine upload dist/pydoppler-0.1.8.tar.gz
 
 setuptools.setup(
      name='PyROA',
-     version='3.1.0',
+     version='3.2.0',
      packages=['PyROA'] ,
      author="Fergus Donnan,",
      author_email="fergus.donnan@physics.ox.ac.uk",
      description="PyROA is a tool for modelling quasar lightcurves",
    long_description_content_type="text/markdown",
      url="https://github.com/FergusDonnan/PyROA",
      classifiers=[
```


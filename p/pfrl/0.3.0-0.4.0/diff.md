# Comparing `tmp/pfrl-0.3.0.tar.gz` & `tmp/pfrl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pfrl-0.3.0.tar", last modified: Wed Jul  7 02:46:11 2021, max compression
+gzip compressed data, was "pfrl-0.4.0.tar", last modified: Sun Jul 16 15:21:51 2023, max compression
```

## Comparing `pfrl-0.3.0.tar` & `pfrl-0.4.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/
--rw-r--r--   0 user       (501) staff       (20)     1081 2021-07-07 02:45:53.000000 pfrl-0.3.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       34 2021-07-07 02:45:53.000000 pfrl-0.3.0/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     8546 2021-07-07 02:46:11.000000 pfrl-0.3.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     7259 2021-07-07 02:45:53.000000 pfrl-0.3.0/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/
--rw-r--r--   0 user       (501) staff       (20)      687 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    11578 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/action_value.py
--rw-r--r--   0 user       (501) staff       (20)     6094 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agent.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/agents/
--rw-r--r--   0 user       (501) staff       (20)      922 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    10245 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/a2c.py
--rw-r--r--   0 user       (501) staff       (20)    11096 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/a3c.py
--rw-r--r--   0 user       (501) staff       (20)    29550 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/acer.py
--rw-r--r--   0 user       (501) staff       (20)     2298 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/al.py
--rw-r--r--   0 user       (501) staff       (20)     1887 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/categorical_double_dqn.py
--rw-r--r--   0 user       (501) staff       (20)     7017 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/categorical_dqn.py
--rw-r--r--   0 user       (501) staff       (20)    11790 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/ddpg.py
--rw-r--r--   0 user       (501) staff       (20)     1246 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/double_dqn.py
--rw-r--r--   0 user       (501) staff       (20)     2438 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/double_pal.py
--rw-r--r--   0 user       (501) staff       (20)     3494 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/dpp.py
--rw-r--r--   0 user       (501) staff       (20)    29741 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/dqn.py
--rw-r--r--   0 user       (501) staff       (20)    14804 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/iqn.py
--rw-r--r--   0 user       (501) staff       (20)     2474 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/pal.py
--rw-r--r--   0 user       (501) staff       (20)    29790 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/ppo.py
--rw-r--r--   0 user       (501) staff       (20)     8231 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/reinforce.py
--rw-r--r--   0 user       (501) staff       (20)    14872 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/soft_actor_critic.py
--rw-r--r--   0 user       (501) staff       (20)     4547 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/state_q_function_actor.py
--rw-r--r--   0 user       (501) staff       (20)    12539 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/td3.py
--rw-r--r--   0 user       (501) staff       (20)    33013 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/agents/trpo.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/collections/
--rw-r--r--   0 user       (501) staff       (20)        0 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/collections/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    13448 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/collections/persistent_collections.py
--rw-r--r--   0 user       (501) staff       (20)     9434 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/collections/prioritized.py
--rw-r--r--   0 user       (501) staff       (20)     3109 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/collections/random_access_queue.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/distributions/
--rw-r--r--   0 user       (501) staff       (20)       51 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/distributions/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1774 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/distributions/delta.py
--rw-r--r--   0 user       (501) staff       (20)     1211 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/env.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/envs/
--rw-r--r--   0 user       (501) staff       (20)      140 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/envs/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     5584 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/envs/abc.py
--rw-r--r--   0 user       (501) staff       (20)     4415 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/envs/multiprocess_vector_env.py
--rw-r--r--   0 user       (501) staff       (20)     1314 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/envs/serial_vector_env.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/experiments/
--rw-r--r--   0 user       (501) staff       (20)      920 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3592 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/evaluation_hooks.py
--rw-r--r--   0 user       (501) staff       (20)    23450 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/evaluator.py
--rw-r--r--   0 user       (501) staff       (20)     1632 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/hooks.py
--rw-r--r--   0 user       (501) staff       (20)     5677 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/prepare_output_dir.py
--rw-r--r--   0 user       (501) staff       (20)     7382 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/train_agent.py
--rw-r--r--   0 user       (501) staff       (20)    10910 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/train_agent_async.py
--rw-r--r--   0 user       (501) staff       (20)     9144 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/experiments/train_agent_batch.py
--rw-r--r--   0 user       (501) staff       (20)      465 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/explorers/
--rw-r--r--   0 user       (501) staff       (20)      459 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1296 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorers/additive_gaussian.py
--rw-r--r--   0 user       (501) staff       (20)     1839 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorers/additive_ou.py
--rw-r--r--   0 user       (501) staff       (20)      810 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorers/boltzmann.py
--rw-r--r--   0 user       (501) staff       (20)     4349 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorers/epsilon_greedy.py
--rw-r--r--   0 user       (501) staff       (20)      245 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/explorers/greedy.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/functions/
--rw-r--r--   0 user       (501) staff       (20)        0 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/functions/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      611 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/functions/bound_by_tanh.py
--rw-r--r--   0 user       (501) staff       (20)      744 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/functions/lower_triangular_matrix.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/initializers/
--rw-r--r--   0 user       (501) staff       (20)      209 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/initializers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      622 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/initializers/chainer_default.py
--rw-r--r--   0 user       (501) staff       (20)      299 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/initializers/lecun_normal.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/nn/
--rw-r--r--   0 user       (501) staff       (20)      771 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2329 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/atari_cnn.py
--rw-r--r--   0 user       (501) staff       (20)      372 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/bound_by_tanh.py
--rw-r--r--   0 user       (501) staff       (20)      964 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/branched.py
--rw-r--r--   0 user       (501) staff       (20)      348 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/concat_obs_and_action.py
--rw-r--r--   0 user       (501) staff       (20)     3234 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/empirical_normalization.py
--rw-r--r--   0 user       (501) staff       (20)      463 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/lmbda.py
--rw-r--r--   0 user       (501) staff       (20)     1235 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/mlp.py
--rw-r--r--   0 user       (501) staff       (20)     2651 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/mlp_bn.py
--rw-r--r--   0 user       (501) staff       (20)      858 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/noisy_chain.py
--rw-r--r--   0 user       (501) staff       (20)     2532 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/noisy_linear.py
--rw-r--r--   0 user       (501) staff       (20)     1152 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/recurrent.py
--rw-r--r--   0 user       (501) staff       (20)      742 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/recurrent_branched.py
--rw-r--r--   0 user       (501) staff       (20)     2220 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/nn/recurrent_sequential.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/optimizers/
--rw-r--r--   0 user       (501) staff       (20)      168 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/optimizers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3064 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/optimizers/rmsprop_eps_inside_sqrt.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/policies/
--rw-r--r--   0 user       (501) staff       (20)      160 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/policies/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      255 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/policies/deterministic_policy.py
--rw-r--r--   0 user       (501) staff       (20)     4099 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/policies/gaussian_policy.py
--rw-r--r--   0 user       (501) staff       (20)      170 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/policies/softmax_policy.py
--rw-r--r--   0 user       (501) staff       (20)      354 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/policy.py
--rw-r--r--   0 user       (501) staff       (20)      864 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/q_function.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/q_functions/
--rw-r--r--   0 user       (501) staff       (20)      172 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/q_functions/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3797 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/q_functions/dueling_dqn.py
--rw-r--r--   0 user       (501) staff       (20)    10249 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/q_functions/state_action_q_functions.py
--rw-r--r--   0 user       (501) staff       (20)     7267 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/q_functions/state_q_functions.py
--rw-r--r--   0 user       (501) staff       (20)    12026 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/replay_buffers/
--rw-r--r--   0 user       (501) staff       (20)      543 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3285 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffers/episodic.py
--rw-r--r--   0 user       (501) staff       (20)     6176 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffers/persistent.py
--rw-r--r--   0 user       (501) staff       (20)     4437 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffers/prioritized.py
--rw-r--r--   0 user       (501) staff       (20)     2981 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffers/prioritized_episodic.py
--rw-r--r--   0 user       (501) staff       (20)     3168 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/replay_buffers/replay_buffer.py
--rw-r--r--   0 user       (501) staff       (20)      756 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/testing.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/utils/
--rw-r--r--   0 user       (501) staff       (20)      548 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      230 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/ask_yes_no.py
--rw-r--r--   0 user       (501) staff       (20)     1119 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/async_.py
--rw-r--r--   0 user       (501) staff       (20)     1234 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/batch_states.py
--rw-r--r--   0 user       (501) staff       (20)     1249 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/clip_l2_grad_norm.py
--rw-r--r--   0 user       (501) staff       (20)     1077 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/conjugate_gradient.py
--rw-r--r--   0 user       (501) staff       (20)      256 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/contexts.py
--rw-r--r--   0 user       (501) staff       (20)     1429 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/copy_param.py
--rw-r--r--   0 user       (501) staff       (20)     1803 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/env_modifiers.py
--rw-r--r--   0 user       (501) staff       (20)      550 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/is_return_code_zero.py
--rw-r--r--   0 user       (501) staff       (20)      756 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/mode_of_distribution.py
--rw-r--r--   0 user       (501) staff       (20)     5940 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/pretrained_models.py
--rw-r--r--   0 user       (501) staff       (20)      843 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/random.py
--rw-r--r--   0 user       (501) staff       (20)      557 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/random_seed.py
--rw-r--r--   0 user       (501) staff       (20)    11744 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/recurrent.py
--rw-r--r--   0 user       (501) staff       (20)      950 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/reward_filter.py
--rw-r--r--   0 user       (501) staff       (20)      540 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/utils/stoppable_thread.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl/wrappers/
--rw-r--r--   0 user       (501) staff       (20)      591 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    10480 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/atari_wrappers.py
--rw-r--r--   0 user       (501) staff       (20)      827 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/cast_observation.py
--rw-r--r--   0 user       (501) staff       (20)     1340 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/continuing_time_limit.py
--rw-r--r--   0 user       (501) staff       (20)     2963 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/monitor.py
--rw-r--r--   0 user       (501) staff       (20)      769 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/normalize_action_space.py
--rw-r--r--   0 user       (501) staff       (20)     1363 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/randomize_action.py
--rw-r--r--   0 user       (501) staff       (20)      562 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/render.py
--rw-r--r--   0 user       (501) staff       (20)      500 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/scale_reward.py
--rw-r--r--   0 user       (501) staff       (20)     3404 2021-07-07 02:45:53.000000 pfrl-0.3.0/pfrl/wrappers/vector_frame_stack.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2021-07-07 02:46:11.000000 pfrl-0.3.0/pfrl.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     8546 2021-07-07 02:46:10.000000 pfrl-0.3.0/pfrl.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3451 2021-07-07 02:46:10.000000 pfrl-0.3.0/pfrl.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2021-07-07 02:46:10.000000 pfrl-0.3.0/pfrl.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       54 2021-07-07 02:46:10.000000 pfrl-0.3.0/pfrl.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        5 2021-07-07 02:46:10.000000 pfrl-0.3.0/pfrl.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)      830 2021-07-07 02:46:11.000000 pfrl-0.3.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      800 2021-07-07 02:45:53.000000 pfrl-0.3.0/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.363031 pfrl-0.4.0/
+-rw-r--r--   0 user       (501) staff       (20)     1081 2023-07-16 15:20:41.000000 pfrl-0.4.0/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       34 2023-07-16 15:20:41.000000 pfrl-0.4.0/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     7502 2023-07-16 15:21:51.363119 pfrl-0.4.0/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     7259 2023-07-16 15:20:41.000000 pfrl-0.4.0/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.340754 pfrl-0.4.0/pfrl/
+-rw-r--r--   0 user       (501) staff       (20)      687 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    11578 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/action_value.py
+-rw-r--r--   0 user       (501) staff       (20)     6094 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agent.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.345861 pfrl-0.4.0/pfrl/agents/
+-rw-r--r--   0 user       (501) staff       (20)      922 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    10244 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/a2c.py
+-rw-r--r--   0 user       (501) staff       (20)    11094 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/a3c.py
+-rw-r--r--   0 user       (501) staff       (20)    29543 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/acer.py
+-rw-r--r--   0 user       (501) staff       (20)     2297 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/al.py
+-rw-r--r--   0 user       (501) staff       (20)     1887 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/categorical_double_dqn.py
+-rw-r--r--   0 user       (501) staff       (20)     7017 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/categorical_dqn.py
+-rw-r--r--   0 user       (501) staff       (20)    11787 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/ddpg.py
+-rw-r--r--   0 user       (501) staff       (20)     1245 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/double_dqn.py
+-rw-r--r--   0 user       (501) staff       (20)     2437 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/double_pal.py
+-rw-r--r--   0 user       (501) staff       (20)     3492 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/dpp.py
+-rw-r--r--   0 user       (501) staff       (20)    30577 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/dqn.py
+-rw-r--r--   0 user       (501) staff       (20)    14804 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/iqn.py
+-rw-r--r--   0 user       (501) staff       (20)     2473 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/pal.py
+-rw-r--r--   0 user       (501) staff       (20)    29788 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/ppo.py
+-rw-r--r--   0 user       (501) staff       (20)     8229 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/reinforce.py
+-rw-r--r--   0 user       (501) staff       (20)    14871 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/soft_actor_critic.py
+-rw-r--r--   0 user       (501) staff       (20)     4547 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/state_q_function_actor.py
+-rw-r--r--   0 user       (501) staff       (20)    12538 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/td3.py
+-rw-r--r--   0 user       (501) staff       (20)    33010 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/agents/trpo.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.346648 pfrl-0.4.0/pfrl/collections/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/collections/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    13448 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/collections/persistent_collections.py
+-rw-r--r--   0 user       (501) staff       (20)     9406 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/collections/prioritized.py
+-rw-r--r--   0 user       (501) staff       (20)     3109 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/collections/random_access_queue.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.347097 pfrl-0.4.0/pfrl/distributions/
+-rw-r--r--   0 user       (501) staff       (20)       51 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/distributions/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1774 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/distributions/delta.py
+-rw-r--r--   0 user       (501) staff       (20)     1211 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/env.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.347876 pfrl-0.4.0/pfrl/envs/
+-rw-r--r--   0 user       (501) staff       (20)      140 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/envs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     5584 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/envs/abc.py
+-rw-r--r--   0 user       (501) staff       (20)     4415 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/envs/multiprocess_vector_env.py
+-rw-r--r--   0 user       (501) staff       (20)     1314 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/envs/serial_vector_env.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.349619 pfrl-0.4.0/pfrl/experiments/
+-rw-r--r--   0 user       (501) staff       (20)      920 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3592 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/evaluation_hooks.py
+-rw-r--r--   0 user       (501) staff       (20)    23450 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/evaluator.py
+-rw-r--r--   0 user       (501) staff       (20)     1632 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/hooks.py
+-rw-r--r--   0 user       (501) staff       (20)     5677 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/prepare_output_dir.py
+-rw-r--r--   0 user       (501) staff       (20)     7380 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/train_agent.py
+-rw-r--r--   0 user       (501) staff       (20)    10903 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/train_agent_async.py
+-rw-r--r--   0 user       (501) staff       (20)     9144 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/experiments/train_agent_batch.py
+-rw-r--r--   0 user       (501) staff       (20)      465 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.350672 pfrl-0.4.0/pfrl/explorers/
+-rw-r--r--   0 user       (501) staff       (20)      459 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1296 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorers/additive_gaussian.py
+-rw-r--r--   0 user       (501) staff       (20)     1837 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorers/additive_ou.py
+-rw-r--r--   0 user       (501) staff       (20)      810 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorers/boltzmann.py
+-rw-r--r--   0 user       (501) staff       (20)     4347 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorers/epsilon_greedy.py
+-rw-r--r--   0 user       (501) staff       (20)      245 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/explorers/greedy.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.351172 pfrl-0.4.0/pfrl/functions/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/functions/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      611 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/functions/bound_by_tanh.py
+-rw-r--r--   0 user       (501) staff       (20)      744 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/functions/lower_triangular_matrix.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.351805 pfrl-0.4.0/pfrl/initializers/
+-rw-r--r--   0 user       (501) staff       (20)      209 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/initializers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      622 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/initializers/chainer_default.py
+-rw-r--r--   0 user       (501) staff       (20)      299 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/initializers/lecun_normal.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.354754 pfrl-0.4.0/pfrl/nn/
+-rw-r--r--   0 user       (501) staff       (20)      771 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2329 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/atari_cnn.py
+-rw-r--r--   0 user       (501) staff       (20)      372 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/bound_by_tanh.py
+-rw-r--r--   0 user       (501) staff       (20)      964 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/branched.py
+-rw-r--r--   0 user       (501) staff       (20)      348 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/concat_obs_and_action.py
+-rw-r--r--   0 user       (501) staff       (20)     3234 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/empirical_normalization.py
+-rw-r--r--   0 user       (501) staff       (20)      463 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/lmbda.py
+-rw-r--r--   0 user       (501) staff       (20)     1235 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/mlp.py
+-rw-r--r--   0 user       (501) staff       (20)     2651 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/mlp_bn.py
+-rw-r--r--   0 user       (501) staff       (20)      858 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/noisy_chain.py
+-rw-r--r--   0 user       (501) staff       (20)     2531 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/noisy_linear.py
+-rw-r--r--   0 user       (501) staff       (20)     1152 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/recurrent.py
+-rw-r--r--   0 user       (501) staff       (20)      742 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/recurrent_branched.py
+-rw-r--r--   0 user       (501) staff       (20)     2220 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/nn/recurrent_sequential.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.355114 pfrl-0.4.0/pfrl/optimizers/
+-rw-r--r--   0 user       (501) staff       (20)      168 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/optimizers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3064 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/optimizers/rmsprop_eps_inside_sqrt.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.355913 pfrl-0.4.0/pfrl/policies/
+-rw-r--r--   0 user       (501) staff       (20)      160 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/policies/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      255 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/policies/deterministic_policy.py
+-rw-r--r--   0 user       (501) staff       (20)     4099 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/policies/gaussian_policy.py
+-rw-r--r--   0 user       (501) staff       (20)      170 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/policies/softmax_policy.py
+-rw-r--r--   0 user       (501) staff       (20)      354 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/policy.py
+-rw-r--r--   0 user       (501) staff       (20)      864 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/q_function.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.356681 pfrl-0.4.0/pfrl/q_functions/
+-rw-r--r--   0 user       (501) staff       (20)      172 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/q_functions/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3797 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/q_functions/dueling_dqn.py
+-rw-r--r--   0 user       (501) staff       (20)    10247 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/q_functions/state_action_q_functions.py
+-rw-r--r--   0 user       (501) staff       (20)     7265 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/q_functions/state_q_functions.py
+-rw-r--r--   0 user       (501) staff       (20)    12023 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.357992 pfrl-0.4.0/pfrl/replay_buffers/
+-rw-r--r--   0 user       (501) staff       (20)      543 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3284 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffers/episodic.py
+-rw-r--r--   0 user       (501) staff       (20)     6176 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffers/persistent.py
+-rw-r--r--   0 user       (501) staff       (20)     4437 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffers/prioritized.py
+-rw-r--r--   0 user       (501) staff       (20)     2981 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffers/prioritized_episodic.py
+-rw-r--r--   0 user       (501) staff       (20)     3168 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/replay_buffers/replay_buffer.py
+-rw-r--r--   0 user       (501) staff       (20)      756 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/testing.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.361119 pfrl-0.4.0/pfrl/utils/
+-rw-r--r--   0 user       (501) staff       (20)      548 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      230 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/ask_yes_no.py
+-rw-r--r--   0 user       (501) staff       (20)     1119 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/async_.py
+-rw-r--r--   0 user       (501) staff       (20)     1234 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/batch_states.py
+-rw-r--r--   0 user       (501) staff       (20)     1249 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/clip_l2_grad_norm.py
+-rw-r--r--   0 user       (501) staff       (20)     1077 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/conjugate_gradient.py
+-rw-r--r--   0 user       (501) staff       (20)      256 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/contexts.py
+-rw-r--r--   0 user       (501) staff       (20)     1429 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/copy_param.py
+-rw-r--r--   0 user       (501) staff       (20)     1803 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/env_modifiers.py
+-rw-r--r--   0 user       (501) staff       (20)      550 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/is_return_code_zero.py
+-rw-r--r--   0 user       (501) staff       (20)      756 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/mode_of_distribution.py
+-rw-r--r--   0 user       (501) staff       (20)     5940 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/pretrained_models.py
+-rw-r--r--   0 user       (501) staff       (20)      843 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/random.py
+-rw-r--r--   0 user       (501) staff       (20)      557 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/random_seed.py
+-rw-r--r--   0 user       (501) staff       (20)    12002 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/recurrent.py
+-rw-r--r--   0 user       (501) staff       (20)      946 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/reward_filter.py
+-rw-r--r--   0 user       (501) staff       (20)      540 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/utils/stoppable_thread.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.362820 pfrl-0.4.0/pfrl/wrappers/
+-rw-r--r--   0 user       (501) staff       (20)      591 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    10631 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/atari_wrappers.py
+-rw-r--r--   0 user       (501) staff       (20)      827 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/cast_observation.py
+-rw-r--r--   0 user       (501) staff       (20)     1340 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/continuing_time_limit.py
+-rw-r--r--   0 user       (501) staff       (20)     3303 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/monitor.py
+-rw-r--r--   0 user       (501) staff       (20)      769 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/normalize_action_space.py
+-rw-r--r--   0 user       (501) staff       (20)     1363 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/randomize_action.py
+-rw-r--r--   0 user       (501) staff       (20)      562 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/render.py
+-rw-r--r--   0 user       (501) staff       (20)      500 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/scale_reward.py
+-rw-r--r--   0 user       (501) staff       (20)     3404 2023-07-16 15:20:41.000000 pfrl-0.4.0/pfrl/wrappers/vector_frame_stack.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-16 15:21:51.341751 pfrl-0.4.0/pfrl.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     7502 2023-07-16 15:21:51.000000 pfrl-0.4.0/pfrl.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3451 2023-07-16 15:21:51.000000 pfrl-0.4.0/pfrl.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-16 15:21:51.000000 pfrl-0.4.0/pfrl.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       54 2023-07-16 15:21:51.000000 pfrl-0.4.0/pfrl.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        5 2023-07-16 15:21:51.000000 pfrl-0.4.0/pfrl.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)      830 2023-07-16 15:21:51.363498 pfrl-0.4.0/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      800 2023-07-16 15:20:41.000000 pfrl-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pfrl-0.3.0/LICENSE` & `pfrl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/PKG-INFO` & `pfrl-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,137 @@
 Metadata-Version: 2.1
 Name: pfrl
-Version: 0.3.0
+Version: 0.4.0
 Summary: PFRL, a deep reinforcement learning library
-Home-page: UNKNOWN
 Author: Yasuhiro Fujita
 Author-email: fujita@preferred.jp
 License: MIT License
-Description: <div align="center"><img src="https://raw.githubusercontent.com/pfnet/pfrl/master/assets/PFRL.png" height=150/></div>
-        
-        # PFRL
-        [![Documentation Status](https://readthedocs.org/projects/pfrl/badge/?version=latest)](http://pfrl.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/pfrl.svg)](https://pypi.python.org/pypi/pfrl)
-        
-        PFRL is a deep reinforcement learning library that implements various state-of-the-art deep reinforcement algorithms in Python using [PyTorch](https://github.com/pytorch/pytorch).
-        
-        ![Boxing](assets/boxing.gif)
-        ![Humanoid](assets/humanoid.gif)
-        ![Grasping](assets/grasping.gif)
-        ![Atlas](examples/atlas/assets/atlas.gif)
-        ![SlimeVolley](examples/slimevolley/assets/slimevolley.gif)
-        
-        ## Installation
-        
-        PFRL is tested with Python 3.7.7. For other requirements, see [requirements.txt](requirements.txt).
-        
-        PFRL can be installed via PyPI:
-        ```
-        pip install pfrl
-        ```
-        
-        It can also be installed from the source code:
-        ```
-        python setup.py install
-        ```
-        
-        Refer to [Installation](http://pfrl.readthedocs.io/en/latest/install.html) for more information on installation. 
-        
-        ## Getting started
-        
-        You can try [PFRL Quickstart Guide](examples/quickstart/quickstart.ipynb) first, or check the [examples](examples) ready for Atari 2600 and Open AI Gym.
-        
-        For more information, you can refer to [PFRL's documentation](http://pfrl.readthedocs.io/en/latest/index.html).
-        
-        ### Blog Posts
-        - [Introducing PFRL: A PyTorch-based Deep RL Library](https://t.co/VaT06nejSC?amp=1)
-        - [PFRL’s Pretrained Model Zoo](https://bit.ly/3fNx5xH)
-        
-        ## Algorithms
-        
-        | Algorithm | Discrete Action | Continous Action | Recurrent Model | Batch Training | CPU Async Training | Pretrained models<sup>*</sup> |
-        |:----------|:---------------:|:----------------:|:---------------:|:--------------:|:------------------:|:------------------:|
-        | DQN (including DoubleDQN etc.) | ✓ | ✓ (NAF) | ✓ | ✓ | x | ✓ |
-        | Categorical DQN | ✓ | x | ✓ | ✓ | x | x |
-        | Rainbow | ✓ | x | ✓ | ✓ | x | ✓ |
-        | IQN | ✓ | x | ✓ | ✓ | x | ✓ |
-        | DDPG | x | ✓ | x | ✓ | x | ✓ |
-        | A3C  | ✓ | ✓ | ✓ | ✓ (A2C) | ✓ | ✓ |
-        | ACER | ✓ | ✓ | ✓ | x | ✓ | x |
-        | PPO  | ✓ | ✓ | ✓ | ✓ | x | ✓ |
-        | TRPO | ✓ | ✓ | ✓ | ✓ | x | ✓ |
-        | TD3 | x | ✓ | x | ✓ | x | ✓ |
-        | SAC | x | ✓ | x | ✓ | x | ✓ |
-        
-        **<sup>*</sup>Note on Pretrained models**: PFRL provides pretrained models (sometimes called a 'model zoo') for our reproducibility scripts on [Atari environments](https://github.com/pfnet/pfrl/tree/master/examples/atari/reproduction) (DQN, IQN, Rainbow, and A3C) and [Mujoco environments](https://github.com/pfnet/pfrl/tree/master/examples/mujoco/reproduction) (DDPG, TRPO, PPO, TD3, SAC), for each benchmarked environment. 
-        
-        Following algorithms have been implemented in PFRL:
-        - [A2C (Synchronous variant of A3C)](https://openai.com/blog/baselines-acktr-a2c/)
-          - examples: [[atari (batched)]](examples/atari/train_a2c_ale.py)
-        - [A3C (Asynchronous Advantage Actor-Critic)](https://arxiv.org/abs/1602.01783)
-          - examples: [[atari reproduction]](examples/atari/reproduction/a3c) [[atari]](examples/atari/train_a3c_ale.py)
-        - [ACER (Actor-Critic with Experience Replay)](https://arxiv.org/abs/1611.01224)
-          - examples: [[atari]](examples/atari/train_acer_ale.py)
-        - [Categorical DQN](https://arxiv.org/abs/1707.06887)
-          - examples: [[atari]](examples/atari/train_categorical_dqn_ale.py) [[general gym]](examples/gym/train_categorical_dqn_gym.py)
-        - [DQN (Deep Q-Network)](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf) (including [Double DQN](https://arxiv.org/abs/1509.06461), [Persistent Advantage Learning (PAL)](https://arxiv.org/abs/1512.04860), Double PAL, [Dynamic Policy Programming (DPP)](http://www.jmlr.org/papers/volume13/azar12a/azar12a.pdf))
-          - examples: [[atari reproduction]](examples/atari/reproduction/dqn) [[atari]](examples/atari/train_dqn_ale.py) [[atari (batched)]](examples/atari/train_dqn_batch_ale.py) [[flickering atari]](examples/atari/train_drqn_ale.py) [[general gym]](examples/gym/train_dqn_gym.py)
-        - [DDPG (Deep Deterministic Policy Gradients)](https://arxiv.org/abs/1509.02971) (including [SVG(0)](https://arxiv.org/abs/1510.09142))
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ddpg)
-        - [IQN (Implicit Quantile Networks)](https://arxiv.org/abs/1806.06923)
-          - examples: [[atari reproduction]](examples/atari/reproduction/iqn)
-        - [PPO (Proximal Policy Optimization)](https://arxiv.org/abs/1707.06347)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ppo) [[atari]](examples/atari/train_ppo_ale.py)
-        - [Rainbow](https://arxiv.org/abs/1710.02298)
-          - examples: [[atari reproduction]](examples/atari/reproduction/rainbow) [[Slime volleyball]](examples/slimevolley/)
-        - [REINFORCE](http://www-anw.cs.umass.edu/~barto/courses/cs687/williams92simple.pdf)
-          - examples: [[general gym]](examples/gym/train_reinforce_gym.py)
-        - [SAC (Soft Actor-Critic)](https://arxiv.org/abs/1812.05905)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/soft_actor_critic) [[Atlas walk]](examples/atlas/)
-        - [TRPO (Trust Region Policy Optimization)](https://arxiv.org/abs/1502.05477) with [GAE (Generalized Advantage Estimation)](https://arxiv.org/abs/1506.02438)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/trpo)
-        - [TD3 (Twin Delayed Deep Deterministic policy gradient algorithm)](https://arxiv.org/abs/1802.09477)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/td3)
-        
-        Following useful techniques have been also implemented in PFRL:
-        - [NoisyNet](https://arxiv.org/abs/1706.10295)
-          - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
-        - [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952)
-          - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
-        - [Dueling Network](https://arxiv.org/abs/1511.06581)
-          - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
-        - [Normalized Advantage Function](https://arxiv.org/abs/1603.00748)
-          - examples: [[DQN]](examples/gym/train_dqn_gym.py) (for continuous-action envs only)
-        - [Deep Recurrent Q-Network](https://arxiv.org/abs/1507.06527)
-          - examples: [[DQN]](examples/atari/train_drqn_ale.py)
-        
-        
-        ## Environments
-        
-        Environments that support the subset of OpenAI Gym's interface (`reset` and `step` methods) can be used.
-        
-        ## Contributing
-        
-        Any kind of contribution to PFRL would be highly appreciated! If you are interested in contributing to PFRL, please read [CONTRIBUTING.md](CONTRIBUTING.md).
-        
-        ## License
-        
-        [MIT License](LICENSE).
-        
-        ## Citations
-        
-        To cite PFRL in publications, please cite our [paper](https://www.jmlr.org/papers/v22/20-376.html) on ChainerRL, the library on which PFRL is based:
-        
-        ```
-        @article{JMLR:v22:20-376,
-          author  = {Yasuhiro Fujita and Prabhat Nagarajan and Toshiki Kataoka and Takahiro Ishikawa},
-          title   = {ChainerRL: A Deep Reinforcement Learning Library},
-          journal = {Journal of Machine Learning Research},
-          year    = {2021},
-          volume  = {22},
-          number  = {77},
-          pages   = {1-14},
-          url     = {http://jmlr.org/papers/v22/20-376.html}
-        }
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center"><img src="https://raw.githubusercontent.com/pfnet/pfrl/master/assets/PFRL.png" height=150/></div>
+
+# PFRL
+[![Documentation Status](https://readthedocs.org/projects/pfrl/badge/?version=latest)](http://pfrl.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/pfrl.svg)](https://pypi.python.org/pypi/pfrl)
+
+PFRL is a deep reinforcement learning library that implements various state-of-the-art deep reinforcement algorithms in Python using [PyTorch](https://github.com/pytorch/pytorch).
+
+![Boxing](assets/boxing.gif)
+![Humanoid](assets/humanoid.gif)
+![Grasping](assets/grasping.gif)
+![Atlas](examples/atlas/assets/atlas.gif)
+![SlimeVolley](examples/slimevolley/assets/slimevolley.gif)
+
+## Installation
+
+PFRL is tested with Python 3.7.7. For other requirements, see [requirements.txt](requirements.txt).
+
+PFRL can be installed via PyPI:
+```
+pip install pfrl
+```
+
+It can also be installed from the source code:
+```
+python setup.py install
+```
+
+Refer to [Installation](http://pfrl.readthedocs.io/en/latest/install.html) for more information on installation. 
+
+## Getting started
+
+You can try [PFRL Quickstart Guide](examples/quickstart/quickstart.ipynb) first, or check the [examples](examples) ready for Atari 2600 and Open AI Gym.
+
+For more information, you can refer to [PFRL's documentation](http://pfrl.readthedocs.io/en/latest/index.html).
+
+### Blog Posts
+- [Introducing PFRL: A PyTorch-based Deep RL Library](https://t.co/VaT06nejSC?amp=1)
+- [PFRL’s Pretrained Model Zoo](https://bit.ly/3fNx5xH)
+
+## Algorithms
+
+| Algorithm | Discrete Action | Continous Action | Recurrent Model | Batch Training | CPU Async Training | Pretrained models<sup>*</sup> |
+|:----------|:---------------:|:----------------:|:---------------:|:--------------:|:------------------:|:------------------:|
+| DQN (including DoubleDQN etc.) | ✓ | ✓ (NAF) | ✓ | ✓ | x | ✓ |
+| Categorical DQN | ✓ | x | ✓ | ✓ | x | x |
+| Rainbow | ✓ | x | ✓ | ✓ | x | ✓ |
+| IQN | ✓ | x | ✓ | ✓ | x | ✓ |
+| DDPG | x | ✓ | x | ✓ | x | ✓ |
+| A3C  | ✓ | ✓ | ✓ | ✓ (A2C) | ✓ | ✓ |
+| ACER | ✓ | ✓ | ✓ | x | ✓ | x |
+| PPO  | ✓ | ✓ | ✓ | ✓ | x | ✓ |
+| TRPO | ✓ | ✓ | ✓ | ✓ | x | ✓ |
+| TD3 | x | ✓ | x | ✓ | x | ✓ |
+| SAC | x | ✓ | x | ✓ | x | ✓ |
+
+**<sup>*</sup>Note on Pretrained models**: PFRL provides pretrained models (sometimes called a 'model zoo') for our reproducibility scripts on [Atari environments](https://github.com/pfnet/pfrl/tree/master/examples/atari/reproduction) (DQN, IQN, Rainbow, and A3C) and [Mujoco environments](https://github.com/pfnet/pfrl/tree/master/examples/mujoco/reproduction) (DDPG, TRPO, PPO, TD3, SAC), for each benchmarked environment. 
+
+Following algorithms have been implemented in PFRL:
+- [A2C (Synchronous variant of A3C)](https://openai.com/blog/baselines-acktr-a2c/)
+  - examples: [[atari (batched)]](examples/atari/train_a2c_ale.py)
+- [A3C (Asynchronous Advantage Actor-Critic)](https://arxiv.org/abs/1602.01783)
+  - examples: [[atari reproduction]](examples/atari/reproduction/a3c) [[atari]](examples/atari/train_a3c_ale.py)
+- [ACER (Actor-Critic with Experience Replay)](https://arxiv.org/abs/1611.01224)
+  - examples: [[atari]](examples/atari/train_acer_ale.py)
+- [Categorical DQN](https://arxiv.org/abs/1707.06887)
+  - examples: [[atari]](examples/atari/train_categorical_dqn_ale.py) [[general gym]](examples/gym/train_categorical_dqn_gym.py)
+- [DQN (Deep Q-Network)](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf) (including [Double DQN](https://arxiv.org/abs/1509.06461), [Persistent Advantage Learning (PAL)](https://arxiv.org/abs/1512.04860), Double PAL, [Dynamic Policy Programming (DPP)](http://www.jmlr.org/papers/volume13/azar12a/azar12a.pdf))
+  - examples: [[atari reproduction]](examples/atari/reproduction/dqn) [[atari]](examples/atari/train_dqn_ale.py) [[atari (batched)]](examples/atari/train_dqn_batch_ale.py) [[flickering atari]](examples/atari/train_drqn_ale.py) [[general gym]](examples/gym/train_dqn_gym.py)
+- [DDPG (Deep Deterministic Policy Gradients)](https://arxiv.org/abs/1509.02971) (including [SVG(0)](https://arxiv.org/abs/1510.09142))
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ddpg)
+- [IQN (Implicit Quantile Networks)](https://arxiv.org/abs/1806.06923)
+  - examples: [[atari reproduction]](examples/atari/reproduction/iqn)
+- [PPO (Proximal Policy Optimization)](https://arxiv.org/abs/1707.06347)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ppo) [[atari]](examples/atari/train_ppo_ale.py)
+- [Rainbow](https://arxiv.org/abs/1710.02298)
+  - examples: [[atari reproduction]](examples/atari/reproduction/rainbow) [[Slime volleyball]](examples/slimevolley/)
+- [REINFORCE](http://www-anw.cs.umass.edu/~barto/courses/cs687/williams92simple.pdf)
+  - examples: [[general gym]](examples/gym/train_reinforce_gym.py)
+- [SAC (Soft Actor-Critic)](https://arxiv.org/abs/1812.05905)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/soft_actor_critic) [[Atlas walk]](examples/atlas/)
+- [TRPO (Trust Region Policy Optimization)](https://arxiv.org/abs/1502.05477) with [GAE (Generalized Advantage Estimation)](https://arxiv.org/abs/1506.02438)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/trpo)
+- [TD3 (Twin Delayed Deep Deterministic policy gradient algorithm)](https://arxiv.org/abs/1802.09477)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/td3)
+
+Following useful techniques have been also implemented in PFRL:
+- [NoisyNet](https://arxiv.org/abs/1706.10295)
+  - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
+- [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952)
+  - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
+- [Dueling Network](https://arxiv.org/abs/1511.06581)
+  - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
+- [Normalized Advantage Function](https://arxiv.org/abs/1603.00748)
+  - examples: [[DQN]](examples/gym/train_dqn_gym.py) (for continuous-action envs only)
+- [Deep Recurrent Q-Network](https://arxiv.org/abs/1507.06527)
+  - examples: [[DQN]](examples/atari/train_drqn_ale.py)
+
+
+## Environments
+
+Environments that support the subset of OpenAI Gym's interface (`reset` and `step` methods) can be used.
+
+## Contributing
+
+Any kind of contribution to PFRL would be highly appreciated! If you are interested in contributing to PFRL, please read [CONTRIBUTING.md](CONTRIBUTING.md).
+
+## License
+
+[MIT License](LICENSE).
+
+## Citations
+
+To cite PFRL in publications, please cite our [paper](https://www.jmlr.org/papers/v22/20-376.html) on ChainerRL, the library on which PFRL is based:
+
+```
+@article{JMLR:v22:20-376,
+  author  = {Yasuhiro Fujita and Prabhat Nagarajan and Toshiki Kataoka and Takahiro Ishikawa},
+  title   = {ChainerRL: A Deep Reinforcement Learning Library},
+  journal = {Journal of Machine Learning Research},
+  year    = {2021},
+  volume  = {22},
+  number  = {77},
+  pages   = {1-14},
+  url     = {http://jmlr.org/papers/v22/20-376.html}
+}
+```
```

### Comparing `pfrl-0.3.0/README.md` & `pfrl-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/__init__.py` & `pfrl-0.4.0/pfrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/action_value.py` & `pfrl-0.4.0/pfrl/action_value.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agent.py` & `pfrl-0.4.0/pfrl/agent.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agents/__init__.py` & `pfrl-0.4.0/pfrl/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agents/a2c.py` & `pfrl-0.4.0/pfrl/agents/a2c.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         act_deterministically=False,
         max_grad_norm=None,
         average_actor_loss_decay=0.999,
         average_entropy_decay=0.999,
         average_value_decay=0.999,
         batch_states=batch_states,
     ):
-
         self.model = model
         if gpu is not None and gpu >= 0:
             assert torch.cuda.is_available()
             self.device = torch.device("cuda:{}".format(gpu))
             self.model.to(self.device)
         else:
             self.device = torch.device("cpu")
```

### Comparing `pfrl-0.3.0/pfrl/agents/a3c.py` & `pfrl-0.4.0/pfrl/agents/a3c.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         act_deterministically=False,
         max_grad_norm=None,
         recurrent=False,
         average_entropy_decay=0.999,
         average_value_decay=0.999,
         batch_states=batch_states,
     ):
-
         # Globally shared model
         self.shared_model = model
 
         # Thread specific model
         self.model = copy.deepcopy(self.shared_model)
 
         self.optimizer = optimizer
@@ -237,15 +236,14 @@
     def observe(self, obs, reward, done, reset):
         if self.training:
             self._observe_train(obs, reward, done, reset)
         else:
             self._observe_eval(obs, reward, done, reset)
 
     def _act_train(self, obs):
-
         self.past_obs[self.t] = obs
 
         with torch.no_grad():
             statevar = self.batch_states([obs], self.device, self.phi)
             if self.recurrent:
                 self.past_recurrent_state[self.t] = self.train_recurrent_states
                 (pout, vout), self.train_recurrent_states = one_step_forward(
```

### Comparing `pfrl-0.3.0/pfrl/agents/acer.py` & `pfrl-0.4.0/pfrl/agents/acer.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,26 +317,25 @@
         Q_loss_coef=0.5,
         use_trust_region=True,
         trust_region_alpha=0.99,
         trust_region_delta=1,
         truncation_threshold=10,
         disable_online_update=False,
         n_times_replay=8,
-        replay_start_size=10 ** 4,
+        replay_start_size=10**4,
         normalize_loss_by_steps=True,
         act_deterministically=False,
         max_grad_norm=None,
         recurrent=False,
         use_Q_opc=False,
         average_entropy_decay=0.999,
         average_value_decay=0.999,
         average_kl_decay=0.999,
         logger=None,
     ):
-
         # Globally shared model
         self.shared_model = model
 
         # Globally shared average model used to compute trust regions
         self.shared_average_model = copy.deepcopy(self.shared_model)
 
         # Thread specific model
@@ -468,15 +467,14 @@
         rewards,
         values,
         action_values,
         action_distribs,
         action_distribs_mu,
         avg_action_distribs,
     ):
-
         assert np.isscalar(R)
         pi_loss = 0
         Q_loss = 0
         Q_ret = R
         Q_opc = R
         discrete = isinstance(action_distribs[t_start], torch.distributions.Categorical)
         del R
@@ -562,15 +560,14 @@
         rewards,
         values,
         action_values,
         action_distribs,
         action_distribs_mu,
         avg_action_distribs,
     ):
-
         assert np.isscalar(R)
         self.assert_shared_memory()
 
         total_loss = self.compute_loss(
             t_start=t_start,
             t_stop=t_stop,
             R=R,
@@ -591,15 +588,14 @@
         # Copy the gradients to the globally shared model
         copy_param.copy_grad(target_link=self.shared_model, source_link=self.model)
         self.optimizer.step()
 
         self.sync_parameters()
 
     def update_from_replay(self):
-
         if self.replay_buffer is None:
             return
 
         if len(self.replay_buffer) < self.replay_start_size:
             return
 
         episode = self.replay_buffer.sample_episodes(1, self.t_max)[0]
@@ -711,15 +707,14 @@
     def observe(self, obs, reward, done, reset):
         if self.training:
             self._observe_train(obs, reward, done, reset)
         else:
             self._observe_eval(obs, reward, done, reset)
 
     def _act_train(self, obs):
-
         statevar = batch_states([obs], self.device, self.phi)
 
         if self.recurrent:
             (
                 (action_distrib, action_value, v),
                 self.train_recurrent_states,
             ) = one_step_forward(self.model, statevar, self.train_recurrent_states)
```

### Comparing `pfrl-0.3.0/pfrl/agents/al.py` & `pfrl-0.4.0/pfrl/agents/al.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     """
 
     def __init__(self, *args, **kwargs):
         self.alpha = kwargs.pop("alpha", 0.9)
         super().__init__(*args, **kwargs)
 
     def _compute_y_and_t(self, exp_batch):
-
         batch_state = exp_batch["state"]
         batch_size = len(exp_batch["reward"])
 
         if self.recurrent:
             qout, _ = pack_and_forward(
                 self.model,
                 batch_state,
```

### Comparing `pfrl-0.3.0/pfrl/agents/categorical_double_dqn.py` & `pfrl-0.4.0/pfrl/agents/categorical_double_dqn.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agents/categorical_dqn.py` & `pfrl-0.4.0/pfrl/agents/categorical_dqn.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agents/ddpg.py` & `pfrl-0.4.0/pfrl/agents/ddpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         n_times_update=1,
         recurrent=False,
         episodic_update_len=None,
         logger=getLogger(__name__),
         batch_states=batch_states,
         burnin_action_func=None,
     ):
-
         self.model = nn.ModuleList([policy, q_func])
         if gpu is not None and gpu >= 0:
             assert torch.cuda.is_available()
             self.device = torch.device("cuda:{}".format(gpu))
             self.model.to(self.device)
         else:
             self.device = torch.device("cpu")
@@ -219,30 +218,28 @@
                 transitions.append([ep[i]])
             batch = batch_experiences(
                 transitions, xp=self.device, phi=self.phi, gamma=self.gamma
             )
             batches.append(batch)
 
         with self.model.state_reset(), self.target_model.state_reset():
-
             # Since the target model is evaluated one-step ahead,
             # its internal states need to be updated
             self.target_q_function.update_state(
                 batches[0]["state"], batches[0]["action"]
             )
             self.target_policy(batches[0]["state"])
 
             # Update critic through time
             critic_loss = 0
             for batch in batches:
                 critic_loss += self.compute_critic_loss(batch)
             self.critic_optimizer.update(lambda: critic_loss / max_epi_len)
 
         with self.model.state_reset():
-
             # Update actor through time
             actor_loss = 0
             for batch in batches:
                 actor_loss += self.compute_actor_loss(batch)
             self.actor_optimizer.update(lambda: actor_loss / max_epi_len)
 
     def batch_act(self, batch_obs):
```

### Comparing `pfrl-0.3.0/pfrl/agents/double_dqn.py` & `pfrl-0.4.0/pfrl/agents/double_dqn.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 class DoubleDQN(dqn.DQN):
     """Double DQN.
 
     See: http://arxiv.org/abs/1509.06461.
     """
 
     def _compute_target_values(self, exp_batch):
-
         batch_next_state = exp_batch["next_state"]
 
         with evaluating(self.model):
             if self.recurrent:
                 next_qout, _ = pack_and_forward(
                     self.model,
                     batch_next_state,
```

### Comparing `pfrl-0.3.0/pfrl/agents/double_pal.py` & `pfrl-0.4.0/pfrl/agents/double_pal.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pfrl.agents import pal
 from pfrl.utils.recurrent import pack_and_forward
 
 
 class DoublePAL(pal.PAL):
     def _compute_y_and_t(self, exp_batch):
-
         batch_state = exp_batch["state"]
         batch_size = len(exp_batch["reward"])
 
         if self.recurrent:
             qout, _ = pack_and_forward(
                 self.model,
                 batch_state,
```

### Comparing `pfrl-0.3.0/pfrl/agents/dpp.py` & `pfrl-0.4.0/pfrl/agents/dpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     """
 
     @abstractmethod
     def _l_operator(self, qout):
         raise NotImplementedError()
 
     def _compute_target_values(self, exp_batch):
-
         batch_next_state = exp_batch["next_state"]
 
         if self.recurrent:
             target_next_qout, _ = pack_and_forward(
                 self.target_model,
                 batch_next_state,
                 exp_batch["next_recurrent_state"],
@@ -34,15 +33,14 @@
         batch_terminal = exp_batch["is_state_terminal"]
 
         return (
             batch_rewards + exp_batch["discount"] * (1 - batch_terminal) * next_q_expect
         )
 
     def _compute_y_and_t(self, exp_batch):
-
         batch_state = exp_batch["state"]
         batch_size = len(exp_batch["reward"])
 
         if self.recurrent:
             qout, _ = pack_and_forward(
                 self.model,
                 batch_state,
```

### Comparing `pfrl-0.3.0/pfrl/agents/dqn.py` & `pfrl-0.4.0/pfrl/agents/dqn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import collections
 import copy
 import ctypes
 import multiprocessing as mp
 import multiprocessing.synchronize
+import os
 import time
+import typing
 from logging import Logger, getLogger
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 
@@ -32,15 +34,15 @@
     pack_and_forward,
     recurrent_state_as_numpy,
 )
 
 
 def _mean_or_nan(xs: Sequence[float]) -> float:
     """Return its mean a non-empty sequence, numpy.nan for a empty one."""
-    return np.mean(xs) if xs else np.nan
+    return typing.cast(float, np.mean(xs)) if xs else np.nan
 
 
 def compute_value_loss(
     y: torch.Tensor,
     t: torch.Tensor,
     clip_delta: bool = True,
     batch_accumulator: str = "mean",
@@ -507,15 +509,14 @@
     def _batch_observe_train(
         self,
         batch_obs: Sequence[Any],
         batch_reward: Sequence[float],
         batch_done: Sequence[bool],
         batch_reset: Sequence[bool],
     ) -> None:
-
         for i in range(len(batch_obs)):
             self.t += 1
             self._cumulative_steps += 1
             # Update the target network
             if self.t % self.target_update_interval == 0:
                 self.sync_target_network()
             if self.batch_last_obs[i] is not None:
@@ -786,14 +787,32 @@
 
         return make_actor, learner, poller, exception_event
 
     def stop_episode(self) -> None:
         if self.recurrent:
             self.test_recurrent_states = None
 
+    def save_snapshot(self, dirname: str) -> None:
+        self.save(dirname)
+        torch.save(self.t, os.path.join(dirname, "t.pt"))
+        torch.save(self.optim_t, os.path.join(dirname, "optim_t.pt"))
+        torch.save(
+            self._cumulative_steps, os.path.join(dirname, "_cumulative_steps.pt")
+        )
+        self.replay_buffer.save(os.path.join(dirname, "replay_buffer.pkl"))
+
+    def load_snapshot(self, dirname: str) -> None:
+        self.load(dirname)
+        self.t = torch.load(os.path.join(dirname, "t.pt"))
+        self.optim_t = torch.load(os.path.join(dirname, "optim_t.pt"))
+        self._cumulative_steps = torch.load(
+            os.path.join(dirname, "_cumulative_steps.pt")
+        )
+        self.replay_buffer.load(os.path.join(dirname, "replay_buffer.pkl"))
+
     def get_statistics(self):
         return [
             ("average_q", _mean_or_nan(self.q_record)),
             ("average_loss", _mean_or_nan(self.loss_record)),
             ("cumulative_steps", self.cumulative_steps),
             ("n_updates", self.optim_t),
             ("rlen", len(self.replay_buffer)),
```

### Comparing `pfrl-0.3.0/pfrl/agents/iqn.py` & `pfrl-0.4.0/pfrl/agents/iqn.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agents/pal.py` & `pfrl-0.4.0/pfrl/agents/pal.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     """
 
     def __init__(self, *args, **kwargs):
         self.alpha = kwargs.pop("alpha", 0.9)
         super().__init__(*args, **kwargs)
 
     def _compute_y_and_t(self, exp_batch):
-
         batch_state = exp_batch["state"]
         batch_size = len(exp_batch["reward"])
 
         if self.recurrent:
             qout, _ = pack_and_forward(
                 self.model,
                 batch_state,
```

### Comparing `pfrl-0.3.0/pfrl/agents/ppo.py` & `pfrl-0.4.0/pfrl/agents/ppo.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
     episodes,
     model,
     phi,
     batch_states,
     obs_normalizer,
     device,
 ):
-
     dataset = list(itertools.chain.from_iterable(episodes))
 
     # Compute v_pred and next_v_pred
     states = batch_states([b["state"] for b in dataset], device, phi)
     next_states = batch_states([b["next_state"] for b in dataset], device, phi)
 
     if obs_normalizer:
@@ -283,15 +282,15 @@
             to update value function. If it is ``None``, value function is not
             clipped on updates.
         standardize_advantages (bool): Use standardized advantages on updates
         recurrent (bool): If set to True, `model` is assumed to implement
             `pfrl.nn.Recurrent` and update in a recurrent
             manner.
         max_recurrent_sequence_len (int): Maximum length of consecutive
-            sequences of transitions in a minibatch for updatig the model.
+            sequences of transitions in a minibatch for updating the model.
             This value is used only when `recurrent` is True. A smaller value
             will encourage a minibatch to contain more and shorter sequences.
         act_deterministically (bool): If set to True, choose most probable
             actions in the act method instead of sampling from distributions.
         max_grad_norm (float or None): Maximum L2 norm of the gradient used for
             gradient clipping. If set to None, the gradient is not clipped.
         value_stats_window (int): Window size used to compute statistics
@@ -529,15 +528,14 @@
                 torch.nn.utils.clip_grad_norm_(
                     self.model.parameters(), self.max_grad_norm
                 )
             self.optimizer.step()
             self.n_updates += 1
 
     def _update_once_recurrent(self, episodes, mean_advs, std_advs):
-
         assert std_advs is None or std_advs > 0
 
         device = self.device
 
         # Sort desc by lengths so that pack_sequence does not change the order
         episodes = sorted(episodes, key=len, reverse=True)
 
@@ -632,15 +630,14 @@
                 dataset, self.minibatch_size
             ):
                 self._update_once_recurrent(minibatch, mean_advs, std_advs)
 
     def _lossfun(
         self, entropy, vs_pred, log_probs, vs_pred_old, log_probs_old, advs, vs_teacher
     ):
-
         prob_ratio = torch.exp(log_probs - log_probs_old)
 
         loss_policy = -torch.mean(
             torch.min(
                 prob_ratio * advs,
                 torch.clamp(prob_ratio, 1 - self.clip_eps, 1 + self.clip_eps) * advs,
             ),
```

### Comparing `pfrl-0.3.0/pfrl/agents/reinforce.py` & `pfrl-0.4.0/pfrl/agents/reinforce.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         average_entropy_decay=0.999,
         backward_separately=False,
         batch_states=pfrl.utils.batch_states,
         recurrent=False,
         max_grad_norm=None,
         logger=None,
     ):
-
         self.model = model
         if gpu is not None and gpu >= 0:
             assert torch.cuda.is_available()
             self.device = torch.device("cuda:{}".format(gpu))
             self.model.to(self.device)
         else:
             self.device = torch.device("cpu")
@@ -99,15 +98,14 @@
     def observe(self, obs, reward, done, reset):
         if self.training:
             self._observe_train(obs, reward, done, reset)
         else:
             self._observe_eval(obs, reward, done, reset)
 
     def _act_train(self, obs):
-
         batch_obs = self.batch_states([obs], self.device, self.phi)
         if self.recurrent:
             action_distrib, self.train_recurrent_states = one_step_forward(
                 self.model, batch_obs, self.train_recurrent_states
             )
         else:
             action_distrib = self.model(batch_obs)
```

### Comparing `pfrl-0.3.0/pfrl/agents/soft_actor_critic.py` & `pfrl-0.4.0/pfrl/agents/soft_actor_critic.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         batch_states=batch_states,
         burnin_action_func=None,
         initial_temperature=1.0,
         entropy_target=None,
         temperature_optimizer_lr=None,
         act_deterministically=True,
     ):
-
         self.policy = policy
         self.q_func1 = q_func1
         self.q_func2 = q_func2
 
         if gpu is not None and gpu >= 0:
             assert torch.cuda.is_available()
             self.device = torch.device("cuda:{}".format(gpu))
```

### Comparing `pfrl-0.3.0/pfrl/agents/state_q_function_actor.py` & `pfrl-0.4.0/pfrl/agents/state_q_function_actor.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/agents/td3.py` & `pfrl-0.4.0/pfrl/agents/td3.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         max_grad_norm=None,
         logger=getLogger(__name__),
         batch_states=batch_states,
         burnin_action_func=None,
         policy_update_delay=2,
         target_policy_smoothing_func=default_target_policy_smoothing_func,
     ):
-
         self.policy = policy
         self.q_func1 = q_func1
         self.q_func2 = q_func2
 
         if gpu is not None and gpu >= 0:
             assert torch.cuda.is_available()
             self.device = torch.device("cuda:{}".format(gpu))
```

### Comparing `pfrl-0.3.0/pfrl/agents/trpo.py` & `pfrl-0.4.0/pfrl/agents/trpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,14 @@
         max_grad_norm=None,
         value_stats_window=1000,
         entropy_stats_window=1000,
         kl_stats_window=100,
         policy_step_size_stats_window=100,
         logger=getLogger(__name__),
     ):
-
         self.policy = policy
         self.vf = vf
         self.vf_optimizer = vf_optimizer
         self.obs_normalizer = obs_normalizer
         self.gamma = gamma
         self.lambd = lambd
         self.phi = phi
@@ -331,26 +330,24 @@
         if self.obs_normalizer:
             self._update_obs_normalizer(flat_dataset)
 
         self._update_policy_recurrent(dataset)
         self._update_vf_recurrent(dataset)
 
     def _update_vf_recurrent(self, dataset):
-
         for epoch in range(self.vf_epochs):
             random.shuffle(dataset)
             for (
                 minibatch
             ) in _yield_subset_of_sequences_with_fixed_number_of_items(  # NOQA
                 dataset, self.vf_batch_size
             ):
                 self._update_vf_once_recurrent(minibatch)
 
     def _update_vf_once_recurrent(self, episodes):
-
         # Sort episodes desc by length for pack_sequence
         episodes = sorted(episodes, key=len, reverse=True)
 
         flat_transitions = flatten_sequences_time_first(episodes)
 
         # Prepare data for a recurrent model
         seqs_states = []
```

### Comparing `pfrl-0.3.0/pfrl/collections/persistent_collections.py` & `pfrl-0.4.0/pfrl/collections/persistent_collections.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/collections/prioritized.py` & `pfrl-0.4.0/pfrl/collections/prioritized.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import collections
-from numbers import Number
 from typing import (
     Any,
     Callable,
     Deque,
     Generic,
     List,
     Optional,
@@ -239,15 +238,15 @@
         if ixc == 0:
             ixl = ixc
             _, self.root, _ = self.root
         self.bounds = ixl, ixr
         return ret
 
 
-def _find(index_left: int, index_right: int, node: Node, pos: Number) -> int:
+def _find(index_left: int, index_right: int, node: Node, pos: float) -> int:
     if index_right - index_left == 1:
         return index_left
     else:
         node_left, node_right, _ = node
         index_center = (index_left + index_right) // 2
         if node_left:
             left_value = node_left[2]
```

### Comparing `pfrl-0.3.0/pfrl/collections/random_access_queue.py` & `pfrl-0.4.0/pfrl/collections/random_access_queue.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/distributions/delta.py` & `pfrl-0.4.0/pfrl/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/env.py` & `pfrl-0.4.0/pfrl/env.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/envs/abc.py` & `pfrl-0.4.0/pfrl/envs/abc.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/envs/multiprocess_vector_env.py` & `pfrl-0.4.0/pfrl/envs/multiprocess_vector_env.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/envs/serial_vector_env.py` & `pfrl-0.4.0/pfrl/envs/serial_vector_env.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/experiments/__init__.py` & `pfrl-0.4.0/pfrl/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/experiments/evaluation_hooks.py` & `pfrl-0.4.0/pfrl/experiments/evaluation_hooks.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/experiments/evaluator.py` & `pfrl-0.4.0/pfrl/experiments/evaluator.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/experiments/hooks.py` & `pfrl-0.4.0/pfrl/experiments/hooks.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/experiments/prepare_output_dir.py` & `pfrl-0.4.0/pfrl/experiments/prepare_output_dir.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/experiments/train_agent.py` & `pfrl-0.4.0/pfrl/experiments/train_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     step_offset=0,
     evaluator=None,
     successful_score=None,
     step_hooks=(),
     eval_during_episode=False,
     logger=None,
 ):
-
     logger = logger or logging.getLogger(__name__)
 
     episode_r = 0
     episode_idx = 0
 
     # o_0, r_0
     obs = env.reset()
@@ -48,15 +47,14 @@
     if hasattr(agent, "t"):
         agent.t = step_offset
 
     eval_stats_history = []  # List of evaluation episode stats dict
     episode_len = 0
     try:
         while t < steps:
-
             # a_t
             action = agent.act(obs)
             # o_{t+1}, r_{t+1}
             obs, r, done, info = env.step(action)
             t += 1
             episode_r += r
             episode_len += 1
```

### Comparing `pfrl-0.3.0/pfrl/experiments/train_agent_async.py` & `pfrl-0.4.0/pfrl/experiments/train_agent_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,39 +37,36 @@
     max_episode_len=None,
     evaluator=None,
     eval_env=None,
     successful_score=None,
     logger=None,
     global_step_hooks=[],
 ):
-
     logger = logger or logging.getLogger(__name__)
 
     if eval_env is None:
         eval_env = env
 
     def save_model():
         if process_idx == 0:
             # Save the current model before being killed
             dirname = os.path.join(outdir, "{}_except".format(global_t))
             agent.save(dirname)
             logger.info("Saved the current model to %s", dirname)
 
     try:
-
         episode_r = 0
         global_t = 0
         local_t = 0
         global_episodes = 0
         obs = env.reset()
         episode_len = 0
         successful = False
 
         while True:
-
             # a_t
             a = agent.act(obs)
             # o_{t+1}, r_{t+1}
             obs, r, done, info = env.step(a)
             local_t += 1
             episode_r += r
             episode_len += 1
@@ -147,16 +144,16 @@
 
 
 def train_agent_async(
     outdir,
     processes,
     make_env,
     profile=False,
-    steps=8 * 10 ** 7,
-    eval_interval=10 ** 6,
+    steps=8 * 10**7,
+    eval_interval=10**6,
     eval_n_steps=None,
     eval_n_episodes=10,
     eval_success_threshold=0.0,
     max_episode_len=None,
     step_offset=0,
     successful_score=None,
     agent=None,
```

### Comparing `pfrl-0.3.0/pfrl/experiments/train_agent_batch.py` & `pfrl-0.4.0/pfrl/experiments/train_agent_batch.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/explorers/additive_gaussian.py` & `pfrl-0.4.0/pfrl/explorers/additive_gaussian.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/explorers/additive_ou.py` & `pfrl-0.4.0/pfrl/explorers/additive_ou.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def select_action(self, t, greedy_action_func, action_value=None):
         a = greedy_action_func()
         if self.ou_state is None:
             if self.start_with_mu:
                 self.ou_state = np.full(a.shape, self.mu, dtype=np.float32)
             else:
-                sigma_stable = self.sigma / np.sqrt(2 * self.theta - self.theta ** 2)
+                sigma_stable = self.sigma / np.sqrt(2 * self.theta - self.theta**2)
                 self.ou_state = np.random.normal(
                     size=a.shape, loc=self.mu, scale=sigma_stable
                 ).astype(np.float32)
         else:
             self.evolve()
         noise = self.ou_state
         self.logger.debug("t:%s noise:%s", t, noise)
```

### Comparing `pfrl-0.3.0/pfrl/explorers/boltzmann.py` & `pfrl-0.4.0/pfrl/explorers/boltzmann.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/explorers/epsilon_greedy.py` & `pfrl-0.4.0/pfrl/explorers/epsilon_greedy.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.end_epsilon = end_epsilon
         self.decay = decay
         self.random_action_func = random_action_func
         self.logger = logger
         self.epsilon = start_epsilon
 
     def compute_epsilon(self, t):
-        epsilon = self.start_epsilon * (self.decay ** t)
+        epsilon = self.start_epsilon * (self.decay**t)
         return max(epsilon, self.end_epsilon)
 
     def select_action(self, t, greedy_action_func, action_value=None):
         self.epsilon = self.compute_epsilon(t)
         a, greedy = select_action_epsilon_greedily(
             self.epsilon, self.random_action_func, greedy_action_func
         )
```

### Comparing `pfrl-0.3.0/pfrl/functions/bound_by_tanh.py` & `pfrl-0.4.0/pfrl/functions/bound_by_tanh.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/functions/lower_triangular_matrix.py` & `pfrl-0.4.0/pfrl/functions/lower_triangular_matrix.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/initializers/chainer_default.py` & `pfrl-0.4.0/pfrl/initializers/chainer_default.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/__init__.py` & `pfrl-0.4.0/pfrl/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/atari_cnn.py` & `pfrl-0.4.0/pfrl/nn/atari_cnn.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/branched.py` & `pfrl-0.4.0/pfrl/nn/branched.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/empirical_normalization.py` & `pfrl-0.4.0/pfrl/nn/empirical_normalization.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/mlp.py` & `pfrl-0.4.0/pfrl/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/mlp_bn.py` & `pfrl-0.4.0/pfrl/nn/mlp_bn.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/noisy_chain.py` & `pfrl-0.4.0/pfrl/nn/noisy_chain.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/noisy_linear.py` & `pfrl-0.4.0/pfrl/nn/noisy_linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     fan_in = torch.nn.init._calculate_correct_fan(tensor, "fan_in")
     s = scale * np.sqrt(3.0 / fan_in)
     with torch.no_grad():
         return tensor.uniform_(-s, s)
 
 
 def init_variance_scaling_constant(tensor, scale=1.0):
-
     if tensor.ndim == 1:
         s = scale / np.sqrt(tensor.shape[0])
     else:
         fan_in = torch.nn.init._calculate_correct_fan(tensor, "fan_in")
         s = scale / np.sqrt(fan_in)
     with torch.no_grad():
         return tensor.fill_(s)
```

### Comparing `pfrl-0.3.0/pfrl/nn/recurrent.py` & `pfrl-0.4.0/pfrl/nn/recurrent.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/recurrent_branched.py` & `pfrl-0.4.0/pfrl/nn/recurrent_branched.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/nn/recurrent_sequential.py` & `pfrl-0.4.0/pfrl/nn/recurrent_sequential.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/optimizers/rmsprop_eps_inside_sqrt.py` & `pfrl-0.4.0/pfrl/optimizers/rmsprop_eps_inside_sqrt.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/policies/gaussian_policy.py` & `pfrl-0.4.0/pfrl/policies/gaussian_policy.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/q_function.py` & `pfrl-0.4.0/pfrl/q_function.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/q_functions/dueling_dqn.py` & `pfrl-0.4.0/pfrl/q_functions/dueling_dqn.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/q_functions/state_action_q_functions.py` & `pfrl-0.4.0/pfrl/q_functions/state_action_q_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             [self.n_hidden_channels] * self.n_hidden_layers,
             nonlinearity=nonlinearity,
         )
         self.lstm = nn.LSTM(
             num_layers=1, input_size=n_hidden_channels, hidden_size=n_hidden_channels
         )
         self.out = nn.Linear(n_hidden_channels, 1)
-        for (n, p) in self.lstm.named_parameters():
+        for n, p in self.lstm.named_parameters():
             if "weight" in n:
                 init_lecun_normal(p)
             else:
                 nn.init.zeros_(p)
 
         init_lecun_normal(self.out.weight, scale=last_wscale)
         nn.init.zeros_(self.out.bias)
```

### Comparing `pfrl-0.3.0/pfrl/q_functions/state_q_functions.py` & `pfrl-0.4.0/pfrl/q_functions/state_q_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         mat_diag = torch.exp(self.mat_diag(h))
         if hasattr(self, "mat_non_diag"):
             mat_non_diag = self.mat_non_diag(h)
             tril = lower_triangular_matrix(mat_diag, mat_non_diag)
             mat = torch.matmul(tril, torch.transpose(tril, 1, 2))
         else:
-            mat = torch.unsqueeze(mat_diag ** 2, dim=2)
+            mat = torch.unsqueeze(mat_diag**2, dim=2)
         return QuadraticActionValue(
             mu,
             mat,
             v,
             min_action=self.action_space.low,
             max_action=self.action_space.high,
         )
```

### Comparing `pfrl-0.3.0/pfrl/replay_buffer.py` & `pfrl-0.4.0/pfrl/replay_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     batch_exp = {
         "state": batch_states([elem[0]["state"] for elem in experiences], device, phi),
         "action": torch.as_tensor(
             [elem[0]["action"] for elem in experiences], device=device
         ),
         "reward": torch.as_tensor(
             [
-                sum((gamma ** i) * exp[i]["reward"] for i in range(len(exp)))
+                sum((gamma**i) * exp[i]["reward"] for i in range(len(exp)))
                 for exp in experiences
             ],
             dtype=torch.float32,
             device=device,
         ),
         "next_state": batch_states(
             [elem[-1]["next_state"] for elem in experiences], device, phi
@@ -312,15 +312,14 @@
         batchsize,
         episodic_update,
         n_times_update,
         replay_start_size,
         update_interval,
         episodic_update_len=None,
     ):
-
         assert batchsize <= replay_start_size
         self.replay_buffer = replay_buffer
         self.update_func = update_func
         self.batchsize = batchsize
         self.episodic_update = episodic_update
         self.episodic_update_len = episodic_update_len
         self.n_times_update = n_times_update
```

### Comparing `pfrl-0.3.0/pfrl/replay_buffers/__init__.py` & `pfrl-0.4.0/pfrl/replay_buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/replay_buffers/episodic.py` & `pfrl-0.4.0/pfrl/replay_buffers/episodic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Optional
 
 from pfrl.collections.random_access_queue import RandomAccessQueue
 from pfrl.replay_buffer import AbstractEpisodicReplayBuffer, random_subseq
 
 
 class EpisodicReplayBuffer(AbstractEpisodicReplayBuffer):
-
     # Implements AbstractReplayBuffer.capacity
     capacity: Optional[int] = None
 
     def __init__(self, capacity=None):
         self.current_episode = collections.defaultdict(list)
         self.episodic_memory = RandomAccessQueue()
         self.memory = RandomAccessQueue()
```

### Comparing `pfrl-0.3.0/pfrl/replay_buffers/persistent.py` & `pfrl-0.4.0/pfrl/replay_buffers/persistent.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/replay_buffers/prioritized.py` & `pfrl-0.4.0/pfrl/replay_buffers/prioritized.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/replay_buffers/prioritized_episodic.py` & `pfrl-0.4.0/pfrl/replay_buffers/prioritized_episodic.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/replay_buffers/replay_buffer.py` & `pfrl-0.4.0/pfrl/replay_buffers/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/testing.py` & `pfrl-0.4.0/pfrl/testing.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/__init__.py` & `pfrl-0.4.0/pfrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/async_.py` & `pfrl-0.4.0/pfrl/utils/async_.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/batch_states.py` & `pfrl-0.4.0/pfrl/utils/batch_states.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/clip_l2_grad_norm.py` & `pfrl-0.4.0/pfrl/utils/clip_l2_grad_norm.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/conjugate_gradient.py` & `pfrl-0.4.0/pfrl/utils/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/copy_param.py` & `pfrl-0.4.0/pfrl/utils/copy_param.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/env_modifiers.py` & `pfrl-0.4.0/pfrl/utils/env_modifiers.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/is_return_code_zero.py` & `pfrl-0.4.0/pfrl/utils/is_return_code_zero.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/mode_of_distribution.py` & `pfrl-0.4.0/pfrl/utils/mode_of_distribution.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/pretrained_models.py` & `pfrl-0.4.0/pfrl/utils/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/random.py` & `pfrl-0.4.0/pfrl/utils/random.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/random_seed.py` & `pfrl-0.4.0/pfrl/utils/random_seed.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/utils/recurrent.py` & `pfrl-0.4.0/pfrl/utils/recurrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,21 @@
             raise ValueError("Invalid recurrent state: {}".format(non_none_s))
 
 
 def pack_one_step_batch_as_sequences(xs):
     if isinstance(xs, tuple):
         return tuple(pack_one_step_batch_as_sequences(x) for x in xs)
     else:
-        return nn.utils.rnn.pack_sequence(xs[:, None])
+        assert isinstance(xs, torch.Tensor)
+        # xs: (B, ...)-shaped tensor
+        # seqs: B-sized list of (1, ...)-shaped tensors
+        seqs = [x for x in xs.split(1)]
+        assert len(xs) == len(seqs)
+        assert (1,) + xs.shape[1:] == seqs[0].shape
+        return nn.utils.rnn.pack_sequence(seqs)
 
 
 def unpack_sequences_as_one_step_batch(pack):
     if isinstance(pack, nn.utils.rnn.PackedSequence):
         return pack.data
     elif isinstance(pack, tuple):
         return tuple(unpack_sequences_as_one_step_batch(x) for x in pack)
```

### Comparing `pfrl-0.3.0/pfrl/utils/reward_filter.py` & `pfrl-0.4.0/pfrl/utils/reward_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
         self.average_reward_squared = 0
         self.eps = eps
 
     def __call__(self, reward):
         self.average_reward *= 1 - self.tau
         self.average_reward += self.tau * reward
         self.average_reward_squared *= 1 - self.tau
-        self.average_reward_squared += self.tau * reward ** 2
-        var = self.average_reward_squared - self.average_reward ** 2
+        self.average_reward_squared += self.tau * reward**2
+        var = self.average_reward_squared - self.average_reward**2
         stdev = min(var, self.eps) ** 0.5
         return self.scale * (reward - self.average_reward) / stdev
 
 
 class AverageRewardFilter(object):
     def __init__(self, tau=1e-3):
         self.tau = tau
```

### Comparing `pfrl-0.3.0/pfrl/utils/stoppable_thread.py` & `pfrl-0.4.0/pfrl/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/__init__.py` & `pfrl-0.4.0/pfrl/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/atari_wrappers.py` & `pfrl-0.4.0/pfrl/wrappers/atari_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from collections import deque
 
 import gym
 import numpy as np
 from gym import spaces
+from packaging import version
 
 import pfrl
 
 try:
     import cv2
 
     cv2.ocl.setUseOpenCL(False)
@@ -33,17 +34,18 @@
 
     def reset(self, **kwargs):
         """Do no-op action for a number of steps in [1, noop_max]."""
         self.env.reset(**kwargs)
         if self.override_num_noops is not None:
             noops = self.override_num_noops
         else:
-            noops = self.unwrapped.np_random.randint(
-                1, self.noop_max + 1
-            )  # pylint: disable=E1101
+            if version.parse(gym.__version__) >= version.parse("0.24.0"):
+                noops = self.unwrapped.np_random.integers(1, self.noop_max + 1)
+            else:
+                noops = self.unwrapped.np_random.randint(1, self.noop_max + 1)
         assert noops > 0
         obs = None
         for _ in range(noops):
             obs, _, done, info = self.env.step(self.noop_action)
             if done or info.get("needs_reset", False):
                 obs = self.env.reset(**kwargs)
         return obs
```

### Comparing `pfrl-0.3.0/pfrl/wrappers/cast_observation.py` & `pfrl-0.4.0/pfrl/wrappers/cast_observation.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/continuing_time_limit.py` & `pfrl-0.4.0/pfrl/wrappers/continuing_time_limit.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/monitor.py` & `pfrl-0.4.0/pfrl/wrappers/monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 import time
 from logging import getLogger
 
-from gym.wrappers import Monitor as _GymMonitor
-from gym.wrappers.monitoring.stats_recorder import StatsRecorder as _GymStatsRecorder
+try:
+    from gym.wrappers import Monitor as _GymMonitor
+except ImportError:
+
+    class _Stub:
+        def __init__(self, *args, **kwargs):
+            raise RuntimeError("Monitor is not available in this version of gym")
+
+    class _GymMonitor(_Stub):  # type: ignore
+        pass
+
+    class _GymStatsRecorder(_Stub):
+        pass
+
+else:
+    from gym.wrappers.monitoring.stats_recorder import StatsRecorder as _GymStatsRecorder  # type: ignore  # isort: skip  # noqa: E501
 
 
 class Monitor(_GymMonitor):
     """`Monitor` with PFRL's `ContinuingTimeLimit` support.
 
     `Agent` in PFRL might reset the env even when `done=False`
     if `ContinuingTimeLimit` returns `info['needs_reset']=True`,
```

### Comparing `pfrl-0.3.0/pfrl/wrappers/normalize_action_space.py` & `pfrl-0.4.0/pfrl/wrappers/normalize_action_space.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/randomize_action.py` & `pfrl-0.4.0/pfrl/wrappers/randomize_action.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/render.py` & `pfrl-0.4.0/pfrl/wrappers/render.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl/wrappers/vector_frame_stack.py` & `pfrl-0.4.0/pfrl/wrappers/vector_frame_stack.py`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/pfrl.egg-info/PKG-INFO` & `pfrl-0.4.0/pfrl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,137 @@
 Metadata-Version: 2.1
 Name: pfrl
-Version: 0.3.0
+Version: 0.4.0
 Summary: PFRL, a deep reinforcement learning library
-Home-page: UNKNOWN
 Author: Yasuhiro Fujita
 Author-email: fujita@preferred.jp
 License: MIT License
-Description: <div align="center"><img src="https://raw.githubusercontent.com/pfnet/pfrl/master/assets/PFRL.png" height=150/></div>
-        
-        # PFRL
-        [![Documentation Status](https://readthedocs.org/projects/pfrl/badge/?version=latest)](http://pfrl.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/pfrl.svg)](https://pypi.python.org/pypi/pfrl)
-        
-        PFRL is a deep reinforcement learning library that implements various state-of-the-art deep reinforcement algorithms in Python using [PyTorch](https://github.com/pytorch/pytorch).
-        
-        ![Boxing](assets/boxing.gif)
-        ![Humanoid](assets/humanoid.gif)
-        ![Grasping](assets/grasping.gif)
-        ![Atlas](examples/atlas/assets/atlas.gif)
-        ![SlimeVolley](examples/slimevolley/assets/slimevolley.gif)
-        
-        ## Installation
-        
-        PFRL is tested with Python 3.7.7. For other requirements, see [requirements.txt](requirements.txt).
-        
-        PFRL can be installed via PyPI:
-        ```
-        pip install pfrl
-        ```
-        
-        It can also be installed from the source code:
-        ```
-        python setup.py install
-        ```
-        
-        Refer to [Installation](http://pfrl.readthedocs.io/en/latest/install.html) for more information on installation. 
-        
-        ## Getting started
-        
-        You can try [PFRL Quickstart Guide](examples/quickstart/quickstart.ipynb) first, or check the [examples](examples) ready for Atari 2600 and Open AI Gym.
-        
-        For more information, you can refer to [PFRL's documentation](http://pfrl.readthedocs.io/en/latest/index.html).
-        
-        ### Blog Posts
-        - [Introducing PFRL: A PyTorch-based Deep RL Library](https://t.co/VaT06nejSC?amp=1)
-        - [PFRL’s Pretrained Model Zoo](https://bit.ly/3fNx5xH)
-        
-        ## Algorithms
-        
-        | Algorithm | Discrete Action | Continous Action | Recurrent Model | Batch Training | CPU Async Training | Pretrained models<sup>*</sup> |
-        |:----------|:---------------:|:----------------:|:---------------:|:--------------:|:------------------:|:------------------:|
-        | DQN (including DoubleDQN etc.) | ✓ | ✓ (NAF) | ✓ | ✓ | x | ✓ |
-        | Categorical DQN | ✓ | x | ✓ | ✓ | x | x |
-        | Rainbow | ✓ | x | ✓ | ✓ | x | ✓ |
-        | IQN | ✓ | x | ✓ | ✓ | x | ✓ |
-        | DDPG | x | ✓ | x | ✓ | x | ✓ |
-        | A3C  | ✓ | ✓ | ✓ | ✓ (A2C) | ✓ | ✓ |
-        | ACER | ✓ | ✓ | ✓ | x | ✓ | x |
-        | PPO  | ✓ | ✓ | ✓ | ✓ | x | ✓ |
-        | TRPO | ✓ | ✓ | ✓ | ✓ | x | ✓ |
-        | TD3 | x | ✓ | x | ✓ | x | ✓ |
-        | SAC | x | ✓ | x | ✓ | x | ✓ |
-        
-        **<sup>*</sup>Note on Pretrained models**: PFRL provides pretrained models (sometimes called a 'model zoo') for our reproducibility scripts on [Atari environments](https://github.com/pfnet/pfrl/tree/master/examples/atari/reproduction) (DQN, IQN, Rainbow, and A3C) and [Mujoco environments](https://github.com/pfnet/pfrl/tree/master/examples/mujoco/reproduction) (DDPG, TRPO, PPO, TD3, SAC), for each benchmarked environment. 
-        
-        Following algorithms have been implemented in PFRL:
-        - [A2C (Synchronous variant of A3C)](https://openai.com/blog/baselines-acktr-a2c/)
-          - examples: [[atari (batched)]](examples/atari/train_a2c_ale.py)
-        - [A3C (Asynchronous Advantage Actor-Critic)](https://arxiv.org/abs/1602.01783)
-          - examples: [[atari reproduction]](examples/atari/reproduction/a3c) [[atari]](examples/atari/train_a3c_ale.py)
-        - [ACER (Actor-Critic with Experience Replay)](https://arxiv.org/abs/1611.01224)
-          - examples: [[atari]](examples/atari/train_acer_ale.py)
-        - [Categorical DQN](https://arxiv.org/abs/1707.06887)
-          - examples: [[atari]](examples/atari/train_categorical_dqn_ale.py) [[general gym]](examples/gym/train_categorical_dqn_gym.py)
-        - [DQN (Deep Q-Network)](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf) (including [Double DQN](https://arxiv.org/abs/1509.06461), [Persistent Advantage Learning (PAL)](https://arxiv.org/abs/1512.04860), Double PAL, [Dynamic Policy Programming (DPP)](http://www.jmlr.org/papers/volume13/azar12a/azar12a.pdf))
-          - examples: [[atari reproduction]](examples/atari/reproduction/dqn) [[atari]](examples/atari/train_dqn_ale.py) [[atari (batched)]](examples/atari/train_dqn_batch_ale.py) [[flickering atari]](examples/atari/train_drqn_ale.py) [[general gym]](examples/gym/train_dqn_gym.py)
-        - [DDPG (Deep Deterministic Policy Gradients)](https://arxiv.org/abs/1509.02971) (including [SVG(0)](https://arxiv.org/abs/1510.09142))
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ddpg)
-        - [IQN (Implicit Quantile Networks)](https://arxiv.org/abs/1806.06923)
-          - examples: [[atari reproduction]](examples/atari/reproduction/iqn)
-        - [PPO (Proximal Policy Optimization)](https://arxiv.org/abs/1707.06347)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ppo) [[atari]](examples/atari/train_ppo_ale.py)
-        - [Rainbow](https://arxiv.org/abs/1710.02298)
-          - examples: [[atari reproduction]](examples/atari/reproduction/rainbow) [[Slime volleyball]](examples/slimevolley/)
-        - [REINFORCE](http://www-anw.cs.umass.edu/~barto/courses/cs687/williams92simple.pdf)
-          - examples: [[general gym]](examples/gym/train_reinforce_gym.py)
-        - [SAC (Soft Actor-Critic)](https://arxiv.org/abs/1812.05905)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/soft_actor_critic) [[Atlas walk]](examples/atlas/)
-        - [TRPO (Trust Region Policy Optimization)](https://arxiv.org/abs/1502.05477) with [GAE (Generalized Advantage Estimation)](https://arxiv.org/abs/1506.02438)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/trpo)
-        - [TD3 (Twin Delayed Deep Deterministic policy gradient algorithm)](https://arxiv.org/abs/1802.09477)
-          - examples: [[mujoco reproduction]](examples/mujoco/reproduction/td3)
-        
-        Following useful techniques have been also implemented in PFRL:
-        - [NoisyNet](https://arxiv.org/abs/1706.10295)
-          - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
-        - [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952)
-          - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
-        - [Dueling Network](https://arxiv.org/abs/1511.06581)
-          - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
-        - [Normalized Advantage Function](https://arxiv.org/abs/1603.00748)
-          - examples: [[DQN]](examples/gym/train_dqn_gym.py) (for continuous-action envs only)
-        - [Deep Recurrent Q-Network](https://arxiv.org/abs/1507.06527)
-          - examples: [[DQN]](examples/atari/train_drqn_ale.py)
-        
-        
-        ## Environments
-        
-        Environments that support the subset of OpenAI Gym's interface (`reset` and `step` methods) can be used.
-        
-        ## Contributing
-        
-        Any kind of contribution to PFRL would be highly appreciated! If you are interested in contributing to PFRL, please read [CONTRIBUTING.md](CONTRIBUTING.md).
-        
-        ## License
-        
-        [MIT License](LICENSE).
-        
-        ## Citations
-        
-        To cite PFRL in publications, please cite our [paper](https://www.jmlr.org/papers/v22/20-376.html) on ChainerRL, the library on which PFRL is based:
-        
-        ```
-        @article{JMLR:v22:20-376,
-          author  = {Yasuhiro Fujita and Prabhat Nagarajan and Toshiki Kataoka and Takahiro Ishikawa},
-          title   = {ChainerRL: A Deep Reinforcement Learning Library},
-          journal = {Journal of Machine Learning Research},
-          year    = {2021},
-          volume  = {22},
-          number  = {77},
-          pages   = {1-14},
-          url     = {http://jmlr.org/papers/v22/20-376.html}
-        }
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center"><img src="https://raw.githubusercontent.com/pfnet/pfrl/master/assets/PFRL.png" height=150/></div>
+
+# PFRL
+[![Documentation Status](https://readthedocs.org/projects/pfrl/badge/?version=latest)](http://pfrl.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/pfrl.svg)](https://pypi.python.org/pypi/pfrl)
+
+PFRL is a deep reinforcement learning library that implements various state-of-the-art deep reinforcement algorithms in Python using [PyTorch](https://github.com/pytorch/pytorch).
+
+![Boxing](assets/boxing.gif)
+![Humanoid](assets/humanoid.gif)
+![Grasping](assets/grasping.gif)
+![Atlas](examples/atlas/assets/atlas.gif)
+![SlimeVolley](examples/slimevolley/assets/slimevolley.gif)
+
+## Installation
+
+PFRL is tested with Python 3.7.7. For other requirements, see [requirements.txt](requirements.txt).
+
+PFRL can be installed via PyPI:
+```
+pip install pfrl
+```
+
+It can also be installed from the source code:
+```
+python setup.py install
+```
+
+Refer to [Installation](http://pfrl.readthedocs.io/en/latest/install.html) for more information on installation. 
+
+## Getting started
+
+You can try [PFRL Quickstart Guide](examples/quickstart/quickstart.ipynb) first, or check the [examples](examples) ready for Atari 2600 and Open AI Gym.
+
+For more information, you can refer to [PFRL's documentation](http://pfrl.readthedocs.io/en/latest/index.html).
+
+### Blog Posts
+- [Introducing PFRL: A PyTorch-based Deep RL Library](https://t.co/VaT06nejSC?amp=1)
+- [PFRL’s Pretrained Model Zoo](https://bit.ly/3fNx5xH)
+
+## Algorithms
+
+| Algorithm | Discrete Action | Continous Action | Recurrent Model | Batch Training | CPU Async Training | Pretrained models<sup>*</sup> |
+|:----------|:---------------:|:----------------:|:---------------:|:--------------:|:------------------:|:------------------:|
+| DQN (including DoubleDQN etc.) | ✓ | ✓ (NAF) | ✓ | ✓ | x | ✓ |
+| Categorical DQN | ✓ | x | ✓ | ✓ | x | x |
+| Rainbow | ✓ | x | ✓ | ✓ | x | ✓ |
+| IQN | ✓ | x | ✓ | ✓ | x | ✓ |
+| DDPG | x | ✓ | x | ✓ | x | ✓ |
+| A3C  | ✓ | ✓ | ✓ | ✓ (A2C) | ✓ | ✓ |
+| ACER | ✓ | ✓ | ✓ | x | ✓ | x |
+| PPO  | ✓ | ✓ | ✓ | ✓ | x | ✓ |
+| TRPO | ✓ | ✓ | ✓ | ✓ | x | ✓ |
+| TD3 | x | ✓ | x | ✓ | x | ✓ |
+| SAC | x | ✓ | x | ✓ | x | ✓ |
+
+**<sup>*</sup>Note on Pretrained models**: PFRL provides pretrained models (sometimes called a 'model zoo') for our reproducibility scripts on [Atari environments](https://github.com/pfnet/pfrl/tree/master/examples/atari/reproduction) (DQN, IQN, Rainbow, and A3C) and [Mujoco environments](https://github.com/pfnet/pfrl/tree/master/examples/mujoco/reproduction) (DDPG, TRPO, PPO, TD3, SAC), for each benchmarked environment. 
+
+Following algorithms have been implemented in PFRL:
+- [A2C (Synchronous variant of A3C)](https://openai.com/blog/baselines-acktr-a2c/)
+  - examples: [[atari (batched)]](examples/atari/train_a2c_ale.py)
+- [A3C (Asynchronous Advantage Actor-Critic)](https://arxiv.org/abs/1602.01783)
+  - examples: [[atari reproduction]](examples/atari/reproduction/a3c) [[atari]](examples/atari/train_a3c_ale.py)
+- [ACER (Actor-Critic with Experience Replay)](https://arxiv.org/abs/1611.01224)
+  - examples: [[atari]](examples/atari/train_acer_ale.py)
+- [Categorical DQN](https://arxiv.org/abs/1707.06887)
+  - examples: [[atari]](examples/atari/train_categorical_dqn_ale.py) [[general gym]](examples/gym/train_categorical_dqn_gym.py)
+- [DQN (Deep Q-Network)](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf) (including [Double DQN](https://arxiv.org/abs/1509.06461), [Persistent Advantage Learning (PAL)](https://arxiv.org/abs/1512.04860), Double PAL, [Dynamic Policy Programming (DPP)](http://www.jmlr.org/papers/volume13/azar12a/azar12a.pdf))
+  - examples: [[atari reproduction]](examples/atari/reproduction/dqn) [[atari]](examples/atari/train_dqn_ale.py) [[atari (batched)]](examples/atari/train_dqn_batch_ale.py) [[flickering atari]](examples/atari/train_drqn_ale.py) [[general gym]](examples/gym/train_dqn_gym.py)
+- [DDPG (Deep Deterministic Policy Gradients)](https://arxiv.org/abs/1509.02971) (including [SVG(0)](https://arxiv.org/abs/1510.09142))
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ddpg)
+- [IQN (Implicit Quantile Networks)](https://arxiv.org/abs/1806.06923)
+  - examples: [[atari reproduction]](examples/atari/reproduction/iqn)
+- [PPO (Proximal Policy Optimization)](https://arxiv.org/abs/1707.06347)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/ppo) [[atari]](examples/atari/train_ppo_ale.py)
+- [Rainbow](https://arxiv.org/abs/1710.02298)
+  - examples: [[atari reproduction]](examples/atari/reproduction/rainbow) [[Slime volleyball]](examples/slimevolley/)
+- [REINFORCE](http://www-anw.cs.umass.edu/~barto/courses/cs687/williams92simple.pdf)
+  - examples: [[general gym]](examples/gym/train_reinforce_gym.py)
+- [SAC (Soft Actor-Critic)](https://arxiv.org/abs/1812.05905)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/soft_actor_critic) [[Atlas walk]](examples/atlas/)
+- [TRPO (Trust Region Policy Optimization)](https://arxiv.org/abs/1502.05477) with [GAE (Generalized Advantage Estimation)](https://arxiv.org/abs/1506.02438)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/trpo)
+- [TD3 (Twin Delayed Deep Deterministic policy gradient algorithm)](https://arxiv.org/abs/1802.09477)
+  - examples: [[mujoco reproduction]](examples/mujoco/reproduction/td3)
+
+Following useful techniques have been also implemented in PFRL:
+- [NoisyNet](https://arxiv.org/abs/1706.10295)
+  - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
+- [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952)
+  - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
+- [Dueling Network](https://arxiv.org/abs/1511.06581)
+  - examples: [[Rainbow]](examples/atari/reproduction/rainbow) [[DQN/DoubleDQN/PAL]](examples/atari/train_dqn_ale.py)
+- [Normalized Advantage Function](https://arxiv.org/abs/1603.00748)
+  - examples: [[DQN]](examples/gym/train_dqn_gym.py) (for continuous-action envs only)
+- [Deep Recurrent Q-Network](https://arxiv.org/abs/1507.06527)
+  - examples: [[DQN]](examples/atari/train_drqn_ale.py)
+
+
+## Environments
+
+Environments that support the subset of OpenAI Gym's interface (`reset` and `step` methods) can be used.
+
+## Contributing
+
+Any kind of contribution to PFRL would be highly appreciated! If you are interested in contributing to PFRL, please read [CONTRIBUTING.md](CONTRIBUTING.md).
+
+## License
+
+[MIT License](LICENSE).
+
+## Citations
+
+To cite PFRL in publications, please cite our [paper](https://www.jmlr.org/papers/v22/20-376.html) on ChainerRL, the library on which PFRL is based:
+
+```
+@article{JMLR:v22:20-376,
+  author  = {Yasuhiro Fujita and Prabhat Nagarajan and Toshiki Kataoka and Takahiro Ishikawa},
+  title   = {ChainerRL: A Deep Reinforcement Learning Library},
+  journal = {Journal of Machine Learning Research},
+  year    = {2021},
+  volume  = {22},
+  number  = {77},
+  pages   = {1-14},
+  url     = {http://jmlr.org/papers/v22/20-376.html}
+}
+```
```

### Comparing `pfrl-0.3.0/pfrl.egg-info/SOURCES.txt` & `pfrl-0.4.0/pfrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/setup.cfg` & `pfrl-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pfrl-0.3.0/setup.py` & `pfrl-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 test_requires = [
     'pytest',
     'attrs<19.2.0',  # pytest does not run with attrs==19.2.0 (https://github.com/pytest-dev/pytest/issues/3280)  # NOQA
 ]
 
 setup(name='pfrl',
-      version='0.3.0',
+      version='0.4.0',
       description='PFRL, a deep reinforcement learning library',
       long_description=codecs.open('README.md', 'r', encoding='utf-8').read(),
       long_description_content_type='text/markdown',
       author='Yasuhiro Fujita',
       author_email='fujita@preferred.jp',
       license='MIT License',
       packages=find_packages(),
```


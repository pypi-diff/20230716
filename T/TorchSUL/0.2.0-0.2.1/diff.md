# Comparing `tmp/TorchSUL-0.2.0.tar.gz` & `tmp/TorchSUL-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSUL-0.2.0.tar", last modified: Sat Jul 15 09:50:20 2023, max compression
+gzip compressed data, was "TorchSUL-0.2.1.tar", last modified: Sun Jul 16 13:17:58 2023, max compression
```

## Comparing `TorchSUL-0.2.0.tar` & `TorchSUL-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-15 09:50:20.830544 TorchSUL-0.2.0/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3860 2023-07-15 09:50:20.828544 TorchSUL-0.2.0/PKG-INFO
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3621 2023-07-15 09:49:09.000000 TorchSUL-0.2.0/README.md
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-15 09:50:20.764228 TorchSUL-0.2.0/TorchSUL/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3859 2023-07-15 09:32:31.000000 TorchSUL-0.2.0/TorchSUL/Base.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      932 2023-07-15 09:38:57.000000 TorchSUL-0.2.0/TorchSUL/Config.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    22395 2023-07-15 08:51:32.000000 TorchSUL-0.2.0/TorchSUL/Layers.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    15107 2023-07-15 08:43:11.000000 TorchSUL-0.2.0/TorchSUL/Model.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13206 2023-07-07 15:01:14.000000 TorchSUL-0.2.0/TorchSUL/Quant.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.0/TorchSUL/__init__.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-15 08:15:48.000000 TorchSUL-0.2.0/TorchSUL/sul_tool.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-15 07:41:07.000000 TorchSUL-0.2.0/TorchSUL/sulplotter.py
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-15 09:50:20.816434 TorchSUL-0.2.0/TorchSUL.egg-info/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3860 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/PKG-INFO
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/SOURCES.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/dependency_links.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/requires.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-07-15 09:50:20.000000 TorchSUL-0.2.0/TorchSUL.egg-info/top_level.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-07-15 09:50:20.830544 TorchSUL-0.2.0/setup.cfg
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-07-15 08:14:28.000000 TorchSUL-0.2.0/setup.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-16 13:17:58.491801 TorchSUL-0.2.1/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4038 2023-07-16 13:17:58.489799 TorchSUL-0.2.1/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3865 2023-07-16 13:16:20.000000 TorchSUL-0.2.1/README.md
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-16 13:17:58.433885 TorchSUL-0.2.1/TorchSUL/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3920 2023-07-16 13:10:08.000000 TorchSUL-0.2.1/TorchSUL/Base.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      932 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Config.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    22926 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Layers.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    15107 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Model.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13358 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Quant.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.1/TorchSUL/__init__.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/sul_tool.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/sulplotter.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-16 13:17:58.477697 TorchSUL-0.2.1/TorchSUL.egg-info/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4038 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/requires.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/top_level.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-07-16 13:17:58.491801 TorchSUL-0.2.1/setup.cfg
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-07-16 13:12:17.000000 TorchSUL-0.2.1/setup.py
```

### Comparing `TorchSUL-0.2.0/PKG-INFO` & `TorchSUL-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchSUL
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple but useful layers for Pytorch
 Home-page: https://github.com/ddddwee1/TorchSUL
 Author: Cheng Yu
 Author-email: chengyu996@gmail.com
 Description-Content-Type: text/markdown
 
 # TorchSUL
@@ -29,22 +29,28 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
-------
-2023-07-15:  Upgrade to 0.2.0. 
+#### 2023-07-16:  Bugfixes 
+1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
+2. Add quantization support for fc layers. 
+
+
+#### 2023-07-15:  Upgrade to 0.2.0. 
 1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
 2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
 3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
 4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples. 
 
 
+
+
 ## Projects 
 
 You can find some examples in the "example" folder.
 
 - ArcFace (Deng, Jiankang, et al. "Arcface: Additive angular margin loss for deep face recognition." arXiv preprint arXiv:1801.07698 (2018))
 
 - HR Net (Sun, Ke, et al. "Deep High-Resolution Representation Learning for Human Pose Estimation." arXiv preprint arXiv:1902.09212 (2019))
```

### Comparing `TorchSUL-0.2.0/README.md` & `TorchSUL-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,66 @@
-# TorchSUL
-
-This package is created for better experience while using Pytorch. 
-
-## Why making this
-
-1. For fun.
-
-2. Path-dependence. I am addicted to my own wrap-ups. 
-
-3. Multi-platform. I have made the same APIs for pytorch, TF, MXNet, and a conversion tool to Caffe. 
-
-4. Some strange reason. Frameworks like TF, MXNet, Caffe, Paddle do not need to claim input shape to initialize layers, but frameworks like pytorch, torch, chainer require this. I prefer not to claim since it will be more convenient when building models (Why I need to care about previous layers when I only want to write forward computation?), so I modified pytorch module to support this. Also, it inlines with my [TF wrap-ups](https://github.com/ddddwee1/sul) so I can move my old code easily to the current package.
-
-## Installation
-
-You need to install the latest version of pytorch.
-
-Good, then just 
-
-```
-pip install --upgrade torchsul
-```
-
-## Patch Notes
-
-------
-2023-07-15:  Upgrade to 0.2.0. 
-1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
-2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
-3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
-4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples. 
-
-
-## Projects 
-
-You can find some examples in the "example" folder.
-
-- ArcFace (Deng, Jiankang, et al. "Arcface: Additive angular margin loss for deep face recognition." arXiv preprint arXiv:1801.07698 (2018))
-
-- HR Net (Sun, Ke, et al. "Deep High-Resolution Representation Learning for Human Pose Estimation." arXiv preprint arXiv:1902.09212 (2019))
-
-- AutoDeepLab (Liu, Chenxi, et al. "Auto-deeplab: Hierarchical neural architecture search for semantic image segmentation." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2019)
-
-- Knowledge distillation (Hinton, Geoffrey, Oriol Vinyals, and Jeff Dean. "Distilling the knowledge in a neural network." arXiv preprint arXiv:1503.02531 (2015))
-
-- 3DCNN (Ji, Shuiwang, et al. "3D convolutional neural networks for human action recognition." IEEE transactions on pattern analysis and machine intelligence 35.1 (2012): 221-231)
-
-- Temporal Convolutional Network (Not the same) (Pavllo, Dario, et al. "3D human pose estimation in video with temporal convolutions and semi-supervised training." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2019)
-
-- RetinaFace for face detection (Deng, Jiankang, et al. "Retinaface: Single-stage dense face localisation in the wild." arXiv preprint arXiv:1905.00641 (2019))
-
-- Fractal Net (Larsson, Gustav, Michael Maire, and Gregory Shakhnarovich. "Fractalnet: Ultra-deep neural networks without residuals." arXiv preprint arXiv:1605.07648 (2016))
-
-- Polarized Self Attention (Liu, Huajun, et al. "Polarized self-attention: Towards high-quality pixel-wise regression." arXiv preprint arXiv:2107.00782 (2021))
-
-- Model conversions 
-
-- Batch_norm compression to speed-up models 
-
+# TorchSUL
+
+This package is created for better experience while using Pytorch. 
+
+## Why making this
+
+1. For fun.
+
+2. Path-dependence. I am addicted to my own wrap-ups. 
+
+3. Multi-platform. I have made the same APIs for pytorch, TF, MXNet, and a conversion tool to Caffe. 
+
+4. Some strange reason. Frameworks like TF, MXNet, Caffe, Paddle do not need to claim input shape to initialize layers, but frameworks like pytorch, torch, chainer require this. I prefer not to claim since it will be more convenient when building models (Why I need to care about previous layers when I only want to write forward computation?), so I modified pytorch module to support this. Also, it inlines with my [TF wrap-ups](https://github.com/ddddwee1/sul) so I can move my old code easily to the current package.
+
+## Installation
+
+You need to install the latest version of pytorch.
+
+Good, then just 
+
+```
+pip install --upgrade torchsul
+```
+
+## Patch Notes
+
+#### 2023-07-16:  Bugfixes 
+1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
+2. Add quantization support for fc layers. 
+
+
+#### 2023-07-15:  Upgrade to 0.2.0. 
+1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
+2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
+3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
+4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples. 
+
+
+
+
+## Projects 
+
+You can find some examples in the "example" folder.
+
+- ArcFace (Deng, Jiankang, et al. "Arcface: Additive angular margin loss for deep face recognition." arXiv preprint arXiv:1801.07698 (2018))
+
+- HR Net (Sun, Ke, et al. "Deep High-Resolution Representation Learning for Human Pose Estimation." arXiv preprint arXiv:1902.09212 (2019))
+
+- AutoDeepLab (Liu, Chenxi, et al. "Auto-deeplab: Hierarchical neural architecture search for semantic image segmentation." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2019)
+
+- Knowledge distillation (Hinton, Geoffrey, Oriol Vinyals, and Jeff Dean. "Distilling the knowledge in a neural network." arXiv preprint arXiv:1503.02531 (2015))
+
+- 3DCNN (Ji, Shuiwang, et al. "3D convolutional neural networks for human action recognition." IEEE transactions on pattern analysis and machine intelligence 35.1 (2012): 221-231)
+
+- Temporal Convolutional Network (Not the same) (Pavllo, Dario, et al. "3D human pose estimation in video with temporal convolutions and semi-supervised training." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2019)
+
+- RetinaFace for face detection (Deng, Jiankang, et al. "Retinaface: Single-stage dense face localisation in the wild." arXiv preprint arXiv:1905.00641 (2019))
+
+- Fractal Net (Larsson, Gustav, Michael Maire, and Gregory Shakhnarovich. "Fractalnet: Ultra-deep neural networks without residuals." arXiv preprint arXiv:1605.07648 (2016))
+
+- Polarized Self Attention (Liu, Huajun, et al. "Polarized self-attention: Towards high-quality pixel-wise regression." arXiv preprint arXiv:2107.00782 (2021))
+
+- Model conversions 
+
+- Batch_norm compression to speed-up models 
+
```

### Comparing `TorchSUL-0.2.0/TorchSUL/Base.py` & `TorchSUL-0.2.1/TorchSUL/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 			self.set_flag(k, self._model_flags[k])
 		self.setup_cfg()
 			
 	def build(self, *inputs, **kwargs):
 		pass
 
 	def build_forward(self, *inputs, **kwargs):
+		# build_forward is used to do value intializations etc.
 		return self.forward(*inputs, **kwargs)
 
 	def __call__(self, *input, **kwargs):
 		if not self._is_built:
 			self.build(*input)
 			self._set_status()
 		for hook in self._forward_pre_hooks.values():
@@ -121,13 +122,13 @@
 
 	def save_tensor(self, out, name):
 		if self.get_flag('save_tensor'):
 			os.makedirs('./layer_dumps/', exist_ok=True)
 			torch.save(out, './layer_dumps/%s.pth'%name.replace('/','_'))
 
 	def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs):
-		super()._load_from_state_dict(state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs)
 		self._load_from_state_dict2(state_dict, prefix)
-
+		super()._load_from_state_dict(state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs)
+		
 	def _load_from_state_dict2(self, state_dict, prefix):
 		# Conveinient method. Omit infrequent arguments
 		pass
```

### Comparing `TorchSUL-0.2.0/TorchSUL/Config.py` & `TorchSUL-0.2.1/TorchSUL/Config.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.0/TorchSUL/Layers.py` & `TorchSUL-0.2.1/TorchSUL/Layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,28 +307,43 @@
 		self.weight = Parameter(torch.Tensor(self.outsize, self.insize))
 		if self.usebias:
 			self.bias = Parameter(torch.Tensor(self.outsize))
 		else:
 			self.register_parameter('bias', None)
 		self.reset_params()
 
+		if self._quant:
+			bit_type = self.get_flag('QActBit')
+			if bit_type is None:
+				bit_type = 'int8'
+			obs_type = self.get_flag('QActObserver')
+			if obs_type is None:
+				obs_type = 'minmax'
+			self.input_quantizer = QQuantizers['uniform'](zero_offset=False, bit_type=bit_type, observer=obs_type)
+			self.w_quantizer = QQuantizers['uniform'](zero_offset=True, mode='channel_wise', is_weight=True)
+
+
 	def reset_params(self):
 		init.normal_(self.weight, std=0.001)
 		if self.bias is not None:
 			init.zeros_(self.bias)
 
 	def forward(self, x):
 		if self.norm:
 			with torch.no_grad():
 				norm = x.norm(p=2, dim=1, keepdim=True)
 				wnorm = self.weight.norm(p=2,dim=1, keepdim=True)
 			x = x / norm
 			weight = self.weight / wnorm
 		else:
 			weight = self.weight
+
+		if self._quant:
+			x = self.input_quantizer(x).contiguous()
+			weight = self.w_quantizer(weight).contiguous()
 		return F.linear(x, weight, self.bias)
 
 	def to_torch(self):
 		fc = nn.Linear(self.insize, self.outsize, self.usebias)
 		fc.weight.data[:] = self.weight.data[:]
 		if self.usebias:
 			fc.bias.data[:] = self.bias.data[:]
```

### Comparing `TorchSUL-0.2.0/TorchSUL/Model.py` & `TorchSUL-0.2.1/TorchSUL/Model.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.0/TorchSUL/Quant.py` & `TorchSUL-0.2.1/TorchSUL/Quant.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 		if dim!=-1 and mode=='channel_wise':
 			x = x.transpose(-1, dim)
 		return x
 
 	@staticmethod
 	@once_differentiable
 	def backward(ctx, out_grad):
+		out_grad = out_grad.contiguous()
 		x, x1, scale, zero_point = ctx.saved_tensors
 
 		# compute ds 
 		ds = x1.clone()
 		ds -= zero_point
 		idx = (x1>ctx.Qn) & (x1<ctx.Qp)
 		# print(idx.shape, scale.shape, ds[idx].shape, x.shape)
@@ -71,15 +72,15 @@
 			# use mean here 
 			ds = ds.flatten(0,-2).sum(dim=0)
 			db = db.flatten(0,-2).sum(dim=0)
 		else:
 			ds = ds.sum()
 			db = db.sum()
 
-		return dx, ds, db, None, None, None, None, None
+		return dx.contiguous(), ds.contiguous(), db.contiguous(), None, None, None, None, None
 
 	@staticmethod
 	def symbolic(g, x, scale, zero_point, Qn, Qp, zero_offset=False, mode='layer_wise', dim=-1):
 		return g.op('custom_ops::quant', x, scale, zero_point, Qn_i=int(Qn), Qp_i=int(Qp), zero_offset_i=int(zero_offset), mode_s=mode, dim_i=int(dim)).setType(x.type().with_sizes(x.type().sizes()))
 
 
 ##### Quant classes 
@@ -113,21 +114,21 @@
 		self.is_weight = is_weight
 		self.scale = None 
 		self.zero_point = None 
 		self.sigma = 0.01 
 		self.percentile = 0.99999
 
 	def build(self, x):
-		if len(x.shape)==4:
-			# b,c,h,w
-			self.dim = -3
-			if self.is_weight:
-				self.dim = -4
+		if self.is_weight:
+			self.dim = 0
 		else:
-			self.dim = -1
+			if len(x.shape)==4:
+				self.dim = 1 
+			else:
+				self.dim = -1
 
 	def observe(self, x):
 		if self.mode == 'channel_wise':
 			x = x.transpose(0, self.dim)
 			x = x.flatten(1)
 			minv = torch.quantile(x.cuda(), 1-self.percentile, dim=1).cpu()
 			maxv = torch.quantile(x.cuda(), self.percentile, dim=1).cpu()
@@ -186,21 +187,21 @@
 		self.bit_type = bit_type
 		self.zero_offset = zero_offset
 		self.is_weight = is_weight
 		self.scale = None 
 		self.zero_point = None 
 
 	def build(self, x):
-		if len(x.shape)==4:
-			# b,c,h,w
-			self.dim = -3
-			if self.is_weight:
-				self.dim = -4
+		if self.is_weight:
+			self.dim = 0
 		else:
-			self.dim = -1
+			if len(x.shape)==4:
+				self.dim = 1 
+			else:
+				self.dim = -1
 
 	def observe(self, x):
 		if self.mode == 'channel_wise':
 			x = x.transpose(0, self.dim)
 			x = x.flatten(1)
 			minv = x.min(dim=1)[0]
 			maxv = x.max(dim=1)[0]
@@ -259,21 +260,22 @@
 		self.bit_type = bit_type
 		self.zero_offset = zero_offset
 		self.is_weight = is_weight
 		self.scale = None 
 		self.zero_point = None 
 
 	def build(self, x):
-		if len(x.shape)==4:
-			# b,c,h,w
-			self.dim = -3
-			if self.is_weight:
-				self.dim = -4
+		# TODO: mannually fit dim?
+		if self.is_weight:
+			self.dim = 0
 		else:
-			self.dim = -1
+			if len(x.shape)==4:
+				self.dim = 1 
+			else:
+				self.dim = -1
 
 	def observe(self, x):
 		if self.mode == 'channel_wise':
 			x = x.transpose(-1, self.dim)
 			x = x.flatten(0,-2)
 			minv = x.min(dim=0)[0]
 			maxv = x.max(dim=0)[0]
@@ -362,46 +364,47 @@
 		self.bit_type = QTYPES[bit_type]
 		self.observer = QObservers[observer](self.bit_type, zero_offset, mode, is_weight)
 		self.mode = mode 
 		self.is_weight = is_weight
 		self.zero_offset = zero_offset
 
 	def build(self, x):
-		if len(x.shape)==4:
-			if self.is_weight:
-				self.dim = -4
-			else:
-				self.dim = -3
+		if self.is_weight:
+			self.dim = 0
 		else:
-			self.dim = -1 
+			if len(x.shape)==4:
+				self.dim = 1 
+			else:
+				self.dim = -1
 
 	def quant_dequant(self, x):
 		if self.dim!=-1 and self.mode=='channel_wise':
 			# make everything run at last dim, no need manually reshape 
 			x = x.transpose(-1, self.dim)
 		x = x / self.observer.scale + self.observer.zero_point
 		x = x.round().clamp(self.bit_type.min_val, self.bit_type.max_val)
 		x = (x - self.observer.zero_point) * self.observer.scale 
 		if self.dim!=-1 and self.mode=='channel_wise':
 			x = x.transpose(-1, self.dim)
 		return x 
 
 	def forward(self, x):
+		x = x.contiguous()
 		if self._quant_calibrating:
 			x = self.observer(x)
 		if self._quant and self._quant_calibrated:
 			if self.observer.scale.device!=x.device:
 				self.observer.scale = self.observer.scale.to(x.device)
 				self.observer.zero_point = self.observer.zero_point.to(x.device)
 			# x = self.quant_dequant(x)
 			if self.get_flag('dump_onnx'):
 				x = QATFunc.apply(x, self.observer.scale.data, self.observer.zero_point.data, self.bit_type.min_val, self.bit_type.max_val, self.zero_offset, self.mode, self.dim)
 			else:
-				x = QATFunc.apply(x, self.observer.scale, self.observer.zero_point, self.bit_type.min_val, self.bit_type.max_val, self.zero_offset, self.mode, self.dim)
-		return x 
+				x = QATFunc.apply(x, self.observer.scale.contiguous(), self.observer.zero_point.contiguous(), self.bit_type.min_val, self.bit_type.max_val, self.zero_offset, self.mode, self.dim)
+		return x.contiguous() 
 
 
 QQuantizers = {"uniform": UniformQuantizer}
 
 
 class QAct(Model):
 	def initialize(self, zero_offset=False, mode='layer_wise', observer=None, bit_type=None):
```

### Comparing `TorchSUL-0.2.0/TorchSUL/sul_tool.py` & `TorchSUL-0.2.1/TorchSUL/sul_tool.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.0/TorchSUL/sulplotter.py` & `TorchSUL-0.2.1/TorchSUL/sulplotter.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.0/TorchSUL.egg-info/PKG-INFO` & `TorchSUL-0.2.1/TorchSUL.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchSUL
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple but useful layers for Pytorch
 Home-page: https://github.com/ddddwee1/TorchSUL
 Author: Cheng Yu
 Author-email: chengyu996@gmail.com
 Description-Content-Type: text/markdown
 
 # TorchSUL
@@ -29,22 +29,28 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
-------
-2023-07-15:  Upgrade to 0.2.0. 
+#### 2023-07-16:  Bugfixes 
+1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
+2. Add quantization support for fc layers. 
+
+
+#### 2023-07-15:  Upgrade to 0.2.0. 
 1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
 2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
 3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
 4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples. 
 
 
+
+
 ## Projects 
 
 You can find some examples in the "example" folder.
 
 - ArcFace (Deng, Jiankang, et al. "Arcface: Additive angular margin loss for deep face recognition." arXiv preprint arXiv:1801.07698 (2018))
 
 - HR Net (Sun, Ke, et al. "Deep High-Resolution Representation Learning for Human Pose Estimation." arXiv preprint arXiv:1902.09212 (2019))
```

### Comparing `TorchSUL-0.2.0/setup.py` & `TorchSUL-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name='TorchSUL',
-    version='0.2.0',
+    version='0.2.1',
     description='Simple but useful layers for Pytorch',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Cheng Yu',
     author_email='chengyu996@gmail.com',
     url='https://github.com/ddddwee1/TorchSUL',
```


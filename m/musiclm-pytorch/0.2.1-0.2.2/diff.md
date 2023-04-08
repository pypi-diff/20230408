# Comparing `tmp/musiclm-pytorch-0.2.1.tar.gz` & `tmp/musiclm-pytorch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclm-pytorch-0.2.1.tar", last modified: Fri Mar 31 15:15:01 2023, max compression
+gzip compressed data, was "musiclm-pytorch-0.2.2.tar", last modified: Sat Apr  8 16:48:10 2023, max compression
```

## Comparing `musiclm-pytorch-0.2.1.tar` & `musiclm-pytorch-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:15:01.741385 musiclm-pytorch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 15:14:48.000000 musiclm-pytorch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-31 15:15:01.741385 musiclm-pytorch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-03-31 15:14:48.000000 musiclm-pytorch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:15:01.737385 musiclm-pytorch-0.2.1/musiclm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-31 15:14:48.000000 musiclm-pytorch-0.2.1/musiclm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27549 2023-03-31 15:14:48.000000 musiclm-pytorch-0.2.1/musiclm_pytorch/musiclm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-03-31 15:14:48.000000 musiclm-pytorch-0.2.1/musiclm_pytorch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:15:01.741385 musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-31 15:15:01.000000 musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-31 15:15:01.000000 musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 15:15:01.000000 musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-31 15:15:01.000000 musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 15:15:01.000000 musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 15:15:01.741385 musiclm-pytorch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-31 15:14:48.000000 musiclm-pytorch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:48:10.182464 musiclm-pytorch-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-08 16:47:58.000000 musiclm-pytorch-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-08 16:48:10.182464 musiclm-pytorch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-08 16:47:58.000000 musiclm-pytorch-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:48:10.182464 musiclm-pytorch-0.2.2/musiclm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-08 16:47:58.000000 musiclm-pytorch-0.2.2/musiclm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-04-08 16:47:58.000000 musiclm-pytorch-0.2.2/musiclm_pytorch/musiclm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-04-08 16:47:58.000000 musiclm-pytorch-0.2.2/musiclm_pytorch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:48:10.182464 musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-08 16:48:10.000000 musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-08 16:48:10.000000 musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:48:10.000000 musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-08 16:48:10.000000 musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 16:48:10.000000 musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:48:10.182464 musiclm-pytorch-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-08 16:47:58.000000 musiclm-pytorch-0.2.2/setup.py
```

### Comparing `musiclm-pytorch-0.2.1/LICENSE` & `musiclm-pytorch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musiclm-pytorch-0.2.1/PKG-INFO` & `musiclm-pytorch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclm-pytorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: MusicLM - AudioLM + Audio CLIP to text to music synthesis
 Home-page: https://github.com/lucidrains/musiclm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text to music,contrastive learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `musiclm-pytorch-0.2.1/README.md` & `musiclm-pytorch-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `musiclm-pytorch-0.2.1/musiclm_pytorch/musiclm_pytorch.py` & `musiclm-pytorch-0.2.2/musiclm_pytorch/musiclm_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,16 +499,16 @@
         if not return_all_layers:
             return out
 
         return out, all_layers
 
 # text transformer
 
-@beartype
 class TextTransformer(nn.Module):
+    @beartype
     def __init__(
         self,
         dim,
         depth,
         num_tokens = tokenizer.vocab_size,
         max_seq_len = 256,
         dim_head = 64,
@@ -542,14 +542,15 @@
         self.pad_id = pad_id
         self.norm = LayerNorm(dim)
 
     @property
     def device(self):
         return next(self.parameters()).device
 
+    @beartype
     def forward(
         self,
         x = None,
         raw_texts: Optional[List[str]] = None,
         mask = None,
         return_all_layers = False
     ):
@@ -644,16 +645,16 @@
 
         cosine_sims = einsum('l i d, l j d -> l i j', audio_latents, text_latents)
 
         return self.contrast(cosine_sims)
 
 # main classes
 
-@beartype
 class MuLaN(nn.Module):
+    @beartype
     def __init__(
         self,
         audio_transformer: AudioSpectrogramTransformer,
         text_transformer: TextTransformer,
         dim_latent = 128,                       # they use 128
         decoupled_contrastive_learning = True,  # think this was used, make it optional
         hierarchical_contrastive_loss = False,
@@ -701,14 +702,15 @@
         out = l2norm(audio_latents)
 
         if not return_all_layers:
             return out
 
         return out, audio_layers
 
+    @beartype
     def get_text_latents(
         self,
         texts = None,
         raw_texts: Optional[List[str]] = None,
         return_all_layers = False
     ):
         text_embeds, text_layers = self.text(texts, raw_texts = raw_texts, return_all_layers = True)
@@ -716,14 +718,15 @@
         out = l2norm(text_latents)
 
         if not return_all_layers:
             return out
 
         return out, text_layers
 
+    @beartype
     def forward(
         self,
         wavs,
         texts = None,
         raw_texts: Optional[List[str]] = None,
         return_latents = False,
         return_similarities = False,
@@ -762,16 +765,16 @@
             text_layers = text_layers
         )
 
         return cl_loss + hierarchical_cl_loss
 
 # music lm
 
-@beartype
 class MuLaNEmbedQuantizer(AudioConditionerBase):
+    @beartype
     def __init__(
         self,
         mulan: MuLaN,
         conditioning_dims: Tuple[int, ...],
         rq_num_quantizers = 8,
         rq_ema_decay = 0.9,
         codebook_size = 1024,
@@ -847,16 +850,16 @@
 
         cond_embeddings = repeat(cond_embeddings, 'q c d -> b q c d', b = batch)
         indices = repeat(indices, 'b q -> b q 1 d', q = num_codebooks, d = dim)
 
         cond_embeddings = cond_embeddings.gather(2, indices)
         return rearrange(cond_embeddings, 'b q 1 d -> b q d')
 
-@beartype
 class MusicLM(nn.Module):
+    @beartype
     def __init__(
         self,
         audio_lm: AudioLM,
         mulan_embed_quantizer: MuLaNEmbedQuantizer
     ):
         super().__init__()
         assert not exists(audio_lm.audio_conditioner), 'mulan must not have been passed into AudioLM. it will be managed externally now, embedding the text into the joint embedding space for text-to-audio synthesis'
```

### Comparing `musiclm-pytorch-0.2.1/musiclm_pytorch/trainer.py` & `musiclm-pytorch-0.2.2/musiclm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `musiclm-pytorch-0.2.1/musiclm_pytorch.egg-info/PKG-INFO` & `musiclm-pytorch-0.2.2/musiclm_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musiclm-pytorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: MusicLM - AudioLM + Audio CLIP to text to music synthesis
 Home-page: https://github.com/lucidrains/musiclm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text to music,contrastive learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `musiclm-pytorch-0.2.1/setup.py` & `musiclm-pytorch-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'musiclm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',
   description = 'MusicLM - AudioLM + Audio CLIP to text to music synthesis',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/musiclm-pytorch',
   keywords = [
```


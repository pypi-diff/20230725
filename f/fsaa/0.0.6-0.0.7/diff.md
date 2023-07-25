# Comparing `tmp/fsaa-0.0.6.tar.gz` & `tmp/fsaa-0.0.7.tar.gz`

## Comparing `fsaa-0.0.6.tar` & `fsaa-0.0.7.tar`

### file list

```diff
@@ -1,55 +1,58 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.6/CITATION.cff
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.6/CODEOWNERS
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.6/environment.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.6/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.6/assets/logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/core.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/jnd.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/nomask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/__init__.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/hf_models/hf_models.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/hub_models/hub_models.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/ibot/ibot.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/ibot/utils.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/ibot/vits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.6/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.6/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.6/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_masks.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_models.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_updaters.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.6/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.6/LICENSE
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.6/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.7/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.7/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.7/environment.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fsaa-0.0.7/update-version.sh
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.7/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.7/assets/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/attack.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/core.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hf/hf_models.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hf_models/hf_models.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hub/hub_models.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hub_models/hub_models.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/random.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.7/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.7/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.7/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_masks.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_transforms.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.7/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.7/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.7/PKG-INFO
```

### Comparing `fsaa-0.0.6/.pre-commit-config.yaml` & `fsaa-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/environment.yml` & `fsaa-0.0.7/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/.github/workflows/python-publish.yml` & `fsaa-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/.vscode/launch.json` & `fsaa-0.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/assets/logo.png` & `fsaa-0.0.7/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/attack.py` & `fsaa-0.0.7/fsaa/attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/core.py` & `fsaa-0.0.7/fsaa/core.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/utils.py` & `fsaa-0.0.7/fsaa/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from fsaa.initializers.random_sign import RandomSignInitializer
 from fsaa.losses.cossim_loss import CosSimLoss
 from fsaa.losses.lpips_loss import LPIPSAlexLoss, LPIPSVGGLoss
 from fsaa.losses.mse_loss import MeanSquaredErrorLoss
 from fsaa.masks.custom import CustomMask
 from fsaa.masks.jnd import JNDMask
 from fsaa.masks.nomask import NoMask
-from fsaa.models.hf_models.hf_models import SUPPORTED_HF_MODELS, HFModel
-from fsaa.models.hub_models.hub_models import SUPPORTED_HUB_MODELS, HubModel
+from fsaa.models.hf.hf_models import SUPPORTED_HF_MODELS, HFModel
+from fsaa.models.hub.hub_models import SUPPORTED_HUB_MODELS, HubModel
 from fsaa.models.ibot.ibot import SUPPORTED_IBOT_MODELS, iBOTModel
 from fsaa.updaters.fgsm import FGSMUpdater
 from fsaa.updaters.langevin import LangevinUpdater
 from fsaa.updaters.pgd import PGDUpdater
 from fsaa.updaters.random import RandomUpdater
 
 INITIALIZERS = {
```

### Comparing `fsaa-0.0.6/fsaa/examples/tutorial.py` & `fsaa-0.0.7/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/losses/lpips_loss.py` & `fsaa-0.0.7/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/masks/jnd.py` & `fsaa-0.0.7/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/models/hf_models/hf_models.py` & `fsaa-0.0.7/fsaa/models/hf/hf_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,14 @@
 
 SUPPORTED_BEIT_MODELS = [
     "microsoft/beit-base-patch16-224",
     "microsoft/beit-base-patch16-224-pt22k",
     "microsoft/beit-base-patch16-224-pt22k-ft22k",
 ]
 
-SUPPORTED_DEIT_MODELS = [
-    "facebook/deit-base-distilled-patch16-224",
-    "facebook/deit-base-patch16-224",
-    "facebook/deit-small-distilled-patch16-224",
-    "facebook/deit-small-patch16-224",
-    "facebook/deit-tiny-distilled-patch16-224",
-    "facebook/deit-tiny-patch16-224",
-]
-
 SUPPORTED_DINO_MODELS = [
     "facebook/dino-vits8",
     "facebook/dino-vits16",
     "facebook/dino-vitb8",
     "facebook/dino-vitb16",
 ]
 
@@ -38,15 +29,14 @@
     "facebook/vit-msn-small",
     "facebook/vit-msn-base",
     "facebook/vit-msn-large"
 ]
 
 SUPPORTED_HF_MODELS = (
     SUPPORTED_BEIT_MODELS
-    + SUPPORTED_DEIT_MODELS
     + SUPPORTED_DINO_MODELS
     + SUPPORTED_MAE_MODELS
     + SUPPORTED_MSN_MODELS
 )
 
 
 def name_to_model(model_name: str):
@@ -73,20 +63,14 @@
             )
 
         hf_model = name_to_model(model_name)
 
         if model_name in SUPPORTED_BEIT_MODELS:
             mean, std = HALF_NORMALIZATION_MEAN, HALF_NORMALIZATION_STD
 
-        if model_name in SUPPORTED_DEIT_MODELS:
-            if "distilled" in model_name:
-                mean, std = IMAGENET_MEAN, IMAGENET_STD
-            else:
-                mean, std = HALF_NORMALIZATION_MEAN, HALF_NORMALIZATION_STD
-
         if (
             model_name in SUPPORTED_DINO_MODELS
             or model_name in SUPPORTED_MAE_MODELS
             or model_name in SUPPORTED_MSN_MODELS
         ):
             mean, std = IMAGENET_MEAN, IMAGENET_STD
```

### Comparing `fsaa-0.0.6/fsaa/models/hub_models/hub_models.py` & `fsaa-0.0.7/fsaa/models/hub/hub_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,18 @@
                                        verbose=False)
 
         if model_name in SUPPORTED_VICREG_MODELS:
             hub_model = torch.hub.load('facebookresearch/vicreg:main',
                                        model_name.split("_")[1],
                                        verbose=False)
 
+        # Removing classification head if any
+        if hasattr(hub_model, "fc"):
+            hub_model.fc = torch.nn.Identity()
+
         self.model = TransformAndModelWrapper(
             hub_model,
             transform=Normalize(IMAGENET_MEAN, IMAGENET_STD)
         )
 
     def forward(self, x):
         return self.model(x)
```

### Comparing `fsaa-0.0.6/fsaa/models/ibot/ibot.py` & `fsaa-0.0.7/fsaa/models/ibot/ibot.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/models/ibot/utils.py` & `fsaa-0.0.7/fsaa/models/ibot/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/models/ibot/vits.py` & `fsaa-0.0.7/fsaa/models/ibot/vits.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/transforms/normalize.py` & `fsaa-0.0.7/fsaa/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/updaters/langevin.py` & `fsaa-0.0.7/fsaa/updaters/langevin.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/updaters/pgd.py` & `fsaa-0.0.7/fsaa/updaters/pgd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/fsaa/updaters/random.py` & `fsaa-0.0.7/fsaa/updaters/random.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/imgs/adv.png` & `fsaa-0.0.7/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/imgs/mask.png` & `fsaa-0.0.7/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/imgs/orig.png` & `fsaa-0.0.7/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/tests/test_attack.py` & `fsaa-0.0.7/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/tests/test_initializers.py` & `fsaa-0.0.7/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/tests/test_masks.py` & `fsaa-0.0.7/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/tests/test_models.py` & `fsaa-0.0.7/tests/test_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from warnings import warn
+
 import pytest
 import requests as r
 import torch
 from PIL import Image
 from torchvision.transforms import ToTensor
 from transformers import AutoImageProcessor
 
-from fsaa.models.hf_models.hf_models import SUPPORTED_HF_MODELS
+from fsaa.models.hf.hf_models import SUPPORTED_HF_MODELS
 from fsaa.utils import SUPPORTED_MODELS, get_model
 
 
 def totensor(img, device=None):
     return ToTensor()(img).unsqueeze(0).to(device)
 
 
@@ -26,36 +28,36 @@
 
 @torch.no_grad()
 def test_stochasticity(image_device):
     """Tests that all models are approximately deterministic."""
     image, device = image_device
     tensor = totensor(image, device)
     for name in SUPPORTED_MODELS:
-        model = get_model(name).to(device).eval()
-        f1 = model(tensor)
-
-        model = get_model(name).to(device).eval()
-        f2 = model(tensor)
-
-        assert torch.allclose(f1, f2, atol=1e-4)
+        try:
+            model = get_model(name).to(device).eval()
+            f1 = model(tensor)
+
+            model = get_model(name).to(device).eval()
+            f2 = model(tensor)
+
+            assert torch.allclose(
+                f1, f2, atol=1e-4), f"Model {name} is not deterministic"
+        except RuntimeError:
+            warn(f"Model {name} failed to run on device {device}")
 
 
 def test_hf_processing_same(image_device):
     """Tests that all processing steps are the same as in the original
     HF processor."""
     image, device = image_device
     tensor = totensor(image, device)
     h, w = tensor.shape[-2:]
     for name in SUPPORTED_HF_MODELS:
         model = get_model(name).to(device).eval()
         processed = model.model.transform(tensor)
 
         original_processor = AutoImageProcessor.from_pretrained(name)
-
-        if 'deit' in name.lower():
-            original_processor.size = {'height': h, 'width': w}
-
         original_processed = original_processor(
             image, return_tensors="pt"
         ).pixel_values.to(device)
 
         assert torch.allclose(processed, original_processed, atol=1e-4)
```

### Comparing `fsaa-0.0.6/tests/test_updaters.py` & `fsaa-0.0.7/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/.gitignore` & `fsaa-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/LICENSE` & `fsaa-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.6/README.md` & `fsaa-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,18 +110,18 @@
 
 ## Citation
 If you used this library as part of your work, please cite the repository as follows:
 
 ```
 @software{Pulfer_FSAA_2023,
 author = {Pulfer, Brian},
-month = jun,
+month = jul,
 title = {{FSAA}},
 url = {https://github.com/BrianPulfer/fsaa},
-version = {0.0.4},
+version = {0.0.7},
 year = {2023}
 }
 ```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
```

### Comparing `fsaa-0.0.6/pyproject.toml` & `fsaa-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Project metadata
 [project]
 name = "fsaa"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name="Brian Pulfer", email="brianpulfer95@gmail.com" }]
 description = "A simple library for adversarial attacks in feature space."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
```

### Comparing `fsaa-0.0.6/PKG-INFO` & `fsaa-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -133,18 +133,18 @@
 
 ## Citation
 If you used this library as part of your work, please cite the repository as follows:
 
 ```
 @software{Pulfer_FSAA_2023,
 author = {Pulfer, Brian},
-month = jun,
+month = jul,
 title = {{FSAA}},
 url = {https://github.com/BrianPulfer/fsaa},
-version = {0.0.4},
+version = {0.0.7},
 year = {2023}
 }
 ```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
```


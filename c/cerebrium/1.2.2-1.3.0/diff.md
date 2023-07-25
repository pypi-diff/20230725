# Comparing `tmp/cerebrium-1.2.2.tar.gz` & `tmp/cerebrium-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.2.2.tar", max compression
+gzip compressed data, was "cerebrium-1.3.0.tar", max compression
```

## Comparing `cerebrium-1.2.2.tar` & `cerebrium-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0      372 2023-07-19 15:27:43.663596 cerebrium-1.2.2/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-07-19 15:27:43.663596 cerebrium-1.2.2/LICENSE
--rw-r--r--   0        0        0      360 2023-07-19 15:30:28.523832 cerebrium-1.2.2/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    39378 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/cli.py
--rw-r--r--   0        0        0    33936 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/conduit.py
--rw-r--r--   0        0        0     5048 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/core.py
--rw-r--r--   0        0        0     2488 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/errors.py
--rw-r--r--   0        0        0    10182 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/flow.py
--rw-r--r--   0        0        0     3070 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3990 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      600 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/models/base.py
--rw-r--r--   0        0        0      550 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      411 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/models/onnx.py
--rw-r--r--   0        0        0      793 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      270 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      273 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8545 2023-07-19 15:27:43.663596 cerebrium-1.2.2/cerebrium/requests.py
--rw-r--r--   0        0        0    10957 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/README_Diffusers.md
--rw-r--r--   0        0        0     5592 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/README_Transformers.md
--rw-r--r--   0        0        0      110 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     1819 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/diffuser_config.yaml
--rw-r--r--   0        0        0    15030 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/diffuser_tuner.py
--rw-r--r--   0        0        0     1836 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/example_configs/falcon-40b.yaml
--rw-r--r--   0        0        0     1804 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/example_configs/falcon-7b.yaml
--rw-r--r--   0        0        0     9079 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1716 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
--rw-r--r--   0        0        0     2647 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
--rw-r--r--   0        0        0     4115 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
--rw-r--r--   0        0        0     1593 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/trainer/transformer_config.yaml
--rw-r--r--   0        0        0     1048 2023-07-19 15:27:43.667595 cerebrium-1.2.2/cerebrium/utils.py
--rw-r--r--   0        0        0     2378 2023-07-19 15:30:28.519832 cerebrium-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 cerebrium-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-07-25 14:13:12.773940 cerebrium-1.3.0/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-07-25 14:13:12.777940 cerebrium-1.3.0/LICENSE
+-rw-r--r--   0        0        0      360 2023-07-25 14:16:12.471104 cerebrium-1.3.0/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    36049 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/cli.py
+-rw-r--r--   0        0        0    35162 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5048 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/core.py
+-rw-r--r--   0        0        0     2488 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      411 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/requests.py
+-rw-r--r--   0        0        0    10957 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     2515 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/diffuser.yaml
+-rw-r--r--   0        0        0     1940 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/falcon-40b.yaml
+-rw-r--r--   0        0        0     1864 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/falcon-7b.yaml
+-rw-r--r--   0        0        0     1916 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama-13b.yaml
+-rw-r--r--   0        0        0     1692 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama-7b.yaml
+-rw-r--r--   0        0        0     1991 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama2-13b.yaml
+-rw-r--r--   0        0        0     1751 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/llama2-7b.yaml
+-rw-r--r--   0        0        0     1747 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/config/transformer.yaml
+-rw-r--r--   0        0        0    15030 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     8826 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     4115 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1048 2023-07-25 14:13:12.777940 cerebrium-1.3.0/cerebrium/utils.py
+-rw-r--r--   0        0        0     2346 2023-07-25 14:16:12.467104 cerebrium-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 cerebrium-1.3.0/PKG-INFO
```

### Comparing `cerebrium-1.2.2/LICENSE` & `cerebrium-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/cli.py` & `cerebrium-1.3.0/cerebrium/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,16 @@
         sys.exit(1)
     return config["api_key"]
 
 
 @app.command()
 def init_trainer(
     training_type: str = typer.Argument(
-        "", help="Type of training to run. Can be either 'diffuser' or 'transformer'."
+        "",
+        help="Type of training to run. Can be either 'diffuser' or 'transformer'. Optionally you can choose a specific model. Can be any in {'falcon-7b', 'llama-7b/13b', 'llama2-7b/13b'}",
     ),
     config_path: str = typer.Argument(
         "",
         help="Path to directory where you would like to init a Cerebrium cortex project.",
     ),
     api_key: str = typer.Option(
         "", help="Private API key for the user. Not included in config by default."
@@ -107,150 +108,64 @@
     overwrite: bool = typer.Option(
         False, help="Whether to overwrite contents of the init_dir."
     ),
 ):
     """
     Initialises an empty Cerebrium trainer project.
     """
-    if not training_name:
-        # deployment_name = typer.prompt("Enter a name for your deployment")
-        training_name = "YOUR_DEPLOYMENT_NAME_HERE"
-
     # check the config file does not exist
     if os.path.exists(config_path) and not overwrite:
-        print("Found a config file at {config_path}. Please specify an empty directory.")
-        sys.exit(1)
-    
-    # check the training type is valid
-    if training_type not in ["diffuser", "transformer"]:
-        print(f"Your training type {training_type} is not supported.")
+        print(
+            "Found a config file at {config_path}. Please specify a new name or use the --overwrite flag if you want to overwrite."
+        )
         sys.exit(1)
-    
+
     # if the config file extention is not yaml, add it
     if os.path.splitext(config_path)[1] != ".yaml":
         config_path = os.path.splitext(config_path)[0] + ".yaml"
-        
 
-    config = """%YAML 1.2
----
-training_type: {training_type} # Type of training to run. Either "diffuser" or "transformer". In this case, "transformer".
-name: {deployment_name} # Your name for the fine-tuning run.""".format(
-        training_type=training_type, deployment_name=training_name
-    )
-    if api_key:
-        config += """\napi_key: {api_key} # Your Cerebrium private API key. Not included in config by default.""".format(
-            api_key=api_key
+    # Load in the config for the training_type
+    base_path = os.path.join(os.path.dirname(trainer.__file__), "config")
+    base_config_path = os.path.join(base_path, f"{training_type}.yaml")
+    if not os.path.exists(base_config_path):
+        print(
+            f"Your training type {training_type} is not supported yet. Please contact Cerebrium support on Slack or Discord if you would like it added."
         )
-
-    if training_type == "transformer":
-        config += """
-
-# Model params:
-hf_model_path: "YOUR_HUGGINGFACE_MODEL_PATH_HERE" # path to your local HuggingFace model.
-model_type: "AutoModelForCausalLM"
-dataset_path: path/to/your/dataset.json # path to your local JSON dataset.
-
-###############################################################
-#  Optional Parameters
-###############################################################
-custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
-seed: 42 # random seed for reproducibility.
-log_level: "INFO" # log_level level for logging.
-
-# Training params:
-training_args:
-  logging_steps: 100
-  per_device_train_batch_size: 15
-  per_device_eval_batch_size: 15
-  warmup_steps: 0
-  gradient_accumulation_steps: 4
-  num_train_epochs: 50
-  learning_rate: 0.0001
-  group_by_length: False
-
-base_model_args: # args for loading in the base model with AutoModelForCausalLM
-  load_in_8bit: True
-  device_map: "auto"
-
-peft_lora_args: # peft lora args.
-  r: 8
-  lora_alpha: 32
-  lora_dropout: 0.05
-  target_modules: ["q_proj", "v_proj"]
-  bias: "none"
-  task_type: "CAUSAL_LM"
-
-dataset_args:
-  prompt_template: "short" # Prompt template to use. Either "short" or "long".
-  instruction_column: "prompt" # column  name of your prompt in the dataset.json
-  label_column: "completion" # column name of your label/completion in the dataset.json
-  context_column: "context" # optional column name of your context in the dataset.json
-  cutoff_len: 512 # cutoff length for the prompt.
-  train_val_ratio: 0.9 # ratio of training to validation data in the dataset split.
-
-    """
-
-    elif training_type == "diffuser":
-        config += """
-hf_model_path: "YOUR_HUGGINGFACE_MODEL_PATH_HERE" # Path to the huggingface diffusion model to train.
-train_prompt: "INSERT YOUR TRAINING PROMPT" # Your prompt to train.
-log_level: "INFO" # log_level level for logging. Can be "DEBUG", "INFO", "WARNING", "ERROR".
-
-###############################################################
-#  Optional Parameters
-###############################################################
-# Diffuser params
-prior_class_prompt: "INSERT YOUR PRIOR CLASS PROMPT HERE" # Your prompt to train prior class images. Only use if you would like to train prior class images.
-revision: "main" # Revision of the diffuser model to use.
-validation_prompt: ~ # an optional validation prompt to use. If ~, will use the training prompt.
-custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
-
-# Dataset params
-train_image_dir: data/training_class_images/ # Directory of training images.
-prior_class_image_dir: ~ # or "path/to/your/prior_class_images". Optional directory of images to use if you would like to train prior class images as well.
-
-# Training params
-training_args:
-  # General training params
-  learning_rate: 1.0E-5
-  num_validation_images: 4 # Number of images to generate in validation.
-  num_train_epochs: 50
-  seed: 1
-  resolution: 512 # Resolution to train images at.
-  center_crop: False # Whether to center crop images to resolution.
-  train_batch_size: 2
-  num_prior_class_images: 0 # Number of prior class images to train on. If 0, will not generate any prior class images. Requires prior_class_prompt to be set.
-  prior_class_generation_batch_size: 2
-  prior_loss_weight: 1.0 # Weight of prior loss in the total loss if using.
-  max_train_steps: ~ # maximum training steps which overrides number of training epochs
-  validation_epochs: 5 # number of epochs before running validation and checkpointing
-
-  # Training loop params
-  gradient_accumulation_steps: 1
-  lr_scheduler: "constant"
-  lr_warmup_steps: 50
-  lr_num_cycles: 1
-  lr_power: 1.0
-  allow_tf32: False
-  max_grad_norm: 1.0
-  mixed_precision: "no" # If you would like to use mixed precision. Supports fp16 and bf16. Defaults to 'no'
-  prior_generation_precision: ~
-  scale_lr: False
-  use_8bit_adam: True
-  use_xformers: True # Whether to use xformers memory efficient attention or not.
-
-"""
-    else:
-        print(f"Your training type {training_type} is not supported.")
         sys.exit(1)
 
+    if training_type not in ["diffuser", "transformer"]:
+        transformer_models = ["falcon", "llama", "llama2"]
+        if training_type.split("-")[0] in transformer_models:
+            training_type = "transformer"
+
+    # modify the base config by matching the yaml params.
+    # cannot load the yaml file as we want to preserve comments.
+    with open(base_config_path, "r") as f:
+        config = f.readlines()
+
+    defaults = {
+        "training_type": training_type,
+        "name": training_name,
+        "api_key": api_key,
+    }
+    for i, line in enumerate(config):
+        for k, v in defaults.items():
+            if not v:  # skip if val is None or empty string
+                continue
+            l = line.lstrip()
+            indent_level = len(line) - len(l)  # strip the leading whitespaces
+            if l.startswith(f"{k}:"):
+                config[i] = f"{' '*indent_level}{k}: {v}\n"
+
     # write config.yaml
     with open(config_path, "w") as f:
         f.writelines(config)
 
+    print(f"✅  Config file written to {config_path}.")
+
 
 @app.command()
 def init_cortex(
     init_dir: str = typer.Argument(
         "",
         help="Path to directory where you would like to init a Cerebrium cortex project.",
     ),
```

### Comparing `cerebrium-1.2.2/cerebrium/conduit.py` & `cerebrium-1.3.0/cerebrium/conduit.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     def __init__(
         self,
         name: str = "",
         api_key: str = "",
         flow: CerebriumFlow = [],
         hardware: Union[Hardware, None] = None,
         from_json: str = "",
+        requirements_file: str = "",
     ):
         if not from_json:
             self.api_key = api_key or os.environ.get("CEREBRIUM_API_KEY", "")
             assert name != "" and self.api_key != ""
             # Check that the flow name is valid
             if len(name) > 20:
                 raise ValueError("Conduit name must be less than 20 characters")
@@ -89,14 +90,31 @@
                     )
                 hardware = Hardware(config["hardware"])
         _set_api_key(self.api_key)
         self.graph = []
         self.ready = False
         self.loggers = {}
         self.hardware = hardware or self._determine_hardware()
+
+        self.requirements_file = requirements_file
+        if self.requirements_file:
+            assert os.path.exists(
+                self.requirements_file
+            ), f"Requirements file {self.requirements_file} does not exist"
+            assert os.path.isfile(
+                self.requirements_file
+            ), f"Requirements file {self.requirements_file} is not a file"
+            assert self.requirements_file.endswith(
+                ".txt"
+            ), f"Requirements file {self.requirements_file} is not a .txt file"
+            ## Calc MD5 hash of ./requirements.txt
+            # if os.path.exists("./requirements.txt"):
+            #     with open("./requirements.txt", "rb") as f:
+            #         self.requirements_hash = hashlib.md5(f.read()).hexdigest()
+
         try:
             from torch.cuda import is_available
 
             self.device = (
                 "cuda" if self.hardware == Hardware.GPU and is_available() else "cpu"
             )
         except ImportError:
@@ -636,14 +654,15 @@
                             "post": None
                             if p[2].get("post", None) is None
                             else getsource(p[2]["post"]),  # type: ignore
                         }
                         for p in self.flow
                     ],
                     "hardware": self.hardware.value,
+                    # "requirements_hash": self.requirements_hash if self.requirements_file else ""
                 },
                 f,
                 indent=2,
             )
 
     def _upload(self, url):
         """
@@ -673,14 +692,21 @@
             # Create a zip file of the Conduit, writing the model files and Conduit object to the zip
             with zipfile.ZipFile(f"{tmpdir}/{self.name}.zip", "w") as zip:
                 for model_type, model_initialization, _ in self.flow:
                     if model_type != ModelType.HUGGINGFACE_PIPELINE:
                         assert isinstance(model_initialization, str)
                         true_path: str = os.path.abspath(model_initialization)
                         zip.write(true_path, os.path.basename(true_path))
+
+                        ## If the user has provided a requirements file, write it to the zip
+                        if self.requirements_file:
+                            zip.write(
+                                self.requirements_file, arcname="requirements.txt"
+                            )
+
                         ## If the model is a spaCy model, write all the folder contents to the zip
                         ## This is necessary because spaCy models are directories
                         if model_type == ModelType.SPACY:
                             for root, _, files in os.walk(true_path):
                                 for file in files:
                                     directory = os.path.basename(root)
                                     directory = (
```

### Comparing `cerebrium-1.2.2/cerebrium/core.py` & `cerebrium-1.3.0/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/errors.py` & `cerebrium-1.3.0/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/flow.py` & `cerebrium-1.3.0/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/logging/arize.py` & `cerebrium-1.3.0/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/logging/base.py` & `cerebrium-1.3.0/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/logging/censius.py` & `cerebrium-1.3.0/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/models/base.py` & `cerebrium-1.3.0/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/models/hf_pipeline.py` & `cerebrium-1.3.0/cerebrium/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/models/sklearn.py` & `cerebrium-1.3.0/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/requests.py` & `cerebrium-1.3.0/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/README_Diffusers.md` & `cerebrium-1.3.0/cerebrium/trainer/README_Diffusers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/README_Transformers.md` & `cerebrium-1.3.0/cerebrium/trainer/README_Transformers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/diffuser_config.yaml` & `cerebrium-1.3.0/cerebrium/trainer/config/diffuser.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 %YAML 1.2
 ---
-training_type: "diffuser" # Type of training to run. Either "diffuser" or "transformer".
-name: "test-config-file" # Name of the experiment.
-api-key: "YOUR API KEY HERE" # Your Cerebrium API key.
-hf_model_path: "runwayml/stable-diffusion-v1-5"
+training_type: { training_type } # Type of training to run. Either "diffuser" or "transformer". In this case, "transformer".
+name: { deployment_name } # Your name for the fine-tuning run.
+
+# Model params:
+hf_model_path: "YOUR_HUGGINGFACE_MODEL_PATH_HERE" # Path to the huggingface diffusion model to train.
+train_prompt: "INSERT YOUR TRAINING PROMPT" # Your prompt to train.
+log_level: "INFO" # log_level level for logging. Can be "DEBUG", "INFO", "WARNING", "ERROR".
+
+###############################################################
+#  Optional Parameters
+###############################################################
+# Diffuser params
+prior_class_prompt: "INSERT YOUR PRIOR CLASS PROMPT HERE" # Your prompt to train prior class images. Only use if you would like to train prior class images.
 revision: "main" # Revision of the diffuser model to use.
-train_prompt: "Photo of a tsdf dog."
 validation_prompt: ~ # an optional validation prompt to use. If ~, will use the training prompt.
 custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
-log_level: "WARNING" # log_level level for logging.
 
+# Dataset params
 train_image_dir: data/training_class_images/ # Directory of training images.
-prior_class_image_dir: ~ # "data/prior_class_images" # Optional directory of images to use for prior class.
-prior_class_prompt: "Photo of a dog."
+prior_class_image_dir: ~ # or "path/to/your/prior_class_images". Optional directory of images to use if you would like to train prior class images as well.
 
 # Training params
 training_args:
   # General training params
+  learning_rate: 1.0E-5
   num_validation_images: 4 # Number of images to generate in validation.
-  learning_rate: 1.0E-4
-  num_train_epochs: 30
-  seed: ~
+  num_train_epochs: 50
+  seed: 1
   resolution: 512 # Resolution to train images at.
   center_crop: False # Whether to center crop images to resolution.
   train_batch_size: 2
-  num_prior_class_images: 10
+  num_prior_class_images: 0 # Number of prior class images to train on. If 0, will not generate any prior class images. Requires prior_class_prompt to be set.
   prior_class_generation_batch_size: 2
-  prior_loss_weight: 1.0 # Weight of prior loss in the total loss.
+  prior_loss_weight: 1.0 # Weight of prior loss in the total loss if using.
   max_train_steps: ~ # maximum training steps which overrides number of training epochs
-  validation_epochs: 10 # number of epochs before running validation and checkpointing
+  validation_epochs: 5 # number of epochs before running validation and checkpointing
 
   # Training loop params
   gradient_accumulation_steps: 1
   lr_scheduler: "constant"
-  lr_warmup_steps: 5
+  lr_warmup_steps: 50
   lr_num_cycles: 1
   lr_power: 1.0
   allow_tf32: False
   max_grad_norm: 1.0
-  mixed_precision: "no" # "fp16 or "bf16"
+  mixed_precision: "no" # If you would like to use mixed precision. Supports fp16 and bf16. Defaults to 'no'
   prior_generation_precision: ~
   scale_lr: False
   use_8bit_adam: True
   use_xformers: True # Whether to use xformers memory efficient attention or not.
```

### Comparing `cerebrium-1.2.2/cerebrium/trainer/diffuser_tuner.py` & `cerebrium-1.3.0/cerebrium/trainer/diffuser_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/example_configs/falcon-40b.yaml` & `cerebrium-1.3.0/cerebrium/trainer/config/falcon-40b.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 %YAML 1.2
 ---
 training_type: "transformer" # Type of training to run. Either "diffuser" or "transformer".
 
-name: test-falcon-40b # Name of the experiment.
+name: your-falcon40b-name-here # Name of the experiment.
 api_key: Your Cerebrium API key here
 
 # Model params:
 hf_model_path: "tiiuae/falcon-40b"
 model_type: "AutoModelForCausalLM"
 dataset_path: path/to/your/local/JSON/dataset.json
 custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
 seed: 42 # random seed for reproducibility.
 log_level: "INFO" # log_level level for logging.
 
 # Training params:
 training_args:
-  logging_steps: 100
+  logging_steps: 10
   per_device_train_batch_size: 2 # These batch sizes have not been optimised as they are hardware dependent.
   per_device_eval_batch_size: 2
   warmup_steps: 0
   gradient_accumulation_steps: 4
-  num_train_epochs: 30
+  num_train_epochs: 50
+  # max_steps: 1000 # an optional if you would like to use steps instead of epochs.
   learning_rate: 2.0e-4
   group_by_length: False
   fp16: True
   max_grad_norm: 0.3
-  # max_steps: 1000 # an optional if you would like to use steps instead of epochs.
   lr_scheduler_type: "constant"
 
 base_model_args: # args for loading in the base model.
   load_in_8bit: True
   device_map: "auto"
   trust_remote_code: True
 
@@ -38,19 +38,20 @@
   lora_alpha: 16
   lora_dropout: 0.05
   target_modules: ["query_key_value"] # This has to be query_key_value for falcon
   bias: "none"
   task_type: "CAUSAL_LM"
 
 dataset_args:
-  # prompt_template: "short"
   # if you would like a custom prompt template it's possible to specify it here as below:
   prompt_template:
     description: "A shorter template to experiment with."
     prompt_input: "### Instruction:\n{instruction}\n\n### Input:\n{input}\n\n### Response:\n"
     prompt_no_input: "### Instruction:\n{instruction}\n\n### Response:\n"
     response_split: "### Response:"
+  # otherwise use `prompt_template: "short"`
+  # if your dataset has data labelled differently, you can set the labels here:
   instruction_column: "prompt"
   label_column: "completion"
   context_column: "context"
   cutoff_len: 512
   train_val_ratio: 0.9
```

### Comparing `cerebrium-1.2.2/cerebrium/trainer/example_configs/falcon-7b.yaml` & `cerebrium-1.3.0/cerebrium/trainer/config/falcon-7b.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 %YAML 1.2
 ---
 training_type: "transformer" # Type of training to run. Either "diffuser" or "transformer".
 
-name: test-falcon-7b # Name of the experiment.
+name: your-falcon7b-name-here # Name of the experiment.
 api_key: Your Cerebrium API key here
 
 # Model params:
 hf_model_path: "tiiuae/falcon-7b"
 model_type: "AutoModelForCausalLM"
 dataset_path: path/to/your/local/JSON/dataset.json
 custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
 seed: 42 # random seed for reproducibility.
 log_level: "INFO" # log_level level for logging.
 
 # Training params:
 training_args:
-  logging_steps: 100
-  per_device_train_batch_size: 10 # TODO - optimise batch sizes for hardware.
+  num_train_epochs: 50
+  # max_steps: 1000 # an optional if you would like to use steps instead of epochs.
+  learning_rate: 2.0e-4
+  per_device_train_batch_size: 10
   per_device_eval_batch_size: 10
   warmup_steps: 0
+  logging_steps: 10
   gradient_accumulation_steps: 4
-  num_train_epochs: 30
-  learning_rate: 2.0e-4
   group_by_length: False
   fp16: True
   max_grad_norm: 0.3
-  # max_steps: 1000 # an optional if you would like to use steps instead of epochs.
   lr_scheduler_type: "constant"
 
 base_model_args: # args for loading in the base model.
   load_in_8bit: True
   device_map: "auto"
   trust_remote_code: True
 
@@ -38,19 +38,20 @@
   lora_alpha: 16
   lora_dropout: 0.05
   target_modules: ["query_key_value"] # This has to be query_key_value for falcon
   bias: "none"
   task_type: "CAUSAL_LM"
 
 dataset_args:
-  # prompt_template: "short"
   # if you would like a custom prompt template it's possible to specify it here as below:
   prompt_template:
     description: "A shorter template to experiment with."
     prompt_input: "### Instruction:\n{instruction}\n\n### Input:\n{input}\n\n### Response:\n"
     prompt_no_input: "### Instruction:\n{instruction}\n\n### Response:\n"
     response_split: "### Response:"
+  # otherwise use `prompt_template: "short"`
+  # if your dataset has data labelled differently, you can set the labels here:
   instruction_column: "prompt"
   label_column: "completion"
   context_column: "context"
   cutoff_len: 512
   train_val_ratio: 0.9
```

### Comparing `cerebrium-1.2.2/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.3.0/cerebrium/trainer/fine_tuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,14 @@
             self.config = config
 
         self.config["training_type"] = "transformer"
         self.config["name"] = name
 
         # override with log_level from params
         self.config["log_level"] = log_level or self.config["log_level"]
-        if (
-            str.find(self.config["hf_model_path"], "llama") != -1
-        ):  # if llama model, use llama tokenizer. This seems to have broken in the latest huggingface release
-            self.config["custom_tokenizer"] = "LlamaTokenizer"
 
         # backup for user to see what they sent
         self.config["user_base_model_kwargs"] = copy(self.config["base_model_args"])
         self.config["user_peft_kwargs"] = copy(self.config["peft_lora_args"])
 
         # will set to our defaults. Easier for beginners.
         # Calling here so that a user can access the defaults and check them before training.
```

### Comparing `cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/finetuning_model.py` & `cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py` & `cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py` & `cerebrium-1.3.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/cerebrium/trainer/transformer_config.yaml` & `cerebrium-1.3.0/cerebrium/trainer/config/llama-7b.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 %YAML 1.2
 ---
 training_type: "transformer" # Type of training to run. Either "diffuser" or "transformer".
 
-name: test-config-file # Name of the experiment.
-api_key: YOUR API KEY HERE # Your Cerebrium API key.
+name: your-llama-7b-name-here # Name of the experiment.
+api_key: Your Cerebrium API key.
 
 # Model params:
 hf_model_path: "decapoda-research/llama-7b-hf"
 model_type: "AutoModelForCausalLM"
-dataset_path: path/to/your/dataset.json # path to your local JSON dataset.
-custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
+dataset_path: /path/to/your/dataset.json # path to your local JSON dataset.
+custom_tokenizer: "LlamaTokenizer" # custom tokenizer from AutoTokenizer if required.
 seed: 42 # random seed for reproducibility.
 log_level: "INFO" # log_level level for logging.
 
 # Training params:
 training_args:
   logging_steps: 10
   per_device_train_batch_size: 15
   per_device_eval_batch_size: 15
   warmup_steps: 0
   gradient_accumulation_steps: 4
-  num_train_epochs: 3
+  num_train_epochs: 50
   learning_rate: 0.0001
   group_by_length: False
 
 base_model_args: # args for loading in the base model.
   load_in_8bit: True
   device_map: "auto"
 
@@ -33,19 +33,20 @@
   lora_alpha: 32
   lora_dropout: 0.05
   target_modules: ["q_proj", "v_proj"]
   bias: "none"
   task_type: "CAUSAL_LM"
 
 dataset_args:
-  # prompt_template: "short"
   # if you would like a custom prompt template it's possible to specify it here as below:
   prompt_template:
     description: "A shorter template to experiment with."
     prompt_input: "### Instruction:\n{instruction}\n\n### Input:\n{input}\n\n### Response:\n"
     prompt_no_input: "### Instruction:\n{instruction}\n\n### Response:\n"
     response_split: "### Response:"
+  # otherwise use `prompt_template: "short"`
+  # if your dataset has data labelled differently, you can set the labels here:
   instruction_column: "prompt"
   label_column: "completion"
   context_column: "context"
   cutoff_len: 512
   train_val_ratio: 0.9
```

### Comparing `cerebrium-1.2.2/cerebrium/utils.py` & `cerebrium-1.3.0/cerebrium/utils.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.2/pyproject.toml` & `cerebrium-1.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.2.2"
+version = "1.3.0"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "EXTERNAL_README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*", "README.md"]
 
 [tool.poetry.urls]
@@ -25,64 +25,68 @@
 python = ">=3.8,<3.12"
 cloudpickle = ">=2.2"
 requests = "^2.30"
 tqdm = ">=4.64,<4.65"
 tenacity = ">=8.2,<8.3"
 yaspin = ">=2.3,<2.4"
 loguru = ">=0.7"
-jsonschema = "^4.17.3"
+jsonschema = ">=4.18.4"
 censius = { version = "^1.6", optional= true }
 arize = { version = ">=6.0.2", optional= true }
 pandas = { version = ">=1.5,<3.0", optional= true }
 typer = { version = ">=0.7.0", extras = ["all"] }
+typing_extensions = ">=3.6.6"
 prodict = ">=0.8.18,<0.9.0"
 pyyaml = ">=6.0,<7.0"
 
 [tool.poetry.group.dev.dependencies]
-black = {extras = ["jupyter"], version= ">=23.3,<24.0"}
+black = {extras = ["jupyter"], version= "23.3,<24.0"}
 ipython = ">=8.9,<9.0"
 ipykernel = ">=6.21,<7.0"
 poetry-dotenv = "0.3.0"
 poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.24,<1.0"}
 pytest = ">=7.4,<8.0"
 coverage = ">=7.2,<8.0"
 pytest-cov = ">=4.1,<5.0"
 notebook = ">=6.5,<7.0"
 
+[tool.poetry.group.server]
+optional = true
+
 [tool.poetry.group.server.dependencies]
 ddtrace = ">=1.15,<1.20.0"
 datadog = ">=0.45,<0.51.0"
-celery = {extras = ["s3", "sqs"], version = ">=5.3,<5.4.0"}
-boto3 = ">=1.28,<1.30"
-fastapi = ">=0.99.1"
-uvicorn = ">=0.21.1"
+celery = {extras = ["s3", "sqs"], version = "5.3.1"}
+boto3 = "1.28.8"
+fastapi = "0.88.0"
+uvicorn = "0.23.1"
+
+
+[tool.poetry.group.ml]
+optional = true
 
 [tool.poetry.group.ml.dependencies]
-xgboost = ">=1.7,<1.8"
-numpy = ">=1.24,<1.30"
-torch = ">=2.0,<2.2"
-scikit-learn = ">=1.3,<1.4.0"
-transformers = ">=4.30,<4.40"
+xgboost = "1.7.6"
+numpy = "1.24.3"
+torch = ">=2.0.0, !=2.0.1"
+scikit-learn = "1.3.0"
+transformers = ">=4.30"
 datasets =">=2.10.0,<2.11.0"
 accelerate = ">=0.20.0"
-bitsandbytes = ">=0.38,<0.39.0"
+bitsandbytes = ">=0.38"
 peft = ">=0.3"
-onnxruntime = ">=1.15"
-
-
-[tool.poetry.group.ml-misc]
-optional = true
+onnxruntime = "1.15.1"
+onnx = "1.14.0"
+tensorflow = "2.13.0"
+keras = "2.13.1"
+Pillow = "10.0.0"
+sentencepiece = "0.1.99"
+spacy = "3.6.0"
+torchvision = ">=0.15.1"
 
-[tool.poetry.group.ml-misc.dependencies]
-tensorflow = ">=2.13,<2.14"
-keras = ">=2.13,<2.14"
-Pillow = ">=9.4,<10.0.0"
-sentencepiece = ">=0.1.99,<0.2.0"
-spacy = ">=3.5"
-torchvision = ">=0.15,<0.16"
 
 
 [tool.poetry.extras]
 monitoring = ["censius", "arize", "pandas"]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
```

### Comparing `cerebrium-1.2.2/PKG-INFO` & `cerebrium-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.2.2
+Version: 1.3.0
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: monitoring
 Requires-Dist: arize (>=6.0.2) ; extra == "monitoring"
 Requires-Dist: censius (>=1.6,<2.0) ; extra == "monitoring"
 Requires-Dist: cloudpickle (>=2.2)
-Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: jsonschema (>=4.18.4)
 Requires-Dist: loguru (>=0.7)
 Requires-Dist: pandas (>=1.5,<3.0) ; extra == "monitoring"
 Requires-Dist: prodict (>=0.8.18,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.30,<3.0)
 Requires-Dist: tenacity (>=8.2,<8.3)
 Requires-Dist: tqdm (>=4.64,<4.65)
 Requires-Dist: typer[all] (>=0.7.0)
+Requires-Dist: typing_extensions (>=3.6.6)
 Requires-Dist: yaspin (>=2.3,<2.4)
 Project-URL: Documentation, https://docs.cerebrium.ai/
 Project-URL: Homepage, https://www.cerebrium.ai
 Description-Content-Type: text/markdown
 
 # Cerebrium
```


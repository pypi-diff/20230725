# Comparing `tmp/spatialprompt-0.0.3.tar.gz` & `tmp/SpatialPrompt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialprompt-0.0.3.tar", last modified: Fri Apr 28 16:58:26 2023, max compression
+gzip compressed data, was "SpatialPrompt-0.0.4.tar", last modified: Tue Jul 25 07:31:05 2023, max compression
```

## Comparing `spatialprompt-0.0.3.tar` & `SpatialPrompt-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/
--rw-------   0 asish     (1000) asish     (1000)        0 2022-08-07 15:26:46.000000 spatialprompt-0.0.3/LICENCE.txt
--rw-------   0 asish     (1000) asish     (1000)       30 2022-08-07 15:26:46.000000 spatialprompt-0.0.3/MANIFEST.in
--rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/PKG-INFO
--rw-------   0 asish     (1000) asish     (1000)      108 2023-04-28 09:19:00.000000 spatialprompt-0.0.3/README.md
--rw-rw-r--   0 asish     (1000) asish     (1000)       38 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/setup.cfg
--rw-------   0 asish     (1000) asish     (1000)      841 2023-04-28 16:57:33.000000 spatialprompt-0.0.3/setup.py
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 16:58:26.547916 spatialprompt-0.0.3/spatialprompt/
--rw-------   0 asish     (1000) asish     (1000)    19750 2023-04-28 16:57:21.000000 spatialprompt-0.0.3/spatialprompt/__init__.py
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/spatialprompt.egg-info/
--rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/PKG-INFO
--rw-rw-r--   0 asish     (1000) asish     (1000)      252 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/SOURCES.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)        1 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/dependency_links.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)       83 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/requires.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)       14 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/top_level.txt
+drwxr-xr-x   0 swainasish  (1000) swainasish  (1000)        0 2023-07-25 07:31:05.651253 SpatialPrompt-0.0.4/
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)        0 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/LICENCE.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)       30 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/MANIFEST.in
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)      679 2023-07-25 07:31:05.651253 SpatialPrompt-0.0.4/PKG-INFO
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)      108 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/README.md
+drwxr-xr-x   0 swainasish  (1000) swainasish  (1000)        0 2023-07-25 07:31:05.651253 SpatialPrompt-0.0.4/SpatialPrompt.egg-info/
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)      679 2023-07-25 07:31:05.000000 SpatialPrompt-0.0.4/SpatialPrompt.egg-info/PKG-INFO
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)      404 2023-07-25 07:31:05.000000 SpatialPrompt-0.0.4/SpatialPrompt.egg-info/SOURCES.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)        1 2023-07-25 07:31:05.000000 SpatialPrompt-0.0.4/SpatialPrompt.egg-info/dependency_links.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)       83 2023-07-25 07:31:05.000000 SpatialPrompt-0.0.4/SpatialPrompt.egg-info/requires.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)       14 2023-07-25 07:31:05.000000 SpatialPrompt-0.0.4/SpatialPrompt.egg-info/top_level.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)       38 2023-07-25 07:31:05.651253 SpatialPrompt-0.0.4/setup.cfg
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)      841 2023-07-25 07:27:03.000000 SpatialPrompt-0.0.4/setup.py
+drwxr-xr-x   0 swainasish  (1000) swainasish  (1000)        0 2023-07-25 07:31:05.651253 SpatialPrompt-0.0.4/spatialprompt/
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)    19935 2023-07-25 07:26:19.000000 SpatialPrompt-0.0.4/spatialprompt/__init__.py
+drwxr-xr-x   0 swainasish  (1000) swainasish  (1000)        0 2023-07-25 07:31:05.651253 SpatialPrompt-0.0.4/spatialprompt.egg-info/
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)      252 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/spatialprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)        1 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/spatialprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)       83 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/spatialprompt.egg-info/requires.txt
+-rw-r--r--   0 swainasish  (1000) swainasish  (1000)       14 2023-07-25 06:48:57.000000 SpatialPrompt-0.0.4/spatialprompt.egg-info/top_level.txt
```

### Comparing `spatialprompt-0.0.3/setup.py` & `SpatialPrompt-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
   'Intended Audience :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
-  name='spatialprompt',
-  version='0.0.3',   #mandatory change
+  name='SpatialPrompt',
+  version='0.0.4',   #mandatory change
   description='Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics',
   long_description=open('README.md').read() ,
   url='',  
   author='Asish Kumar Swain',
   author_email='swainkasish@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `spatialprompt-0.0.3/spatialprompt/__init__.py` & `SpatialPrompt-0.0.4/spatialprompt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 Created on Tue Jun 28 12:11:26 2022
 @author: swainkasish@gmail.com
-spatialprompt_V 0.0.3
+spatialprompt_V 0.0.4
 """
-#%%
 #%% import libraries 
 import numpy as np
 import pandas as pd 
 import time 
 from sklearn.preprocessing import  StandardScaler,Normalizer,MinMaxScaler
 from sklearn.decomposition import PCA,TruncatedSVD
 from sklearn.neighbors import KNeighborsRegressor
 from alive_progress import alive_bar
 from scipy.spatial import cKDTree
 from  scipy.spatial.distance import cdist
 from sklearn.cluster import KMeans,AgglomerativeClustering
 from sklearn.linear_model import Ridge,RidgeCV
-
-#%%
+#%% fast spatial_prompt 
 class SpatialDeconvolution:
     def __init__(self):
         pass
     
     def __preprocessing__(self,sc_array,st_array,sc_genes,st_genes,n_hvgs=1000):
         
         '''
@@ -66,14 +64,15 @@
                     pass
                 sc_cg_df = self.__norm_hvg__(sc_cg_df)
                 sc_vars = sc_cg_df.var().to_numpy()
                 bar()
                 sorted_variance_indexes = np.argsort(sc_vars)[::-1]
                 bar()
                 top_hvg_index = sorted_variance_indexes[0:n_hvgs]
+                
                 self.hvgs = sc_cg_df.columns[top_hvg_index]
                 sc_df = sc_df.loc[:,self.hvgs]
                 st_df = st_df.loc[:,self.hvgs]
                 bar()
         n_hvg_final = sc_df.shape[1]
         print(f"{len(common_genes)} Common Genes Found {n_hvg_final} HVGs Retained")
 
@@ -285,58 +284,54 @@
             old_weightage = 1-nei_weightage
             expr_micro_env = np.array([expr_spatial_neighbor[domain_index[i,:],:].mean(axis=0) for i in range(n_spot)],dtype=np.float32)
             expr_spatial_neighbor = (old_weightage * expr_spatial_neighbor) + (nei_weightage * expr_micro_env)
         return expr_spatial_neighbor
     
     
     def __spatial_integration__(self,simu_arr,real_arr,x_cor,y_cor,n_neighbor =40,n_itr=3):
-        simu_arr_norm,real_arr_norm = self.__normalisation1__(simu_arr),self.__normalisation1__(real_arr)
-        n_spot,n_gene = real_arr_norm.shape
-        domain_index = self.__domain_neighbor_index__(real_arr_norm, x_cor, y_cor,n_neighbor =n_neighbor)
-        std_scale = StandardScaler()
-        real_arr_norm_std = std_scale.fit_transform(real_arr_norm)
-        simu_arr_norm_std = std_scale.fit_transform(simu_arr_norm)
-        real_exp_spatial = self.__domain_inspired__(real_arr_norm, domain_index,n_itr=n_itr )
-        ridge_cv = RidgeCV(alphas=[1,10,25,50,100,500,1000,5000])
-        chunk_st, chunk_sc = self.__chunk_df__(real_arr_norm_std,real_exp_spatial,5000)
-        ridge_cv.fit(chunk_st, chunk_sc)
-        print(ridge_cv.alpha_)
-        ridge_model = Ridge(alpha=ridge_cv.alpha_)
-        ridge_model.fit(real_arr_norm_std,real_exp_spatial)
-        simu_exp_spatial = ridge_model.predict(simu_arr_norm_std)
-        
-        
-
-        simu_exp_spatial[simu_exp_spatial<0]=0
-        
-        real_nei_arr = np.hstack([real_arr_norm,real_exp_spatial])
-        simu_nei_arr = np.hstack([simu_arr_norm,simu_exp_spatial])
-        
-        
+        with alive_bar(5,title="Capturing spatial microenvironment relation:") as bar:
+            simu_arr_norm,real_arr_norm = self.__normalisation1__(simu_arr),self.__normalisation1__(real_arr)
+            n_spot,n_gene = real_arr_norm.shape
+            domain_index = self.__domain_neighbor_index__(real_arr_norm, x_cor, y_cor,n_neighbor =n_neighbor)
+            std_scale = StandardScaler()
+            bar()
+            real_arr_norm_std = std_scale.fit_transform(real_arr_norm)
+            simu_arr_norm_std = std_scale.fit_transform(simu_arr_norm)
+            bar()
+            real_exp_spatial = self.__domain_inspired__(real_arr_norm, domain_index,n_itr=n_itr )
+            ridge_cv = RidgeCV(alphas=[1,10,25,50,100,500,1000,5000])
+            bar()
+            chunk_st, chunk_sc = self.__chunk_df__(real_arr_norm_std,real_exp_spatial,5000)
+            ridge_cv.fit(chunk_st, chunk_sc)
+            ridge_model = Ridge(alpha=ridge_cv.alpha_)
+            bar()
+            ridge_model.fit(real_arr_norm_std,real_exp_spatial)
+            simu_exp_spatial = ridge_model.predict(simu_arr_norm_std)
+            simu_exp_spatial[simu_exp_spatial<0]=0            
+            real_nei_arr = np.hstack([real_arr_norm,real_exp_spatial])
+            simu_nei_arr = np.hstack([simu_arr_norm,simu_exp_spatial])
+            bar()   
         return real_nei_arr,simu_nei_arr
-            
-        
-        
 
     def __fit_predict__(self,real_st,simu_st,simu_prop,return_prop = True):
         
         """
         Predict the cell type proportations from the Spatial data 
         
         Parameters
         ----------------------------------------------------------------------
         st_data : st_data output from the preprocessing function 
         return_low_exp_celltypes  : low expressed cell proportions needed or not
         cell_prop_threshold : Threshold for low expression celltype
             
         """
-        with alive_bar(5,title="Fitting Domain Adapt Model :") as bar:
+        with alive_bar(5,title="Spot Denvolution:") as bar:
             simu_st_norm = self.__normalisation2__(simu_st)
             real_st_norm = self.__normalisation2__(real_st)
-            # bar()
+            bar()
       
             model = KNeighborsRegressor(n_neighbors=250)
             bar()
             # print(best_alpha)
             model.fit(simu_st_norm,simu_prop)
             bar()
             predict = model.predict(np.array(real_st_norm))
@@ -384,14 +379,16 @@
                 thres = threshold - 0.10
                 clus_deconvo_major = clus_deconvo[clus_deconvo>thres]
             dicti_annot[i] = ' / '.join(list(clus_deconvo_major.index))
             if len(clus_deconvo_major)==0:
                 dicti_annot[i] = "ambiguous"
         mod_cluster_annot = pd.Categorical([dicti_annot[i]for i in cluster_annot])
         return dicti_annot,mod_cluster_annot
+    
+
 #%% 
 class SpatialCluster:
     def __init__(self):
         pass
     def __hvg_detect__(self,df_array,N=1000):
         df_array = np.array(df_array)
         st_vars = df_array.var(axis=0)
@@ -403,15 +400,15 @@
         # std = StandardScaler()
         std = MinMaxScaler()
         pca =   TruncatedSVD(n_components=50)
         st_df_graph_std = std.fit_transform(df)
         st_df_graph_pca = pca.fit_transform(st_df_graph_std)
         if n_clus=="auto":
             n_clus = self.__auto_k_find__(st_df_graph_pca)
-        kmean = KMeans(n_clusters=n_clus)
+        kmean = KMeans(n_clusters=n_clus,n_init=20)
         kmean.fit(st_df_graph_pca)
         labels = np.array(kmean.labels_)
         return labels
     
     def __auto_k_find__(self,data):
         n_row,_ = data.shape
         random_row = np.random.choice(n_row,5000)
@@ -447,8 +444,8 @@
             bar()
             cluster_assignment = self.__kmean_clus__(st_array_hvg_norm_domain,n_clus = n_cluster)
             cluster_assignment = pd.Categorical(cluster_assignment)
             bar()
         t2 = time.time()
         print(f"Executed in {t2-t1} second")
         
-        return cluster_assignment
+        return cluster_assignment
```


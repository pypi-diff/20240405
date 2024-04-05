# Comparing `tmp/ScoreDrivenBOCPD-0.1.6-py3-none-any.whl.zip` & `tmp/ScoreDrivenBOCPD-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8791 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-02 19:53 ScoreDrivenBOCPD/__init__.py
--rw-rw-rw-  2.0 fat     2072 b- defN 24-Apr-02 11:33 ScoreDrivenBOCPD/data.py
--rw-rw-rw-  2.0 fat     6486 b- defN 24-Apr-02 15:31 ScoreDrivenBOCPD/prob_model.py
+Zip file size: 8758 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-03 14:55 ScoreDrivenBOCPD/__init__.py
+-rw-rw-rw-  2.0 fat     2156 b- defN 24-Apr-05 08:39 ScoreDrivenBOCPD/data.py
+-rw-rw-rw-  2.0 fat     6417 b- defN 24-Apr-05 08:54 ScoreDrivenBOCPD/prob_model.py
 -rw-rw-rw-  2.0 fat     2273 b- defN 24-Mar-22 06:47 ScoreDrivenBOCPD/sd_ar.py
--rw-rw-rw-  2.0 fat     7873 b- defN 24-Apr-02 15:31 ScoreDrivenBOCPD/sd_bocpd.py
--rw-rw-rw-  2.0 fat     1093 b- defN 24-Apr-02 21:19 ScoreDrivenBOCPD-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      382 b- defN 24-Apr-02 21:19 ScoreDrivenBOCPD-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 21:19 ScoreDrivenBOCPD-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-02 21:19 ScoreDrivenBOCPD-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      848 b- defN 24-Apr-02 21:19 ScoreDrivenBOCPD-0.1.6.dist-info/RECORD
-10 files, 21170 bytes uncompressed, 7331 bytes compressed:  65.4%
+-rw-rw-rw-  2.0 fat     7711 b- defN 24-Apr-05 08:27 ScoreDrivenBOCPD/sd_bocpd.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      382 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      848 b- defN 24-Apr-05 09:13 ScoreDrivenBOCPD-0.1.7.dist-info/RECORD
+10 files, 21023 bytes uncompressed, 7298 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: ScoreDrivenBOCPD/sd_ar.py
 Comment: 
 
 Filename: ScoreDrivenBOCPD/sd_bocpd.py
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.6.dist-info/LICENSE
+Filename: ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.6.dist-info/METADATA
+Filename: ScoreDrivenBOCPD-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.6.dist-info/WHEEL
+Filename: ScoreDrivenBOCPD-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.6.dist-info/top_level.txt
+Filename: ScoreDrivenBOCPD-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ScoreDrivenBOCPD-0.1.6.dist-info/RECORD
+Filename: ScoreDrivenBOCPD-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScoreDrivenBOCPD/data.py

```diff
@@ -6,66 +6,69 @@
     def __init__(self,bern_p,mean0,var0):
         
         self.bern_p = bern_p
         self.mean0  = mean0
         self.var0   = var0
         
     
-    def __bernoulli(self):
+    def bernoulli(self):
         
         if np.random.random() < self.bern_p:
             
             return True
         
         
-    def __gaussian(self):
-        
+    def gaussian(self):
+
         return np.random.normal(self.mean0, self.var0)
 
 
 class Data(Priors):
     
     def __init__(self, bern_p=1/100,mean0=1,var0=3, file_name = "_",data_type =  "real"):
         super().__init__(bern_p,mean0,var0)
         
+        if data_type == "real" and file_name == "_":
+            raise ValueError("When the data_type is \"real\" you should also provide the file_name")
+        
         self.data_type = data_type
         self.file_name = file_name
-        self.data      = []
-        self.cps       = []
         
     
     def update_data(self):
         
         if self.data_type == "sim":
             
             return self.__sim_data()
         
         if self.data_type == "real":
             
             return self.__real_data()
         
     
     def __sim_data(self,var = 1, rho = 0.3, T = 500):
-
-        mean = super().__gaussian()
-        self.data.append(np.random.normal(mean,var))
+        data = []
+        cps = []
+        mean = super().gaussian()
+        data.append(np.random.normal(mean,var))
         
-        for t in range(1,self.T): 
-            
-            if super().__bernoulli():
+        for t in range(1,T): 
+
+            if super().bernoulli():
+
+                mean = super().gaussian()
                 
-                mean = super().__gaussian()
-                self.cps.append(t)
-                self.data.append(np.random.normal(mean,var))
+                cps.append(t)
+                data.append(np.random.normal(mean,var))
                 
                 continue
             
-            self.data.append(np.random.normal(mean+rho*(self.data[t-1]-mean),var*(1-rho**2)))
+            data.append(np.random.normal(mean+rho*(data[t-1]-mean),var*(1-rho**2)))
         
-        return self.data
+        return data,cps
     
     
     def __real_data(self):
 
         data_df = pd.read_csv(self.file_name,delimiter =',',header = 0)
         data = list(data_df[data_df.columns[0]])
```

## ScoreDrivenBOCPD/prob_model.py

```diff
@@ -8,21 +8,19 @@
 by Tsaknaki,Lillo,Mazzarisi, 2023
 
 see: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4500960 
 """
 import numpy as np
 from   scipy.stats import norm
 import sd_ar as sd
-# import warnings
-# warnings.filterwarnings('ignore')
 
 
 class GaussianModel:
     
-    def __init__(self, mean0, var0, varx, init_cor, init_var, init_theta,q):
+    def __init__(self, mean0, var0, varx, init_theta, q, init_cor = 0):
         
         varx = 1e-8 + varx
         var0 = 1e-8 + var0
         
         if varx < 0:
             raise ValueError("The variance should be zero or positive")
             
@@ -38,15 +36,15 @@
         if (q == 1/2 or q == 1) and init_cor == 0:
             raise ValueError("For this model the correlation should live in the set [-0.9,0.9]\{0}")
         
         if q == 0:
             init_cor = 0
            
         self.parameters        = init_theta
-        self.init_var          = init_var
+        self.init_var          = varx
         self.init_cor          = init_cor
         self.cor               = init_cor
         self.mean0             = mean0
         self.var0              = var0
         self.varx              = varx
         self.var_vector        = np.array([varx])
         self.cor_vector        = np.array([0])
@@ -170,9 +168,8 @@
 
 
     @property 
     def mean_dep_params(self):
         """Helper function for computing the posterior mean.
         """         
         return (1-self.cor_vector)*self.mean_params + (self.cor_vector)*self.prev_element
-            
-
+
```

## ScoreDrivenBOCPD/sd_bocpd.py

```diff
@@ -18,31 +18,28 @@
 
 Author: Yvonni Tsaknaki
 """
 import matplotlib.pyplot as plt
 from   matplotlib.colors import LogNorm
 import numpy as np
 from   scipy.special import logsumexp
-# import warnings
-# warnings.filterwarnings('ignore')
-
 
 class SDBocpd:
     
     def __init__(self, T, d, q):
         
         self.T       = T
         self.d       = d
         self.q       = q
         self.ml_path = np.ones(self.T+1)
         self.ml_cps  = [0]
         self.run_length_mtx = -np.inf * np.ones((self.T+1, self.T+1))
     
     
-    def bocpd(self,data, model, hazard, plot = True):
+    def bocpd(self,data, model, hazard, true_cps = [], plot = True):
         """This function implements Algorithm 1 from: "Bayesian Online Changepoint Detection" 
             by R.P.Adams and D.J.C.MacKay. 
         """
         
         if self.d != 0 and self.d != 1/2:
             raise ValueError("d should be either 0 or 1/2") 
     
@@ -121,33 +118,30 @@
             self.ml_path[t-1] = self.T-position_max_element[0][0]
         
         position_max_element = np.where(log_run_length[self.T, :self.T+1] == np.amax(log_run_length[self.T, :self.T+1]))
         self.ml_path[self.T] = self.T-position_max_element[0][0]
         
         self.run_length_mtx = np.exp(log_run_length)
         
-        # mse_bo = mean_squared_error(data[2:],pmean[2:])
-        # print('MSE of model:',mse_bo/statistics.stdev(data[2:])**2)
-        
         if plot == True:
             
-            self.__plt_run_length_posterior(data, pmean, pvar)
+            self.__plt_run_length_posterior(data, true_cps, pmean, pvar)
             
         return self.run_length_mtx, self.ml_cps
     
     
     def SubtrckToList(self,lista,number):
         new_lista = []
         for i in lista:
             new_lista.append(i-number)
         return new_lista
     
         
-    def __plt_run_length_posterior(self, data, pmean, pvar): 
-        
+    def __plt_run_length_posterior(self, data, true_cps, pmean, pvar): 
+
         fig, axes = plt.subplots(2, 1, figsize=(16,8))
         plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=0.3, hspace=0.4)
     
         ax1, ax2 = axes
         
         ax1.scatter(range(1, self.T+1), data)
         ax1.plot(range(1, self.T+1), data)
@@ -157,33 +151,34 @@
         ax1.plot(range(1, self.T+1), pmean + _2std, c='black', ls='--')
         ax1.set_title("Real Data",fontsize=25)
         line2, = ax1.plot(range(1, self.T+1), pmean, c='black',linewidth=1,ls='-')
         ax1.legend([line1,line2],['pvar','pmean'],fontsize="19")
         ax1.tick_params(labelsize=22)
         ax1.set_ylabel(r'$x_t$',fontsize=26)
         ax1.margins(0)
-        
+
         im = ax2.imshow(np.rot90(self.run_length_mtx,k=1), aspect='auto', cmap='gray_r',norm=LogNorm(vmin=0.0001, vmax=1))
         cax = fig.add_axes([1.0, 0.07, 0.018, 0.4])
         fig.colorbar(im, cax=cax, orientation='vertical')
         line3, = ax2.plot(self.ml_path,color='red',linewidth=2)
-        ticks = list(range(self.T, int(self.T/2), -20))
-        tick_labels = list(range(0, int(self.T/2), 20))
-        ax2.set_ylim([self.T,int(self.T/2)])
+        
+        ticks = list(range(self.T, int(min(self.ml_path)), -int(self.T/4)))
+        tick_labels = list(range(0, self.T-int(min(self.ml_path)), int((self.T)/4)))
+        ax2.set_ylim([self.T,int(min(self.ml_path))])
+        
         ax2.set_yticks(ticks)
         ax2.set_yticklabels(tick_labels,fontsize=22)
         ax2.legend([line3], ['most likely path'],fontsize="19")
         ax2.tick_params(labelsize=22)
         ax2.set_ylabel(r'$r_t$',fontsize=26)
         ax2.set_title('Run Length Posterior of MBOC',fontsize=25)
         ax2.margins(0)
         
-        for cp_f in self.ml_cps:
+        for cp_f in true_cps:
             ax1.axvline(cp_f, c='red', ls='dotted',lw=2)
-            ax2.axvline(cp_f, c='red', ls='dotted',lw=2)
     
         plt.tight_layout()
         
  
 class Hazard:
     
     def __init__(self,T,hazard,constant = True):
```

## Comparing `ScoreDrivenBOCPD-0.1.6.dist-info/LICENSE` & `ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ScoreDrivenBOCPD-0.1.6.dist-info/RECORD` & `ScoreDrivenBOCPD-0.1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ScoreDrivenBOCPD/__init__.py,sha256=MHuUwF05F2TPiYu5QDp2yIpuRqw07SBGQyC5Qp05dgE,34
-ScoreDrivenBOCPD/data.py,sha256=Oauh99C0zZxziVRwCWN_IzJ7aPzUcD3pKVG1odkK-2g,2072
-ScoreDrivenBOCPD/prob_model.py,sha256=n8eq28bEzmitXmIxAFo6mU7N15ubnjXU4kCtu7HkUmA,6486
+ScoreDrivenBOCPD/data.py,sha256=CC5FxsuzDF7v-UxBmYJVn7BpFktpwX2N8bglPu5oZVw,2156
+ScoreDrivenBOCPD/prob_model.py,sha256=mTPkmViq-RcEojKjnhMO5qUXFuHV7jiUK2mnNV5Hwoo,6417
 ScoreDrivenBOCPD/sd_ar.py,sha256=qPVxciaaahB7rC4FF5xcrkG9iiXQPptaYS-Wb5t25ek,2273
-ScoreDrivenBOCPD/sd_bocpd.py,sha256=PTfWAIKRf49DVH5FsjqvrchUz7CiUyuXYevQJAHfqys,7873
-ScoreDrivenBOCPD-0.1.6.dist-info/LICENSE,sha256=tqaU2RKeRvOViWELR1Jc-XujDbQku657gN6LbIw1mvw,1093
-ScoreDrivenBOCPD-0.1.6.dist-info/METADATA,sha256=kVrLPK2vJK508fIXCWVG3sgKYUMk1a_dMdu7SnwuDN4,382
-ScoreDrivenBOCPD-0.1.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-ScoreDrivenBOCPD-0.1.6.dist-info/top_level.txt,sha256=z4HtCrg_hwaOBm6rmY9ylxXWRWZ5qgIpcepyEqtpPGQ,17
-ScoreDrivenBOCPD-0.1.6.dist-info/RECORD,,
+ScoreDrivenBOCPD/sd_bocpd.py,sha256=xTp7rm5DWTE9x_RoS2NAMJO0iv3UzoFUCXQpoqLGeYE,7711
+ScoreDrivenBOCPD-0.1.7.dist-info/LICENSE,sha256=tqaU2RKeRvOViWELR1Jc-XujDbQku657gN6LbIw1mvw,1093
+ScoreDrivenBOCPD-0.1.7.dist-info/METADATA,sha256=BFWsErtqtUurDgP5aqg0ZRjcrzEvrqFJ7jXs5X_T9FU,382
+ScoreDrivenBOCPD-0.1.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+ScoreDrivenBOCPD-0.1.7.dist-info/top_level.txt,sha256=z4HtCrg_hwaOBm6rmY9ylxXWRWZ5qgIpcepyEqtpPGQ,17
+ScoreDrivenBOCPD-0.1.7.dist-info/RECORD,,
```


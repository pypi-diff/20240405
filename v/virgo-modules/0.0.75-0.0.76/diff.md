# Comparing `tmp/virgo_modules-0.0.75.tar.gz` & `tmp/virgo_modules-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.75.tar", last modified: Tue Apr  2 07:09:17 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.76.tar", last modified: Fri Apr  5 14:59:35 2024, max compression
```

## Comparing `virgo_modules-0.0.75.tar` & `virgo_modules-0.0.76.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:09:17.250752 virgo_modules-0.0.75/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.75/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-02 07:09:17.248753 virgo_modules-0.0.75/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.75/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 07:09:17.255757 virgo_modules-0.0.75/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-02 07:08:25.000000 virgo_modules-0.0.75/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:09:16.937079 virgo_modules-0.0.75/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-02 07:09:17.100756 virgo_modules-0.0.75/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:09:17.244755 virgo_modules-0.0.75/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     1383 2024-03-05 19:39:06.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0     7691 2024-03-03 08:13:30.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    53096 2024-03-29 14:10:19.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   105164 2024-04-02 07:08:25.000000 virgo_modules-0.0.75/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:09:17.182752 virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-02 07:09:15.000000 virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-02 07:09:16.000000 virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:09:15.000000 virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-02 07:09:15.000000 virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-02 07:09:15.000000 virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.871625 virgo_modules-0.0.76/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.76/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-04-05 14:59:35.869624 virgo_modules-0.0.76/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.76/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:59:35.872624 virgo_modules-0.0.76/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-05 14:59:05.000000 virgo_modules-0.0.76/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.780584 virgo_modules-0.0.76/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.802730 virgo_modules-0.0.76/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.863631 virgo_modules-0.0.76/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    64053 2024-04-04 18:20:37.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   142521 2024-04-03 15:42:01.000000 virgo_modules-0.0.76/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:59:35.824246 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 14:59:35.000000 virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.75/LICENSE` & `virgo_modules-0.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.75/PKG-INFO` & `virgo_modules-0.0.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.75
+Version: 0.0.76
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.75/setup.py` & `virgo_modules-0.0.76/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.75",
+    version="0.0.76",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.75/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.76/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,32 +2,64 @@
 import boto3
 from pathlib import Path
 from io import StringIO, BytesIO
 import pandas as pd
 
 
 def upload_file_to_aws(bucket,key,input_path, aws_credentials):
-    
+    '''
+    upload file from a folder to an s3 folder
+
+            Parameters:
+                    bucket (str): bucket name
+                    key (str): key pattern or folder in s3 e.g. path/to/upload/
+                    input_path (str): input path of the file to upload e.g. path/to/upload.txt
+                    aws_credentials (dict): aws credentials dictionary
+                    
+            Returns:
+                    None
+    '''
     session = boto3.Session(aws_access_key_id=aws_credentials['AWS_ACCESS_KEY_ID'],aws_secret_access_key=aws_credentials['AWS_SECRET_ACCESS_KEY'])
     bucket = aws_credentials[bucket]
     s3 = session.resource('s3')
     s3.meta.client.upload_file(Filename=input_path , Bucket=bucket, Key=key)
 
 def upload_pandas_to_s3(data_frame,bucket,key, aws_credentials):
+    '''
+    upload dataframe as csv to an s3 folder
 
+            Parameters:
+                    data_frame (pd.DataFrame): data
+                    bucket (str): bucket name
+                    key (str): key pattern or folder in s3 e.g. path/to/upload/
+                    aws_credentials (dict): aws credentials dictionary
+                    
+            Returns:
+                    None
+    '''
     csv_buffer = StringIO()
     data_frame.to_csv(csv_buffer)
     csv_buffer.seek(0)
 
     s3 = boto3.client("s3",region_name=aws_credentials['AWS_DEFAULT_REGION'],aws_access_key_id=aws_credentials['AWS_ACCESS_KEY_ID'],aws_secret_access_key=aws_credentials['AWS_SECRET_ACCESS_KEY'])
     bucket = aws_credentials[bucket]
     s3.put_object(Bucket=bucket, Body=csv_buffer.getvalue(), Key= key)
 
 def download_file_to_aws(bucket,key, aws_credentials):
-    
+    '''
+    download csv file from s3 folder
+
+            Parameters:
+                    bucket (str): bucket name
+                    key (str): key pattern or folder in s3 e.g. path/to/download/file.csv
+                    aws_credentials (dict): aws credentials dictionary
+                    
+            Returns:
+                    None
+    '''
     s3c = boto3.client(
             's3', 
             region_name = aws_credentials['AWS_DEFAULT_REGION'],
             aws_access_key_id = aws_credentials['AWS_ACCESS_KEY_ID'],
             aws_secret_access_key = aws_credentials['AWS_SECRET_ACCESS_KEY']
         )
     obj = s3c.get_object(Bucket= bucket , Key = key)
```

### Comparing `virgo_modules-0.0.75/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.76/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.75/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.76/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,38 +27,98 @@
 
 import mlflow
 
 from pykalman import KalmanFilter
 from .aws_utils import upload_file_to_aws
 
 def calculate_cointegration(series_1, series_2):
+    '''
+    calculate cointegration score of two time series.
+
+            Parameters:
+                    series_1 (pd.series): pandas series of the asset returns
+                    series_2 (pd.series): pandas series of the asset returns
+
+            Returns:
+                    coint_flag (int): cointegration flag, 1 or 0. 1 if p value and coint_t lower than 0.05 and critical value
+                    hedge_value (float): hedge value
+    '''
+
     coint_flag = 0
     coint_res = coint(series_1, series_2)
     coint_t = coint_res[0]
     p_value = coint_res[1]
     critical_value = coint_res[2][1]
     
     model = sm.OLS(series_1, series_2).fit()
     hedge_value = model.params[0]
     coint_flag = 1 if p_value < 0.05 and coint_t < critical_value else 0
     
     return coint_flag, hedge_value
 
 class pair_finder():
+    """
+    class that is going assess two assets to evaluate whether both are cointegrated
+
+    Attributes
+    ----------
+    df  : pd.DataFrame
+        dataframe of merged assets with spread score
+    asset_1 : str
+        asset to assess
+    asset_2 : str
+        secondary asset to assess
+
+    Methods
+    -------
+    produce_zscore(window=int, z_threshold=float, verbose=boolean):
+        producing z score from the spread. Also getting signals using window functions
+    plot_scores():
+        display plot of the time series and signals and other plot for pair signal strategy
+    evaluate_signal(days_list=list(),test_size=int, signal_position=int,threshold=float,verbose=boolean, plot=boolean):
+        evaluate the signal strategy using future returns
+    create_backtest_signal(days_strategy=int, test_size=int):
+        create back test of the strategy and get somo plot analysis
+    """
     def __init__(self, raw_data , asset_1 ,asset_2):
-        
+        """
+        Initialize object, selecting just the two assets and getting the spread between both assets
+
+        Parameters
+        ----------
+        raw_data (pd.DataFrame): dataframe of all assets
+        asset_1 (str): asset to assess
+        asset_2 (str): secondary asset to assess
+
+        Returns
+        -------
+        None
+        """
         df = raw_data[[asset_1, asset_2]]
         coint_flag, hedge_ratio = calculate_cointegration(df[asset_1], df[asset_2])
         spread = df[asset_1] - (hedge_ratio * df[asset_2])
         df['spread'] = spread
         self.df = df
         self.asset_1 = asset_1
         self.asset_2 = asset_2
         
     def produce_zscore(self, window, z_threshold, verbose = False):
+        """
+        producing z score from the spread. Also getting signals using window functions
+
+        Parameters
+        ----------
+        window (int): window size
+        z_threshold (float): alpha and z threhold for the normalized feature
+        verbose (boolean): to print analysis
+
+        Returns
+        -------
+        None
+        """
         self.z_threshold = z_threshold
         spread_series = pd.Series(self.df.spread)
         mean = spread_series.rolling(center = False, window = window).mean()
         std = spread_series.rolling(center = False, window = window).std()
         x = spread_series.rolling(center=False, window =  1).mean()
         z_score = (x - mean)/std
 
@@ -70,15 +130,25 @@
         up_signal = np.where(z_score >= z_threshold,1,0)
         low_signal = np.where(z_score <= -z_threshold,1,0)
 
         self.df['up_pair_signal'] = up_signal
         self.df['low_pair_signal'] = low_signal
         
     def plot_scores(self):
-        
+        """
+        display plot of the time series and signals and other plot for pair signal strategy
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         plt.axhline(y=0.0, color='grey', linestyle='--')
         plt.figure(1, figsize = (10, 4))
         plt.plot(self.df.spread.values)
         plt.show()
         print('-----------------------------------------------------------------')
         plt.figure(1,figsize = (10,4))
         plt.axhline(y=self.z_threshold, color='r', linestyle='--')
@@ -100,15 +170,30 @@
         fig.add_trace(go.Scatter(name = 'up_signal',x=self.df.index, y=np.where(self.df['up_pair_signal'] == 1, asset_2_values, np.nan), mode='markers',marker=dict(color='green')))
         fig.add_trace(go.Scatter(name = 'low_signal',x=self.df.index, y=np.where(self.df['low_pair_signal'] == 1, asset_2_values, np.nan), mode='markers',marker=dict(color='red')))
         fig.update_layout(height=500, width=1200)
 
         fig.show()
         
     def evaluate_signal(self, days_list,test_size, signal_position = False,threshold = 0.05,verbose = False, plot = False):
-    
+        """
+        evaluate the signal strategy using future returns 
+
+        Parameters
+        ----------
+        days_list (list): list of days future returns
+        test_size (int): teste data size, the remainng is taken as training data
+        signal_position (int): position of the signal to open position
+        threshold (float): alpha or z threshold of the normalized feature
+        verbose (boolean): if True, print results
+        plot (boolean): if true, display plots
+
+        Returns
+        -------
+        None
+        """
         df = self.df.sort_values('Date').iloc[0:-test_size,:].copy()
         returns_list = list()
         
         for days in days_list:
 
             feature_ = f'return_{days}d'
             df[feature_] = (df[self.asset_1].shift(-days)/df[self.asset_1]-1)*100
@@ -202,14 +287,26 @@
             axs[2].axhline(y=0, color='grey', linestyle='--')
             axs[2].set_title('signal type expected returns distribution at different time lapses')
             plt.show()
             
         del df
         
     def create_backtest_signal(self,days_strategy, test_size):
+        """
+        create back test of the strategy and get somo plot analysis
+
+        Parameters
+        ----------
+        days_strategy (int): list of days future returns
+        test_size (int): teste data size, the remainng is taken as training data
+        
+        Returns
+        -------
+        None
+        """
         asset_1 = self.asset_1
         df1 = self.df.iloc[-test_size:,:].copy()
         df2 = df1.copy()
         df2['signal_type'] = np.where(
                     df2['up_pair_signal'] == 1, 
                     'up', 
                     np.where(
@@ -269,15 +366,26 @@
         plt.legend()
         plt.title('strategy and cumulative returns based on signal strategy')
         plt.plot()
 
         del df1,df2,dft
         
 def produce_big_dataset(data_frames, stocks_codes_, feature_list, limit = 500):
-    
+    '''
+    combine multiple asset, taking a common schema
+
+            Parameters:
+                    data_frames (pd.DataFrame): Base dataframe
+                    stocks_codes_ (list): assets to select
+                    feature_list (list): feature list
+                    limit (int): number of observation per asset
+
+            Returns:
+                    dataframe (pd.DataFrame): Base dataframe with extra data
+    '''
     feature_list_ = list()
     columns_vector = list(data_frames[stocks_codes_[-1]].columns )
     for feat in feature_list:
         feature_list_.append(feat)
         items = [featx for featx in [f'norm_{feat}', f'z_{feat}'] if featx in columns_vector]
         if len(items) > 0:
             feature_list_.append(items[0])
@@ -297,15 +405,27 @@
         df = df[features_list].sort_values('Date').iloc[-limit:,:]
         df['Ticket'] = ticket
         list_df.append(df)
     dataframe = pd.concat(list_df)
     return dataframe
 
 def ranking(data, weighted_features, top = 5, window = 5):
-    
+    '''
+    Create a ranking of assets given current signals and weighted average importance
+
+            Parameters:
+                    data (pd.Dataframe): base data
+                    weighted_features (dict): configuration dictionary
+                    top (int): top n to get result
+                    window (int): number of days to assess
+
+            Returns:
+                    top_up (list): top roof signal asset
+                    top_low (list): top botton signal asset
+    '''
     features = weighted_features.keys()
     up_columns = ['signal_up_' + x for x in features]
     low_columns = ['signal_low_' + x for x in features]
     
     ticket_list= list(data.Ticket.unique())
     result = dict()
     for ticket in ticket_list:
@@ -332,24 +452,31 @@
     
     top_up = list(df.sort_values('up_signas', ascending = False).index)[:top]
     top_low = list(df.sort_values('low_signas', ascending = False).index)[:top]
     
     return top_up, top_low
 
 def produce_dashboard(data, columns , ticket_list, show_plot = True, nrows = 150,save_name = False, save_path = False, save_aws = False, aws_credential = False):
-    """
-    data: pandas df
-    columns: list 
-    ticket_list: list asset list
-    nrows: int
-    show_plot: bool
-    save_path: str local path for saving e.g r'C:/path/to/the/file/'
-    save_aws: str remote key in s3 bucket path e.g. 'path/to/file/'
-    aws_credentials: dict
-    """
+    '''
+    produce dashboard using signals and list of assets
+
+            Parameters:
+                    data (pd.Dataframe): base data
+                    columns (list): list of features or signals 
+                    ticket_list (list): list of assets
+                    show_plot (boolean): if true, display plot
+                    nrows (int): number of days back to display
+                    save_name (str): dashboad name resulting file
+                    save_path (str): local path for saving e.g r'C:/path/to/the/file/'
+                    save_aws (str): remote key in s3 bucket path e.g. 'path/to/file/'
+                    aws_credential (dict): aws credentials
+
+            Returns:
+                    None
+    '''
     top = len(ticket_list)
     columns = ['history'] + columns
     subtitles = list()
     
     for ticket in ticket_list:
         for col in columns:
             subtitles.append(ticket + ': ' + col)
@@ -391,15 +518,25 @@
         
     if save_name and save_path and save_aws:
         # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'multi_dashboards/'+save_name+'.json',input_path = save_path+save_name+'.json')
         upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = save_aws + save_name + '.json', input_path = save_path + save_name + '.json', aws_credentials = aws_credential)
         
 
 def rank_by_return(data, lag_days, top_n = 5):
-    
+    '''
+    produce ranking  by returns
+
+            Parameters:
+                    data (pd.Dataframe): base data
+                    lag_days (int): number of days to consider
+                    top_n (int): top n results assets
+
+            Returns:
+                    result (list): resulting assets top n most important
+    '''
     data = data.sort_values(['Ticket','Date'], ascending=[False,False]).reset_index(drop = True)
     data['first'] = data.sort_values(['Date'], ascending=[False]).groupby(['Ticket']).cumcount() + 1
     data =  data[data['first'] <= lag_days]
     
     data = data.sort_values(['Ticket','Date'], ascending=[False,False]).reset_index(drop = True)
     data['last'] = data.sort_values(['Date'], ascending=[True]).groupby(['Ticket']).cumcount() + 1
     
@@ -412,26 +549,27 @@
     data = data.iloc[:top_n,:]
     
     result = list(data.Ticket.values)
     
     return result
 
 def get_data(ticker_name:str, ticket_settings:dict, n_days:int = False, hmm_available: object = False, data_window:str = '5y') -> object:
-    """
-    this functions runs the stock_eda_panel
-    it is shared between train model and predictions
-    arguments:
-    hmm_available: if the hmm is available, in prediction is required
-    ticker_name: name of the asset
-    ticket_settings: dictionary with all the parameters to compute features
-    n_days: to set an arbitrary data size
-
-    returns: stock eda panel
-    """
+    '''
+    this functions runs the stock_eda_panel. It is shared between train model and predictions
 
+            Parameters:
+                    ticker_name (str): name of the asset
+                    ticket_settings (dict): dictionary with all the parameters to compute features
+                    n_days (int): to set an arbitrary data size
+                    hmm_available (obj): if the hmm is available, in prediction is required
+                    data_window (str): window for the data extraction
+
+            Returns:
+                    object_stock (obj): resulting object_stock object
+    '''
     object_stock = stock_eda_panel(ticker_name , n_days, data_window)
     object_stock.get_data()
 
     # computing features if they exists in the ticketr settings
 
     if 'volatility' in ticket_settings['settings']:
         parameters = ticket_settings['settings']['volatility']
@@ -520,29 +658,46 @@
                                             seed = ticket_settings['settings']['hmm']['seed'])
     
     return object_stock
 
 trends = {'adjusted' : 0.001, 'smooth' : 0.0001}
 
 def apply_KF(self, trends):
+    '''
+    create kalman filter feature and attach it to the stock_eda_panel object
+
+            Parameters:
+                    trends (dict): configurations of the kalman filter
+            Returns:
+                    none
+    '''
     for ttrend in trends:
         tcov = trends.get(ttrend)
         kf = KalmanFilter(transition_matrices = [1],
                              observation_matrices = [1],
                              initial_state_mean = 0,
                              initial_state_covariance = 1,
                              observation_covariance=1,
                              transition_covariance=tcov)
         vector = kf.filter(self.df[['Close']])[0]
         self.df[f'KalmanFilter_{ttrend}'] = vector.reshape((vector.shape[0]))
         
 stock_eda_panel.apply_KF = apply_KF
 
 def call_ml_objects(stock_code, client, call_models = False):
-    
+    '''
+    call artifcats from mlflow
+
+            Parameters:
+                    stock_code (str): asset name
+                    client (obj): mlflow client
+                    call_models (boolean): if true, call ml artifacts
+            Returns:
+                    objects (dict): that contains ml artifacts, data , configs and models
+    '''
     objects = dict()
     
     registered_model_name = f'{stock_code}_models'
     latest_version_info = client.get_latest_versions(registered_model_name, stages=["Production"])
     latest_production_version = latest_version_info[0].version
     run_id_prod_model = latest_version_info[0].run_id
     
@@ -580,36 +735,88 @@
     
     objects['called_ticket_settings'] = ticket_settings
     objects['called_data_frame'] = object_stock.df
     
     return objects
 
 class produce_plotly_plots:
+    """
+    class that helps to produce different dashboards
+
+    Attributes
+    ----------
+    ticket_name : str
+        asset name
+    data_frame (pd.DataFrame): asset data
+    settings : dict
+        asset configurations
+    show_plot : boolean
+        if true, display plots
+    save_path : str
+        local path for saving e.g r'C:/path/to/the/file/'
+    save_aws : str
+        remote key in s3 bucket path e.g. 'path/to/file/'
+    aws_credentials : dict
+        aws credentials
+    return_figs : boolean
+        if true, methods will return objects
+
+    Methods
+    -------
+    plot_asset_signals(feature_list=list, spread_column=list, date_intervals=list):
+        Display signals and hmm states over closing prices and feature time series
+    explore_states_ts():
+        display scaled time series of every hmm state
+    plot_hmm_analysis(settings=dict, t_matrix=txt, model=obj):
+        display plots that analyse hmm states
+    produce_forecasting_plot(predictions=pd.DataFrame):
+        display forecasting plots
+    """
     def __init__(self,ticket_name, data_frame,settings, save_path = False, save_aws = False, show_plot= True, aws_credentials = False, return_figs = False):
         """
-        ticket_name: str asset name
-        data_frame: pandas df
-        settings: dict
-        show_plot: bool
-        save_path: str local path for saving e.g r'C:/path/to/the/file/'
-        save_aws: str remote key in s3 bucket path e.g. 'path/to/file/'
-        aws_credentials: dict
+        Initialize object
+
+        Parameters
+        ----------
+        ticket_name (str): asset name
+        data_frame (pd.DataFrame): asset data
+        settings (dict): asset configurations
+        show_plot (boolean): if true, display plots
+        save_path (str): local path for saving e.g r'C:/path/to/the/file/'
+        save_aws (str): remote key in s3 bucket path e.g. 'path/to/file/'
+        aws_credentials (dict): aws credentials
+        return_figs (boolean): if true, methods will return objects
+
+        Returns
+        -------
+        None
         """
-        
         self.ticket_name = ticket_name
         self.data_frame = data_frame
         self.settings = settings
         self.save_path = save_path
         self.save_aws = save_aws
         self.show_plot = show_plot
         self.aws_credentials = aws_credentials
         self.return_figs = return_figs
 
     def plot_asset_signals(self, feature_list,spread_column, date_intervals = False):
-        
+        """
+        Display signals and hmm states over closing prices and feature time series
+
+        Parameters
+        ----------
+        feature_list (list): signal list
+        spread_column (list): moving average list
+        date_intervals (list): list of tuples of dates, e.g [('2022-01-01','2023-01-01'),('2022-01-01','2023-01-01')]
+
+        Returns
+        -------
+        fig (obj): plotly dashboard
+        """
         result_json_name = 'panel_signals.json'
         df = self.data_frame
         ma1 = self.settings['settings'][spread_column]['ma1']
         ma2 = self.settings['settings'][spread_column]['ma2']
         hmm_n_clust = self.settings['settings']['hmm']['n_clusters']
 
         def return_FeatureSingal_lists(feature, feature_2):
@@ -691,14 +898,25 @@
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_json_name ,input_path = self.save_path+result_json_name)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
         if self.return_figs:
             return fig
         
     def explore_states_ts(self):
+        """
+        display scaled time series of every hmm state
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        fig (obj): plotly dashboard
+        """
         result_json_name = 'ts_hmm.json'
         df = self.data_frame
         hmm_n_clust = self.settings['settings']['hmm']['n_clusters']
         state_rows = math.ceil(hmm_n_clust/2)
 
         rows_subplot = state_rows 
         height_plot = rows_subplot * 400
@@ -739,14 +957,28 @@
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_json_name ,input_path = self.save_path+result_json_name)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
         if self.return_figs:
             return fig
         
     def plot_hmm_analysis(self,settings, t_matrix, model = False):
+        """
+        display plots that analyse hmm states
+
+        Parameters
+        ----------
+        settings (dict): asset configurations
+        t_matrix (txt): asset state transition matrix
+        model(obj): hmm model
+
+        Returns
+        -------
+        fig (obj): plotly dashboard
+        messages (dict): hmm model metrics
+        """
         result_json_name = 'hmm_analysis.json'
         df = self.data_frame
         hmm_n_clust = self.settings['settings']['hmm']['n_clusters']
 
         rows_subplot = 2
         height_plot = rows_subplot * 400
         color_map = { i:DEFAULT_PLOTLY_COLORS[i] for i in range(hmm_n_clust)}
@@ -860,14 +1092,25 @@
             
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + 'market_message.json', input_path = self.save_path + 'market_message.json', aws_credentials = self.aws_credentials)
         
         if self.return_figs:
             return fig, messages
     def produce_forecasting_plot(self,predictions):
+        """
+        display forecasting plots
+
+        Parameters
+        ----------
+        predictions (pd.DataFrame): asset predictions
+
+        Returns
+        -------
+        None
+        """
         result_json_name = 'forecast_plot.json'
         hmm_n_clust = self.settings['settings']['hmm']['n_clusters']
         model_type = self.settings.get('model_type',False)
         lags = self.settings['settings']['volatility']['lags']
 
         df = self.data_frame
 
@@ -932,29 +1175,51 @@
         if self.show_plot:
             fig.show()
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_json_name ,input_path = self.save_path+result_json_name)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
 
 def plot_hmm_analysis_logger(data_frame,test_data_size, save_path = False, show_plot = True):
-    
+    '''
+    display box plots train and test of hmm state returns
+
+            Parameters:
+                    data_frame (pd.DataFrame): asset data
+                    test_data_size (int): test data size, the remaining is training data
+                    save_path (str): path/to/save/
+                    show_plot (boolean): if true, display plot
+
+            Returns:
+                    None
+    '''
     df = data_frame
     df_ = df[['Date','hmm_feature','Close',"chain_return"]].sort_values('Date')
     fig, axs = plt.subplots(1,2,figsize=(10,4))
     df__ = df_.iloc[:-test_data_size,]
     sns.boxplot(data=df__, x="hmm_feature", y="chain_return",ax = axs[0]).set_title('train dist')
     df__ = df_.iloc[-test_data_size:,]
     sns.boxplot(data=df__ , x="hmm_feature", y="chain_return",ax = axs[1]).set_title('test dist')
     if save_path:
         plt.savefig(save_path) 
     if not show_plot:
         plt.close()
 
 def plot_hmm_tsanalysis_logger(data_frame, test_data_size,save_path = False, show_plot = True):
-    
+    '''
+    display time series hmm state analisys
+
+            Parameters:
+                    data_frame (pd.DataFrame): asset data
+                    test_data_size (int): test data size, the remaining is training data
+                    save_path (str): path/to/save/
+                    show_plot (boolean): if true, display plot
+
+            Returns:
+                    None
+    '''
     df = data_frame
     df_ = df[['Date','hmm_feature','Close',"chain_return"]].sort_values('Date')
     states = list(df_['hmm_feature'].unique())
     states.sort()
     
     if test_data_size:
         df__ = df_.iloc[-test_data_size:,]
@@ -973,15 +1238,28 @@
     fig.autofmt_xdate()
     if save_path:
         plt.savefig(save_path) 
     if not show_plot:
         plt.close()
 
 def extract_data_traintest(object_stock,features_to_search,configs, target_configs, window_analysis = False, drop_nan= True):
+    '''
+    code snippet that execute object_stock or stock_eda_panel to get features
 
+            Parameters:
+                    object_stock (object): stock_eda_panel object
+                    features_to_search (list): list of features
+                    configs (dict): asset configurations
+                    target_configs (dict): target configurations
+                    window_analysis (int): take a sample size data
+                    drop_nan (boolean): remove nans from the data
+
+            Returns:
+                    object_stock (obj): object_stock with features and signals
+    '''
     object_stock.get_data() 
     object_stock.volatility_analysis(**configs['volatility']['config_params'], plot = False, save_features = False)
     target_params_up = target_configs['params_up']
     target_params_down = target_configs['params_down']
 
     for feature_name in features_to_search:
         initial_columns = object_stock.df.columns
@@ -999,15 +1277,27 @@
         object_stock.df = object_stock.df.dropna()
     if window_analysis:
         object_stock.df = object_stock.df.iloc[-window_analysis:,:]
         
     return object_stock
 
 def produce_simple_ts_from_model(stock_code, configs, n_days = 2000 , window_scope = '5y'):
+    '''
+    display dashboard analysis of a given asset
 
+            Parameters:
+                    stock_code (str): asset name
+                    configs (dict): asset configurations
+                    n_days (int): data size
+                    window_scope (str): window data size
+
+            Returns:
+                    fig (obj): plotly dashboard
+                    df (pd.DataFrame): result asset dataset
+    '''
     ## getting data
     volat_args = {'lags': 3, 'trad_days': 15, 'window_log_return': 10}
     
     object_stock = stock_eda_panel(stock_code , n_days, window_scope)
     object_stock.get_data() 
     object_stock.volatility_analysis(**volat_args, plot = False, save_features = False)
     features = list(configs.keys())
@@ -1058,25 +1348,29 @@
     fig.update_layout(height=height_plot, width=1600, title_text = f'asset plot and signals: {stock_code}')
 
     del object_stock
     
     return fig, df
 
 def save_edge_model(data, save_path = False, save_aws = False, show_result = False, aws_credentials = False):
-    """
-    data: pandas df
-    model_name: str
-    ticket_name: str name of the asset
-    save_path: str local path for saving e.g r'C:/path/to/the/file/'
-    save_aws: str remote key in s3 bucket path e.g. 'path/to/file/'
-    show_results: bool
-    aws_credentials: dict
-    
-    return a print of the dictionary
-    """
+    '''
+    get latest edge execution and edge probability
+
+            Parameters:
+                    data (pd.DataFrame): asset data
+                    model_name (str): model name
+                    ticket_name (str): name of the asset
+                    save_path (str): local path for saving e.g r'C:/path/to/the/file/'
+                    save_aws (str): remote key in s3 bucket path e.g. 'path/to/file/'
+                    show_results (bool): if true, display results
+                    aws_credentials (dict): aws credentials
+
+            Returns:
+                    None
+    '''
     today = datetime.datetime.today().strftime('%Y-%m-%d')
     
     curent_edge = (
         data[['Date','proba_target_down','proba_target_up']]
         .rename(columns = {'proba_target_down':'probability go down', 'proba_target_up':'probability go up'})
         .iloc[-1,:]
     )
@@ -1092,15 +1386,27 @@
     if save_path and save_aws:
         upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = save_aws + result_json_name, input_path = save_path+result_json_name, aws_credentials = aws_credentials)
         
     if show_result:
         print(curent_edge)
 
 def create_feature_edge(model, data,feature_name, threshold, target_variables):
+    '''
+    get latest edge execution and edge probability
 
+            Parameters:
+                    model (obj): edge model artifact
+                    data (pd.DataFrame): asset data
+                    feature_name (str): edge feature name
+                    threshold (float): edge threshold
+                    target_variables (list): names of the target columns
+
+            Returns:
+                    result_df (pd.DataFrame): result dataframe with edges
+    '''
     label_prediction = ['proba_'+x for x in target_variables]
     predictions = model.predict_proba(data)
     predictions = pd.DataFrame(predictions, columns = label_prediction, index = data.index)
     
     result_df = pd.concat([data, predictions], axis=1)
 
     for pred_col in label_prediction:
```

### Comparing `virgo_modules-0.0.75/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.76/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 27% similar despite different names*

```diff
@@ -49,113 +49,232 @@
 from feature_engine.discretisation import EqualWidthDiscretiser
 
 from .aws_utils import upload_file_to_aws
 
 import logging
 
 class InverseHyperbolicSine(BaseEstimator, TransformerMixin):
+
+    """
+    Class that applies inverse hyperbolic sine for feature transformation.
+    this class is compatible with scikitlearn pipeline
+
+    Attributes
+    ----------
+    features : list
+        list of features to apply the transformation
+    prefix : str
+        prefix for the new features. is '' the features are overwrite
+
+    Methods
+    -------
+    fit(additional="", X=DataFrame, y=None):
+        fit transformation.
+    transform(X=DataFrame, y=None):
+        apply feature transformation
+    """
+
     def __init__(self, features, prefix = ''):
         self.features = features
         self.prefix = prefix
 
     def fit(self, X, y=None):
         return self
-    
+
     def transform(self, X, y=None):
         for feature in self.features:
             X[f'{self.prefix}{feature}'] = np.arcsinh(X[feature])
         return X
 
 class VirgoWinsorizerFeature(BaseEstimator, TransformerMixin):
+
+    """
+    Class that applies winsorirization of a feature for feature transformation.
+    this class is compatible with scikitlearn pipeline
+
+    Attributes
+    ----------
+    feature_configs : dict
+        dictionary of features and configurations. the configuration has high and low limits per feature
+
+    Methods
+    -------
+    fit(additional="", X=DataFrame, y=None):
+        fit transformation.
+    transform(X=DataFrame, y=None):
+        apply feature transformation
+    """
+
     def __init__(self, feature_configs):
         self.feature_configs = feature_configs
     def fit(self, X, y=None):
         return self
 
     def transform(self, X, y=None):
         for feature in self.feature_configs:
             lower = self.feature_configs[feature]['min']
             upper = self.feature_configs[feature]['max']
             X[feature] = np.where( lower > X[feature], lower, X[feature])
             X[feature] = np.where( upper < X[feature], upper, X[feature])
         return X
 
 class FeatureSelector(BaseEstimator, TransformerMixin):
+
+    """
+    Class that applies selection of features.
+    this class is compatible with scikitlearn pipeline
+
+    Attributes
+    ----------
+    columns : list
+        list of features to select
+
+    Methods
+    -------
+    fit(additional="", X=DataFrame, y=None):
+        fit transformation.
+    transform(X=DataFrame, y=None):
+        apply feature transformation
+    """
+
     def __init__(self, columns):
         self.columns = columns
 
     def fit(self, X, y=None):
         return self
 
     def transform(self, X, y=None):
         return X[self.columns]
-    
+
 def sharpe_ratio(return_series):
+
+    '''
+    calculate sharpe ratio for given array.
+
+            Parameters:
+                    return_series (pd.series): pandas series of the asset returns
+
+            Returns:
+                    sharpe (float): sharpe ratio
+    '''
+
     N = 255 # Trading days in the year (change to 365 for crypto)
     rf = 0.005 # Half a percent risk free rare
     mean = return_series.mean() * N -rf
     sigma = return_series.std() * np.sqrt(N)
     sharpe = round(mean / sigma, 3)
     return sharpe
 
 class signal_combiner(BaseEstimator, TransformerMixin):
+
+    """
+    Class that applies feature combination of binary signals.
+    this class is compatible with scikitlearn pipeline
+
+    ...
+
+    Attributes
+    ----------
+    columns : list
+        list of features to select
+    drop : boolean
+        drop combining features
+    prefix_up : str
+        up prefix of the base feature
+    prefix_low : str
+        low prefix of the base feature
+
+    Methods
+    -------
+    fit(additional="", X=DataFrame, y=None):
+        fit transformation.
+    transform(X=DataFrame, y=None):
+        apply feature transformation
+    """
+
     def __init__(self, columns, drop = True, prefix_up = 'signal_up_', prefix_low = 'signal_low_'):
         self.columns = columns
         self.drop = drop
         self.prefix_up = prefix_up
         self.prefix_low = prefix_low
-        
+
     def fit(self, X, y=None):
         return self
 
     def transform(self, X, y=None):
         for column in self.columns:
             X['CombSignal_'+column] = np.where(
                 X[self.prefix_up + column] == 1,
-                1, 
+                1,
                 np.where(
                     X[self.prefix_low + column] == 1,
                     1,
                     0
                 )
             )
             if self.drop:
                 X = X.drop(columns = [self.prefix_up + column, self.prefix_low + column])
         return X
-    
+
 def data_processing_pipeline(features_base,features_to_drop = False, lag_dict = False, combine_signals = False, discretize_columns = False, correlation = 0.77):
-    
+
+    '''
+    create a scikit learn pipeline object using different configurations and feature engineering blocks with a given flow
+
+            Parameters:
+                    features_to_drop (list): list of features to drop
+                    lag_dict (dict): feature dictionary with configurations to apply lags
+                    combine_signals (list): list of columns/signals to combine
+                    discretize_columns (list): list of features to discretize, bins is fixed
+                    correlation (float): correaltion score threshold for feature selection
+
+            Returns:
+                    pipe (obj): pipeline object
+    '''
+
     lag_pipe_sec = [(f'lags_{key}', LagFeatures(variables = key, periods = lag_dict[key])) for key in lag_dict] if lag_dict else []
     drop_pipe = [('drop_features' , DropFeatures(features_to_drop=features_to_drop))] if features_to_drop else []
     merge = [('signal_combiner', signal_combiner(combine_signals))] if combine_signals else []
     discretize = [('discretize',EqualWidthDiscretiser(discretize_columns, bins = 20 ))] if discretize_columns else []
     drop_corr = [('drop_corr', DropCorrelatedFeatures(threshold=correlation))] if correlation else []
-    
+
     pipe = Pipeline(
         [('selector', FeatureSelector(features_base))] + \
         [('encoding',OneHotEncoder(top_categories=None, variables=['hmm_feature']))]  + \
         merge + \
         discretize + \
         lag_pipe_sec + \
         [('fill na', MeanMedianImputer())] + \
         drop_corr + \
         drop_pipe
     )
     return pipe
 
 def states_relevance_score(data, default_benchmark_sd = 0.00003, t_threshold = 2):
+    '''
+    calculate relevance score and summary report for hmm model 
+
+            Parameters:
+                    default_benchmark_sd (float): default value to bias SD for t calculation
+                    t_threshold (float): alpha or z threshold for the normalized score
+
+            Returns:
+                    mean_relevance (float): mean relevance score of the states
+                    cluster_returns (pd.DataFrame): summary report of the analysis
+                    number_relevant_states (int): number of relevant states
+    '''
     ## legnths
     cluster_lengths = data.groupby(['hmm_feature','chain_id'],as_index = False).agg(chain_lenght = ('hmm_chain_order','max'))
     cluster_lengths = cluster_lengths.groupby('hmm_feature').agg(cluster_length_median = ('chain_lenght','median'))
     ## means
     def quantile2(x):
         return x.quantile(0.25)
     def quantile3(x):
         return x.quantile(0.75)
-    
+
     cluster_returns = data.groupby('hmm_feature').agg(
         n_uniques = ('chain_id','nunique'),
         n_obs = ('Date','count'),
         cluster_ret_q25 = ('chain_return',quantile2),
         cluster_ret_median = ('chain_return','median'),
         cluster_ret_q75 = ('chain_return',quantile3),
     )
@@ -167,100 +286,253 @@
     cluster_returns['iqr'] = cluster_returns.cluster_ret_q75 - cluster_returns.cluster_ret_q25
     cluster_returns['perc_25'] = abs(cluster_returns.cluster_ret_q25)/cluster_returns['iqr']
     cluster_returns['perc_75'] = abs(cluster_returns.cluster_ret_q75)/cluster_returns['iqr']
     cluster_returns['min_perc'] = cluster_returns[['perc_25','perc_75']].min(axis = 1)
     cluster_returns['min_overlap'] = np.where(cluster_returns['perc_dispute'] == 1,cluster_returns['min_perc'],0)
     cluster_returns['abs_median'] = abs(cluster_returns['cluster_ret_median'])
     cluster_returns = cluster_returns.drop(columns = ['perc_25','perc_75','min_perc'])
-    
+
     ## relevance or importance
     # naive aproach
     cluster_returns['relevance'] =  cluster_returns['abs_median'] + ( 0.5 - cluster_returns['min_overlap'])
     cluster_returns['t_calc'] = (cluster_returns['cluster_ret_median'] - 0)/(cluster_returns['iqr']/cluster_returns['n_obs'] + default_benchmark_sd/cluster_returns['n_obs'])**(1/2)
     cluster_returns['abs_t_accpted'] = abs(cluster_returns['t_calc'])
     cluster_returns['t_accpted'] = abs(cluster_returns['abs_t_accpted']) > t_threshold
-    
+
     mean_relevance = cluster_returns['abs_t_accpted'].mean()
     number_relevant_states = len(cluster_returns[cluster_returns.t_accpted == True])
 
     return mean_relevance, cluster_returns, number_relevant_states
 
 
 class stock_eda_panel(object):
-    
+
+    """
+    Class that initialy gets stock data then apply feature enginering, enrichment, analysis, plotting, model training etc.
+
+    Attributes
+    ----------
+    stock_code : str
+        symbol of the asset
+    n_days : str
+        number of days to extract data
+    data_window : str
+        large window to extract data. Large window is required o extract more data. e.g. '5y', '10y', '15'
+    df : pd.DataFrame
+        Pandas dataframe of the asset data with features
+    strategy_log: pd.DataFrame
+        Pandas dataframe that has the results of different tested strategies (result from strategy simulator hmm)
+    best_strategy: list
+        features of the best performing strategy (result from strategy simulator hmm)
+    top_10_strategy: dict
+        top 10 best performing strategies (result from strategy simulator hmm)
+    settings: dict
+        configuration dictionary of the features and other parameters
+
+    Methods
+    -------
+    augmented_dickey_fuller_statistics(time_series=pd.Series, label=str):
+        Perform dickey fuller or stationary test for a given time series
+        It will print p value of the features
+    get_data():
+        Get asset data performing some data normalization or formating (in case of dates)
+    plot_series_returns(roll_mean_lags1=int, roll_mean_lags2=int)
+        Display plot that time series with mean rolling windows and rolling standard deviations of daily closing prices
+    seasonal_plot():
+        Display time series split by year
+    plot_price_signal(feature=str, feature_2=str, opacity=float):
+        Display botton and roof signals over the closing prices
+    volatility_analysis(lags=int, trad_days=int, window_log_return=int, plot=boolean, save_features=boolean):
+        this method performs log return and volatilyty analysis of the closing prices
+    find_lag(feature=str, lag_list=list, column_target=str,posterior_lag=int, test_size=int):
+        displays correlation curves, using spearman and pearson correlation, of a given feature at different time lags with respecto to a given target
+    outlier_plot(zlim=float, plot=boolean, save_features=boolean):
+        perform outlier analysis of the log returns. It also permors normality test of returns
+    analysis_roll_mean_log_returns(lags=int, plot=boolean):
+        perform analysis of lags of the mean rolling log return
+    compute_clip_bands(feature_name=str,threshold=float):
+        compute outlier detection for a given signal, Note that this follows mean reversion procedure and feature has to be stationary. Also botton and roof resulting signals is attached to the dataframe
+    signal_plotter(feature_name=str):
+        display analysis plot of a feature with high and low signals
+    log_features_standard(feature_name=str):
+        save resulting feature names in an standard structure
+    relative_spread_MA(ma1=int, ma2=int, threshold=float, plot=boolean, save_features=boolean):
+        perform relative moving average features, one for short term and another for long/mid term
+    pair_feature(pair_symbol=str, plot=boolean):
+        initialize pair feature data extraction and analysis
+    calculate_cointegration(series_1=pd.series, series_2=pd.series):
+        calculate cointegration score for two time series
+    bidirect_count_feature(rolling_window=int, threshold=float, plot=boolean, save_features=boolean):
+        perform negative and positive return counting in a given rolling time window
+    get_relative_range_feature(window=int, threshold=float, plot=boolean, save_features=boolean):
+        perform relative spread of opening and closing price
+    rsi_feature_improved(window=int, threshold=float, plot=boolean, save_features=boolean):
+        perform relative strength index
+    days_features_bands(window=int, threshold=float, plot=boolean, save_features=boolean):
+        compute mean returns for a given day of the week in a window scope per day
+    analysis_smooth_volume(window=int, threshold=float, plot=boolean, save_features=boolean):
+        compute feature of thrading volumes
+    roc_feature(window=int, threshold=float, plot=boolean, save_features=boolean):
+        perform price rate of change
+    stoch_feature(window=int, smooth1=int, smooth2=int, threshold=float, plot=boolean, save_features=boolean):
+        perform stochastic oscilator RSI feature
+    stochastic_feature(window=int, smooth=int, threshold=float, plot=boolean, save_features=boolean):
+        perform stochastic oscilator feature
+    william_feature(lbp=int, threshold=float, plot=boolean, save_features=boolean):
+        perfom fast stochastic oscilator or william indicator
+    vortex_feature(window=int, threshold=float, plot=boolean, save_features=boolean):
+        perform vortex oscilator
+    pair_index_feature(pair_symbol=str, feature_label=str, window=int, threshold=float, plot=boolean, save_features=boolean):
+        perform additional asset ROC feature, then a new feature is created in the main dataframe
+    produce_order_features(feature_name=str, save_features=boolean):
+        perform a feature that captures high and low values in an index. this is usefull to know duration/persistence of a signal
+    create_hmm_derived_features():
+        create features derived from hmm states features. Features are the index of the state, the duration of the state, chain raturn
+    cluster_hmm_analysis(n_clusters=int,features_hmm=list, test_data_size=int, seed=int, lag_returns_state=int, plot=boolean, save_features=boolean, model=obj):
+        create or use a hmm model
+    sharpe_ratio(return_series=pd.Series, n_trad_days=int, rf=float):
+        perform sharpe ratio of a given time series return
+    treat_signal_strategy(test_data=pd.DataFrame, strategy=list):
+        helper method that treats signals and converts signals to 1 or 0
+    stategy_simulator(features=list, hmm_feature=boolean):
+        execute strategy and get some performance metrics like sharpe ratio, return
+    viz_strategy(strategy):
+        display analysis plot of a given strategy
+    deep_dive_analysis_hmm(test_data_size=int, split=str):
+        display analysis plot hmm model
+    get_targets(steps=int):
+        produce regression target return taking future prices
+    get_categorical_targets(horizon=int, flor_loss=float, top_gain=float):
+        produce binary target return taking future prices. it produce two targets, one for high returns and another for low returns
+    get_configurations(test_data_size=int, val_data_size=int, model_type=str):
+        produce configuration dictionary that were saved in the feature generation methods if save_features was activated
+    """
+
     def __init__(self, stock_code, n_days, data_window = '5y'):
+
+        """
+        Initialize object
+
+        Parameters
+        ----------
+        stock_code (str): symbol of the asset
+        n_days (str): number of days to extract data
+        data_window (str): large window to extract data. Large window is required o extract more data. e.g. '5y', '10y', '15'
+
+        Returns
+        -------
+        None
+        """
+
         self.stock_code = stock_code
         self.n_days = n_days
         self.today = datetime.date.today()
         self.features = list()
         self.signals = list()
         self.data_window = data_window
-        
+
     def augmented_dickey_fuller_statistics(self,time_series, label):
+        """
+        Perform dickey fuller or stationary test for a given time series
+        It will print p value of the features
+
+        Parameters
+        ----------
+        time_series (pd.Series): pandas series of the time series
+        label (pd.Series): feature name
+
+        Returns
+        -------
+        None
+        """
         result = adfuller(time_series.dropna().values)
         print('p-value: {} for the series {}'.format(round(result[1],6), label))
-        
+
     def get_data(self):
+        """
+        Get asset data performing some data normalization or formating (in case of dates)
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
+
         begin_date = self.today - relativedelta(days = self.n_days)
         begin_date_str = begin_date.strftime('%Y-%m-%d')
 
         stock = yf.Ticker(self.stock_code)
         df = stock.history(period=self.data_window)
 
         df = df.sort_values('Date')
         df.reset_index(inplace=True)
         df['Date'] = pd.to_datetime(df['Date'], format='mixed',utc=True).dt.date
         df['Date'] = pd.to_datetime(df['Date'])
-        
+
         df = df[df.Date >= begin_date_str ]
         self.settings_general = {
             'n_days':self.n_days,
             'begin_date':begin_date_str,
             'data_window': self.data_window,
             'execution_date': self.today.strftime('%Y-%m-%d')
         }
         self.df = df
-        
+
         ### cleaning volume
         ### volume clearning
         self.df['Volume'] = np.where(self.df['Volume'] <= 10, np.nan, self.df['Volume'])
         self.df['Volume'] = self.df['Volume'].fillna(method='bfill')
-        
+
         ## filling
-        
+
         base_columns_unit_test = ['Open','High','Low','Close','Volume']
         self.df[base_columns_unit_test] = self.df[base_columns_unit_test].fillna(method='ffill')
-        
+
         ## cleaning nulls
-        
+
         xs = self.df[base_columns_unit_test].isnull().sum()/self.df[base_columns_unit_test].count()
         reject_columns = list(xs[xs > 0.5].index.values)
-        
+
         if len(reject_columns) > 0:
             logging.warning("the following columns have many nulls and are drop: {}".format(reject_columns))
             self.df = self.df.drop(columns = reject_columns)
-        
-        
+
     def plot_series_returns(self,roll_mean_lags1,roll_mean_lags2):
-        
+
+        """
+        Display plot that time series with mean rolling windows and rolling standard deviations of daily closing prices
+
+        Parameters
+        ----------
+        roll_mean_lags1 (int): short term window
+        roll_mean_lags2 (int): mid/long term window
+
+        Returns
+        -------
+        None
+        """
+
         df = self.df
         begin_date = self.today - relativedelta(days = self.n_days)
         begin_date_str = begin_date.strftime('%Y-%m-%d')
-        
+
          ### getting rolling mean
         df["Close_roll_mean"] = (
             df.sort_values("Date")["Close"]
             .transform(lambda x: x.rolling(roll_mean_lags1, min_periods=1).mean())
         )
-        
+
         df["Close_roll_mean_2"] = (
             df.sort_values("Date")["Close"]
             .transform(lambda x: x.rolling(roll_mean_lags2, min_periods=1).mean())
         )
-        
+
         ### getting rolling stdv
         df["Close_roll_std"] = (
             df.sort_values("Date")["Close"]
             .transform(lambda x: x.rolling(roll_mean_lags1, min_periods=1).std())
         )
         df["upper"] = df['Close_roll_mean'] + df["Close_roll_std"]*2
         df["lower"] = df['Close_roll_mean'] - df["Close_roll_std"]*2
@@ -269,24 +541,37 @@
 
         fig = make_subplots(rows=1, cols=1,vertical_spacing = 0.1,shared_xaxes=True,
                            subplot_titles=(
                                f'stock: {self.stock_code} roll window analysis: {roll_mean_lags1} days'
                            ))
 
         fig.add_trace(go.Scatter(x=df['Date'], y=df.Close, marker_color = 'blue', name='Price'),row=1, col=1)
-        
+
         fig.add_trace(go.Scatter(x=df['Date'], y=df.Close_roll_mean, marker_color = 'black', name='roll mean' ),row=1, col=1)
         fig.add_trace(go.Scatter(x=df['Date'], y=df.Close_roll_mean_2, marker_color = 'grey', name='roll mean 2' ),row=1, col=1)
         fig.add_trace(go.Scatter(x=df['Date'], y=df.lower, marker_color = 'pink',legendgroup='bound', name='bound' ),row=1, col=1)
         fig.add_trace(go.Scatter(x=df['Date'], y=df.upper, marker_color = 'pink',legendgroup='bound', name='bound', showlegend=False ),row=1, col=1)
 
         fig.update_layout(height=500, width=1200, title_text=f"stock {self.stock_code} vizualization")
         fig.show()
-        
+
     def seasonal_plot(self):
+
+        """
+        Display time series split by year
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
+
         df = self.df
         years = list(df['Date'].dt.year.unique())
         years.sort()
         years = years[::-1]
         years_last = max(years)
 
         fig = make_subplots(rows=1, cols=1,vertical_spacing = 0.1,shared_xaxes=True,)
@@ -298,35 +583,49 @@
             if year == years_last:
                 fig.add_trace(go.Scatter(x= df_plot.Date_trunc, y=df_plot.Close, name=str(year)),row=1, col=1)
                 continue
             fig.add_trace(go.Scatter(x= df_plot.Date_trunc, y=df_plot.Close, name=str(year), line = dict(dash='dash')),row=1, col=1)
 
         fig.update_layout(height=500, width=1400, title_text=f"stock {self.stock_code} seasonal vizualization")
         fig.show()
-        
+
     def plot_price_signal(self, feature, feature_2 = '', opacity = 0.3):
-    
-        signal_up_list = [f'signal_up_{feature}', f'signal_up_{feature_2}']  
+
+        """
+        Display botton and roof signals over the closing prices
+
+        Parameters
+        ----------
+        feature (str): name of the main feature to plot
+        feature_2 (str): name of the alternative feature to plot
+        opacity (float): opacity degree of the signals points
+
+        Returns
+        -------
+        None
+        """
+
+        signal_up_list = [f'signal_up_{feature}', f'signal_up_{feature_2}']
         signal_low_list = [f'signal_low_{feature}', f'signal_low_{feature_2}']
         norm_list = [f'norm_{feature}', f'z_{feature}', feature]
 
         fig = make_subplots(rows=2, cols=1,vertical_spacing = 0.1, shared_xaxes=True, subplot_titles = [f'norm signal - {feature}',f'signal over price'] )
 
         for norm_feat in norm_list:
             if norm_feat in self.df.columns:
                 fig.add_trace(go.Scatter(x=self.df['Date'], y=self.df[norm_feat],legendgroup="up", mode='lines',name = norm_feat, marker_color = 'blue'),col = 1, row = 1)
                 break
-        
-        
+
+
         fig.add_trace(go.Scatter(x=self.df['Date'], y=self.df['Close'], mode='lines',name = 'history', marker_color = 'grey'),col = 1, row = 2)
-        
+
         if feature == 'MA_spread':
             fig.add_trace(go.Scatter(x=self.df['Date'], y=self.df[self.ma1_column],legendgroup="ma", mode='lines',name = self.ma1_column, marker_color = 'black'),col = 1, row = 2)
             fig.add_trace(go.Scatter(x=self.df['Date'], y=self.df[self.ma2_column],legendgroup="ma", mode='lines',name = self.ma2_column, marker_color = 'grey'),col = 1, row = 2)
-        
+
         for norm_feat in norm_list:
             if norm_feat in self.df.columns:
                 fig.add_trace(go.Scatter(x=self.df['Date'], y=np.where(self.df[norm_feat] > 0, self.df['Close'], np.nan),legendgroup="up", mode='markers',name = 'up', marker_color = 'green',opacity = opacity),col = 1, row = 2)
                 fig.add_trace(go.Scatter(x=self.df['Date'], y=np.where(self.df[norm_feat] <= 0, self.df['Close'], np.nan),legendgroup="low", mode='markers',name = 'low', marker_color = 'red',opacity = opacity),col = 1, row = 2)
 
         for signal_up in signal_up_list:
             if signal_up in self.df.columns:
@@ -334,32 +633,49 @@
 
         for signal_low in signal_low_list:
             if signal_low in self.df.columns:
                 fig.add_trace(go.Scatter(x=self.df['Date'], y=np.where(self.df[signal_low] == 1, self.df['Close'], np.nan),legendgroup="high low", mode='markers',name = 'high low', marker_color = 'red'),col = 1, row = 2)
 
         fig.update_layout(height=900, width=1200)
         fig.show()
-    
+
     def volatility_analysis(self, lags, trad_days, window_log_return, plot = False, save_features = False):
+
+        """
+        this method performs log return and volatilyty analysis of the closing prices
+
+        Parameters
+        ----------
+        lags (int): number of lags to apply to the closing prices
+        trad_days (int): number of trading days to anualize returns or volatility
+        window_log_return (int): window for rolling returns
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+
+        Returns
+        -------
+        None
+        """
+
         df = self.df
         df['log_return'] = np.log(df.Close/df.Close.shift(lags))
         df['sqr_log_return'] = np.square(df.log_return)
         df['volatility_log_return'] = df.log_return.rolling(window = trad_days).std()*np.sqrt(252)
 
         df["roll_mean_log_return"] = (
                 df.sort_values("Date")["log_return"]
                 .transform(lambda x: x.rolling(window_log_return, min_periods=1).mean())
             )
-        
+
         if save_features:
             self.features.append('volatility_log_return')
             self.features.append('roll_mean_log_return')
             self.features.append('log_return')
             self.settings_volatility = {'lags':lags, 'trad_days':trad_days, 'window_log_return':window_log_return}
-            
+
         if plot:
             fig = make_subplots(rows=3, cols=1,vertical_spacing = 0.02,shared_xaxes=True,
                             specs=[
                                 [{}],
                                 [{"secondary_y": True}],
                                 [{}],
                                   ])
@@ -391,49 +707,79 @@
             axs[3].set_title('pacf roll_mean_log_return')
             plt.show()
 
             print('___________________________________________')
 
             self.augmented_dickey_fuller_statistics(df['log_return'], 'log_return')
             self.augmented_dickey_fuller_statistics(df['roll_mean_log_return'], 'roll_mean_log_return')
-            
-            
+
+
     def find_lag(self, feature, lag_list, column_target = 'log_return',posterior_lag = 4, test_size = 350):
 
+        """
+        displays correlation curves, using spearman and pearson correlation, of a given feature at different time lags with respecto to a given target
+
+        Parameters
+        ----------
+        feature (str): feature name to apply lags
+        lag_list (list): list of lags, each lag as integer
+        column_target (str): target to get correlation, e.g return or mean reaturn
+        posterior_lag (int): for the target, posterior window shift to calculate a window return
+        test_size (int): data size of the test data. The remaining is going to be used as training data. This parameters is ment to avoid overfiting and leackage
+
+        Returns
+        -------
+        None
+        """
+
         results = dict()
         df = self.df.iloc[:-test_size,:][['Date','Close','roll_mean_log_return','log_return',feature]].sort_values('Date').copy()
         for i,lag in enumerate(lag_list):
             lag_column = f'{feature}_lag_{lag}'
             df[lag_column] = df[feature].shift(lag)
             df['target_posterior_lag'] = df[column_target].shift(-posterior_lag)
             df = df.dropna()
             r_log = stats.mstats.pearsonr(df['target_posterior_lag'], df[lag_column])
             sp_log = stats.spearmanr(df['target_posterior_lag'], df[lag_column])
 
             results[i] = {
                 'lag':lag,
                 'pearsonr_log_return':r_log[0],
                 'spearman_log_return': sp_log[0],
-            } 
+            }
         del df
         results_df = pd.DataFrame(results).T
 
         fig = plt.figure(figsize = (10,3))
         plt.plot(results_df.lag,results_df.pearsonr_log_return,label = f'pearsonr_{column_target}')
         plt.plot(results_df.lag,results_df.spearman_log_return,label = f'spearman_{column_target}')
         plt.scatter(results_df.lag,results_df.pearsonr_log_return)
         plt.scatter(results_df.lag,results_df.spearman_log_return)
         plt.title(f'{feature}: correlation curve with the target {column_target} lag -{posterior_lag} periods')
         plt.legend()
         plt.axhline(y=0, color='grey', linestyle='--')
         plt.show()
-    
-    
+
+
     def outlier_plot(self, zlim, plot = False, save_features = False):
-        
+
+        """
+        perform outlier analysis of the log returns. It also permors normality test of returns
+
+        Parameters
+        ----------
+        zlim (float): alpha or z thrsholds for normalized returns
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+
+        Returns
+        -------
+        None
+        """
+
         mean = self.df.log_return.mean()
         std = self.df.log_return.std()
         self.df['z_log_return'] = (self.df.log_return - mean)/std
         l1,l2 = 1.96, 1.0
 
         mean_ = self.df['z_log_return'].mean()
         self.df['z_std_log_return'] = self.df.sort_values("Date")["z_log_return"].rolling(50).std()
@@ -447,89 +793,139 @@
             self.signals.append('signal_up_outlier')
             self.settings_outlier = {'zlim':zlim}
         if plot:
             mu = self.df['z_log_return'].mean()
             sigma = self.df['z_log_return'].std()
             x = np.linspace(self.df['z_log_return'].min(),self.df['z_log_return'].max(), 15000)
             y = stats.norm.pdf(x, loc = mu, scale = sigma)
-            
+
             fig, axs = plt.subplots(2, 1,figsize=(15,8))
 
             axs[0].hist(self.df['z_log_return'],density = True,bins = 100 , label = 'Returns distribution')
             axs[0].axvline(l1, color='r', linestyle='--')
             axs[0].axvline(-l1, color='r', linestyle='--')
             axs[0].axvline(l2, color='green', linestyle='--')
             axs[0].axvline(-l2, color='green', linestyle='--')
             axs[0].plot(x,y, linewidth = 3, color = 'r', label = 'Normal Dist Curve')
-            
+
             axs[1].plot(self.df['Date'],self.df['z_log_return'])
             axs[1].plot(self.df['Date'],self.df['low_outlier'], linestyle='--')
             axs[1].plot(self.df['Date'],self.df['up_outlier'], linestyle='--')
 
             fig.legend()
             plt.show()
 
             z_stat, p_stat = stats.normaltest(self.df['z_log_return'].dropna())
-            p_stat = round(p_stat, 7) 
+            p_stat = round(p_stat, 7)
             print('---------------------- returns normality tests ----------------------------')
             if p_stat < 0.05:
                 print(f'pvalue: {p_stat} then, returns do not follow a normal distribution')
             else:
                 print(f'pvalue: {p_stat} then, returns follow a normal distribution')
-    
+
     def analysis_roll_mean_log_returns(self, lags, plot = False):
 
+        """
+        perform analysis of lags of the mean rolling log return
+
+        Parameters
+        ----------
+        lags (int): lags to apply to the roll log return
+        plot (boolean): True to display plot
+
+        Returns
+        -------
+        None
+        """
+
         self.df['lag'] = self.df.roll_mean_log_return.shift(lags)
         self.df['Diff'] = self.df['roll_mean_log_return'] - self.df['lag']
-        
+
         if plot:
 
             fig, axs = plt.subplots(1, 3,figsize=(19,4))
             self.df['Diff'].plot(ax=axs[0])
             plot_acf(self.df['Diff'].dropna(),lags=25, ax=axs[1])
             plot_pacf(self.df['Diff'].dropna(),lags=25, ax=axs[2])
             axs[0].set_title('Integration of the roll mean log-returns')
             axs[1].set_title('acf Integration of the roll mean log-returns')
             axs[2].set_title('pacf Integration of the roll mean log-returns')
             plt.show()
 
     def compute_clip_bands(self,feature_name,threshold):
-    
+
+        """
+        compute outlier detection for a given signal, Note that this follows mean reversion procedure and feature has to be stationary. Also botton and roof resulting signals is attached to the dataframe
+
+        Parameters
+        ----------
+        feature_name (str): feature name
+        threshold (float): alpha or z thrsholds for normalized returns
+
+        Returns
+        -------
+        None
+        """
+
         self.df[f'norm_{feature_name}'] =  (self.df[feature_name] - self.df[feature_name].mean())/self.df[feature_name].std()
         mean_ = self.df[f'norm_{feature_name}'].mean()
 
         self.df[f'up_rollstd_{feature_name}'] = self.df.sort_values("Date")[f'norm_{feature_name}'].clip(0,100).rolling(50).std()
         self.df[f'low_rollstd_{feature_name}'] = self.df.sort_values("Date")[f'norm_{feature_name}'].clip(-100,0).rolling(50).std()
 
         self.df[f'upper_{feature_name}'] = threshold*self.df[f'up_rollstd_{feature_name}'] + mean_
         self.df[f'lower_{feature_name}'] = -threshold*self.df[f'low_rollstd_{feature_name}'] + mean_
 
         self.df[f'signal_low_{feature_name}'] = np.where( (self.df[f'norm_{feature_name}'] < self.df[f'lower_{feature_name}'] ), 1, 0)
         self.df[f'signal_up_{feature_name}'] = np.where( (self.df[f'norm_{feature_name}'] > self.df[f'upper_{feature_name}'] ), 1, 0)
 
     def signal_plotter(self, feature_name):
+
+        """
+        display analysis plot of a feature with high and low signals
+
+        Parameters
+        ----------
+        feature_name (str): feature name
+
+        Returns
+        -------
+        None
+        """
+
         fig, axs = plt.subplots(1, 3,figsize=(17,5))
-        
+
         axs[0].plot(self.df[f'upper_{feature_name}'],color = 'grey', linestyle='--')
         axs[0].plot(self.df[f'lower_{feature_name}'],color = 'grey', linestyle='--')
         axs[0].plot(self.df[f'norm_{feature_name}'])
-        
+
         plot_acf(self.df[feature_name].dropna(),lags=25,ax = axs[1])
         axs[1].set_title(f'acf {feature_name}')
-        
+
         plot_pacf(self.df[feature_name].dropna(),lags=25,ax = axs[2])
         axs[2].set_title(f'pacf {feature_name}')
-        
+
         fig.show()
 
     def log_features_standard(self, feature_name):
+        """
+        save resulting feature names in an standard structure
+
+        Parameters
+        ----------
+        feature_name (str): feature name
+
+        Returns
+        -------
+        None
+        """
         self.features.append(feature_name)
         self.signals.append(f'signal_up_{feature_name}')
         self.signals.append(f'signal_low_{feature_name}')
-    
+
     #######################
     #### to be deprecated ####
     def spread_MA(self, ma1, ma2, limit = 1.95, plot = False, save_features = False):
 
         self.df[f'MA_{ma1}'] = (self.df.sort_values("Date")["Close"].transform(lambda x: x.rolling(ma1, min_periods=1).mean()))
         self.df[f'MA_{ma2}'] = (self.df.sort_values("Date")["Close"].transform(lambda x: x.rolling(ma2, min_periods=1).mean()))
 
@@ -542,33 +938,33 @@
         self.df['rollstd_MA_spread'] = self.df.sort_values("Date")["norm_MA_spread"].rolling(50).std()
 
         self.df['upper_MA_spread'] = limit*self.df['rollstd_MA_spread'] + mean_
         self.df['lower_MA_spread'] = -limit*self.df['rollstd_MA_spread'] + mean_
 
         self.df['signal_low_MA_spread'] = np.where( (self.df['norm_MA_spread'] < self.df['lower_MA_spread'] ), 1, 0)
         self.df['signal_up_MA_spread'] = np.where( (self.df['norm_MA_spread'] > self.df['upper_MA_spread'] ), 1, 0)
-        
+
         ### ploting purposes
         self.df[f"Roll_mean_{ma1}"] = (
             self.df.sort_values("Date")["Close"]
             .transform(lambda x: x.rolling(ma1, min_periods=1).mean())
         )
         self.df[f"Roll_mean_{ma2}"] = (
             self.df.sort_values("Date")["Close"]
             .transform(lambda x: x.rolling(ma2, min_periods=1).mean())
         )
-        
+
 
         print('--------------------------------------------------------------------')
         if save_features:
             self.features.append('MA_spread')
             self.signals.append('signal_low_MA_spread')
             self.signals.append('signal_up_MA_spread')
-            self.settings_spread_ma = {'ma1':ma1, 'ma2':ma2, 'limit':limit}  
-            
+            self.settings_spread_ma = {'ma1':ma1, 'ma2':ma2, 'limit':limit}
+
         if plot:
 
             fig, axs = plt.subplots(1, 3,figsize=(21,4))
 
             axs[0].plot(self.df['Date'],self.df['norm_MA_spread'])
             axs[0].plot(self.df['Date'],self.df['upper_MA_spread'], linestyle='--')
             axs[0].plot(self.df['Date'],self.df['lower_MA_spread'], linestyle='--')
@@ -577,17 +973,31 @@
             plot_acf(self.df['MA_spread'].dropna(),lags=25, ax=axs[1])
             axs[1].set_title('acf MA_spread series')
 
             plot_pacf(self.df['MA_spread'].dropna(),lags=25, ax=axs[2])
             axs[2].set_title('acf MA_spread series')
             plt.show()
     ##################################################
-    
+
     def relative_spread_MA(self, ma1, ma2, threshold = 1.95, plot = False, save_features = False):
-    
+        """
+        perform relative moving average features, one for short term and another for long/mid term
+
+        Parameters
+        ----------
+        ma1 (int): short term moving average window
+        ma2 (int): long/mid term moving average window
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+
+        Returns
+        -------
+        None
+        """
         feature_name = 'rel_MA_spread'
 
         self.df[f'MA_{ma1}'] = (self.df.sort_values("Date")["Close"].transform(lambda x: x.rolling(ma1, min_periods=1).mean()))
         self.df[f'MA_{ma2}'] = (self.df.sort_values("Date")["Close"].transform(lambda x: x.rolling(ma2, min_periods=1).mean()))
 
         self.ma1_column = f'MA_{ma1}'
         self.ma2_column = f'MA_{ma2}'
@@ -604,34 +1014,47 @@
             self.df.sort_values("Date")["Close"]
             .transform(lambda x: x.rolling(ma2, min_periods=1).mean())
         )
 
         print('--------------------------------------------------------------------')
         if save_features:
             self.log_features_standard(feature_name)
-            self.settings_relative_spread_ma = {'ma1':ma1, 'ma2':ma2, 'threshold':threshold}  
+            self.settings_relative_spread_ma = {'ma1':ma1, 'ma2':ma2, 'threshold':threshold}
 
         if plot:
 
             self.signal_plotter(feature_name)
-    
+
     def pair_feature(self, pair_symbol, plot = False):
+        """
+        initialize pair feature data extraction and analysis
+
+        Parameters
+        ----------
+        pair_symbol (str): symbol of the pair asset to extract
+        plot (boolean): True to display plot
+        
+        Returns
+        -------
+        None
+        """
+
         self.pair_symbol = pair_symbol
         begin_date = self.today - relativedelta(days = self.n_days)
         begin_date_str = begin_date.strftime('%Y-%m-%d')
 
         stock = yf.Ticker(self.pair_symbol)
         df = stock.history(period=self.data_window)
         df = df.sort_values('Date')
         df.reset_index(inplace=True)
         df['Date'] = pd.to_datetime(df['Date'], format='mixed',utc=True).dt.date
         df['Date'] = pd.to_datetime(df['Date'])
         df = df[df.Date >= begin_date_str ]
         self.pair_df = df
-        
+
         #### converting the same index ####
         dates_vector = self.df.Date.to_frame()
         self.pair_df = dates_vector.merge(self.pair_df, on ='Date',how = 'left')
         self.pair_df = self.pair_df.fillna(method = 'bfill')
         self.pair_df = self.pair_df.fillna(method = 'ffill')
         ########
 
@@ -649,69 +1072,96 @@
             asset_1_values = self.df['Close'].values/self.df['Close'].iloc[0].item()
             asset_2_values = self.pair_df['Close'].values/self.pair_df['Close'].iloc[0].item()
             plt.figure(1, figsize=(10,5))
             plt.plot(self.df['Date'],asset_1_values,label = asset_1)
             plt.plot(self.df['Date'],asset_2_values,label = asset_2)
             plt.legend()
             plt.show()
-    
+
     def calculate_cointegration(self,series_1, series_2):
+        """
+        calculate cointegration score for two time series
+
+        Parameters
+        ----------
+        series_1 (pd.series): time series
+        series_2 (pd.series): time series
+        
+        Returns
+        -------
+        coint_flag (boolean): 1 if the p_value cointegration_t are lower than 0.05 and critical value
+        hedge_value (float): beta from the regression model
+        """
+
         coint_flag = 0
         coint_res = coint(series_1, series_2)
         coint_t = coint_res[0]
         p_value = coint_res[1]
         critical_value = coint_res[2][1]
 
         model = sm.OLS(series_1, series_2).fit()
         hedge_value = model.params[0]
         coint_flag = 1 if p_value < 0.05 and coint_t < critical_value else 0
 
         return coint_flag, hedge_value
-    
+
     def produce_pair_score_plot(self, window, z_threshold, plot = False, save_features = False):
+        """
+        display analysis of the pair feature and save results in case if needed
 
+        Parameters
+        ----------
+        window (int): window to apply to the rolling spread between pair and main asset
+        z_threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         spread_series = pd.Series(self.df.pair_spread)
         mean = spread_series.rolling(center = False, window = window).mean()
         std = spread_series.rolling(center = False, window = window).std()
         x = spread_series.rolling(center=False, window =  1).mean()
         z_score = (x - mean)/std
         self.df['pair_z_score'] = z_score
         self.df['signal_low_pair_z_score'] = np.where(self.df['pair_z_score'] < -z_threshold, 1, 0)
         self.df['signal_up_pair_z_score'] = np.where(self.df['pair_z_score'] > z_threshold, 1, 0)
-        
+
         if save_features:
             self.log_features_standard('pair_z_score')
-            self.settings_pair_feature = {'pair_symbol':self.pair_symbol,'window':window, 'z_threshold':z_threshold}  
-            
+            self.settings_pair_feature = {'pair_symbol':self.pair_symbol,'window':window, 'z_threshold':z_threshold}
+
         if plot:
             pvalue = round(adfuller(z_score.dropna().values)[1],4)
             print(f'p value of the rolling z-score is {pvalue}')
 
             fig, axs = plt.subplots(2, 2,figsize=(17,11))
 
             axs[0,0].axhline(y=2, color='r', linestyle='--')
             axs[0,0].axhline(y=-2, color='r', linestyle='--')
             axs[0,0].axhline(y=1.1, color='grey', linestyle='--')
             axs[0,0].axhline(y=-1.1, color='grey', linestyle='--')
             axs[0,0].axhline(y=0, color='blue', linestyle='-.')
             axs[0,0].plot(self.df.pair_z_score)
             axs[0,0].set_title('z score from the spread')
-            
+
             axs[0,1].plot(self.df['Date'],self.df['pair_spread'])
             axs[0,1].plot(self.df['Date'],np.where(self.df['signal_low_pair_z_score'] == 1, self.df['pair_spread'], np.nan),'o-r',color = 'red')
             axs[0,1].plot(self.df['Date'],np.where(self.df['signal_up_pair_z_score'] == 1, self.df['pair_spread'], np.nan),'o-r',color = 'green')
             axs[0,1].axhline(y=0, color='blue', linestyle='-.')
             axs[0,1].set_title('pair_sprear_plot')
 
             plot_acf(self.df['pair_z_score'].dropna(),lags=25, ax=axs[1,0])
             axs[1,0].set_title('acf pair_z_score')
-            
+
             plot_pacf(self.df['pair_z_score'].dropna(),lags=25, ax=axs[1,1])
             axs[1,1].set_title('pacf pair_z_score')
-            
+
             plt.show()
 
     #######################
     #### to be deprecated ####
     def get_count_feature(self, rolling_window, threshold, plot = False, save_features = False):
 
         # negative countiing and rolling countingng
@@ -721,31 +1171,44 @@
 
         mean = self.df['roll_pos_counting'].mean()
         std = self.df['roll_pos_counting'].std()
         self.df['norm_counting'] =  (self.df['roll_pos_counting'] - mean )/std
 
         self.df['signal_up_roll_pos_counting'] = np.where((self.df['norm_counting'] > threshold),1,0)
         self.df['signal_low_roll_pos_counting'] = np.where((self.df['norm_counting'] < -threshold),1,0)
-        
+
         if save_features:
             self.features.append('roll_pos_counting')
             self.signals.append('signal_up_roll_pos_counting')
             self.signals.append('signal_low_roll_pos_counting')
-            self.settings_count_features = {'rolling_window':rolling_window, 'threshold':threshold}  
-            
+            self.settings_count_features = {'rolling_window':rolling_window, 'threshold':threshold}
+
         if plot:
             fig = plt.figure(figsize = (10,4))
             plt.plot(self.df['Date'],self.df.norm_counting)
             plt.axhline(y=threshold, color='grey', linestyle='--')
             plt.axhline(y=-threshold, color='grey', linestyle='--')
             plt.show()
     #######################
-    
+
     def bidirect_count_feature(self, rolling_window, threshold, plot = False, save_features = False):
-    
+        """
+        perform negative and positive return counting in a given rolling time window
+
+        Parameters
+        ----------
+        rolling_window (int): window to apply to positive and negative returns
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'bidirect_counting'
         # negative countiing and rolling countingng
         self.df['RetClose'] = self.df['Close'].pct_change()
         self.df['roll_pos_counting'] = np.where(self.df['RetClose'].shift(1) > 0,1,0 )
         self.df['roll_pos_counting'] = self.df['roll_pos_counting'].rolling(window = rolling_window).sum()
 
         self.df['roll_neg_counting'] = np.where(self.df['RetClose'].shift(1) <= 0,1,0 )
@@ -753,15 +1216,15 @@
 
         self.df[feature_name] = np.where(self.df['roll_pos_counting'] > self.df['roll_neg_counting'], self.df['roll_pos_counting'], -self.df['roll_neg_counting'])
 
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
-            self.settings_bidirect_count_features = {'rolling_window':rolling_window, 'threshold':threshold}  
+            self.settings_bidirect_count_features = {'rolling_window':rolling_window, 'threshold':threshold}
 
         if plot:
             fig = plt.figure(figsize = (10,4))
             plt.plot(self.df['Date'],self.df[f'norm_{feature_name}'])
             plt.plot(self.df['Date'],self.df[f'upper_{feature_name}'], linestyle='--')
             plt.plot(self.df['Date'],self.df[f'lower_{feature_name}'], linestyle='--')
             plt.show()
@@ -779,20 +1242,20 @@
         self.df[f'std_norm_dist_range'] = (self.df.sort_values("Date")["norm_dist_range"].transform(lambda x: x.rolling(window, min_periods=1).std()))
 
         self.df['up_bound_norm_dist_range'] = up_threshold*self.df['std_norm_dist_range'] + mean_
         self.df['low_bound_norm_dist_range'] = -low_threshold*self.df['std_norm_dist_range'] + mean_
 
         self.df['signal_up_dist_range'] = np.where(self.df['norm_dist_range'] > self.df['up_bound_norm_dist_range'],1,0 )
         self.df['signal_low_dist_range'] = np.where(self.df['norm_dist_range'] < self.df['low_bound_norm_dist_range'],1,0 )
-        
+
         if save_features:
             self.features.append('dist_range')
             self.signals.append('signal_up_dist_range')
             self.signals.append('signal_low_dist_range')
-            self.settings_price_range = {'window':window, 'up_threshold':up_threshold, 'low_threshold':low_threshold} 
+            self.settings_price_range = {'window':window, 'up_threshold':up_threshold, 'low_threshold':low_threshold}
 
         if plot:
             fig, axs = plt.subplots(2, 2,figsize=(17,11))
 
             axs[0,0].plot(self.df['Range'])
             axs[0,0].set_title('range')
 
@@ -800,17 +1263,30 @@
             axs[0,1].set_title('Avg_range')
 
             axs[1,0].plot(self.df['up_bound_norm_dist_range'],color = 'grey', linestyle='--')
             axs[1,0].plot(self.df['low_bound_norm_dist_range'],color = 'grey', linestyle='--')
             axs[1,0].plot(self.df['norm_dist_range'])
             axs[1,0].set_title('norm_dist_range')
     #######################
-    
+
     def get_relative_range_feature(self, window, threshold, plot = False, save_features = False):
-    
+        """
+        perform relative spread of opening and closing price
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'CO_Range'
         self.df[feature_name] = self.df["Close"] / self.df["Open"]-1
         self.df[f'norm_{feature_name}'] = (self.df[feature_name] - self.df[feature_name].mean())/ self.df[feature_name].std()
 
         mean_ = self.df[f'norm_{feature_name}'].mean()
         self.df[f'std_norm_{feature_name}'] = (self.df.sort_values("Date")[f'norm_{feature_name}'].transform(lambda x: x.rolling(window, min_periods=1).std()))
 
@@ -818,15 +1294,15 @@
         self.df[f'low_bound_norm_{feature_name}'] = -threshold*self.df[f'std_norm_{feature_name}'] + mean_
 
         self.df[f'signal_up_{feature_name}'] = np.where(self.df[f'norm_{feature_name}'] > self.df[f'up_bound_norm_{feature_name}'],1,0 )
         self.df[f'signal_low_{feature_name}'] = np.where(self.df[f'norm_{feature_name}'] < self.df[f'low_bound_norm_{feature_name}'],1,0 )
 
         if save_features:
             self.log_features_standard(feature_name)
-            self.settings_relative_price_range = {'window':window, 'threshold':threshold} 
+            self.settings_relative_price_range = {'window':window, 'threshold':threshold}
 
         if plot:
             fig, axs = plt.subplots(1, 2,figsize=(14,5))
 
             axs[0].plot(self.df[feature_name])
             axs[0].set_title(feature_name)
 
@@ -836,15 +1312,15 @@
             axs[1].set_title(f'norm_{feature_name}')
 
     #######################
     #### to be deprecated ####
     def rsi_feature(self, window, lag_rsi_ret, threshold, plot = False, save_features = False):
 
         rsi = RSIIndicator(close = self.df['Close'], window = window).rsi()
-        self.df['RSI'] = rsi 
+        self.df['RSI'] = rsi
         self.df['RSI_ret'] = self.df['RSI']/self.df['RSI'].shift(lag_rsi_ret)
 
         mean = self.df['RSI_ret'].mean()
         std = self.df['RSI_ret'].std()
         self.df['norm_RSI_ret'] = (self.df['RSI_ret']-mean)/std
         self.df['signal_up_RSI_ret'] = np.where(self.df['norm_RSI_ret'] > threshold,1,0)
         self.df['signal_low_RSI_ret'] = np.where(self.df['norm_RSI_ret'] < -threshold,1,0)
@@ -866,28 +1342,42 @@
             axs[1].set_title('acf RSI_ret')
 
             plot_pacf(self.df['RSI_ret'].dropna(),lags=25,ax = axs[2])
             axs[2].set_title('pacf RSI_ret')
 
             fig.show()
     #######################
-    
+
     def rsi_feature_improved(self, window, threshold, plot = False, save_features = False):
+        """
+        perform relative strength index
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'RSI'
         rsi = RSIIndicator(close = self.df['Close'], window = window).rsi()
         self.df[feature_name] = rsi.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_rsi_feature_v2 = {'window':window, 'threshold':threshold}
 
         if plot:
             self.signal_plotter(feature_name)
-            
+
     #######################
     #### to be deprecated ####
     def days_features(self, window_day, limit, plot = False, save_features = False):
 
         self.df['dow'] = self.df.Date.dt.dayofweek
         self.df['dow'] = self.df['dow'].astype('str')
 
@@ -912,29 +1402,42 @@
             self.signals.append('signal_up_target_mean_input')
             self.signals.append('signal_low_target_mean_input')
             self.settings_days_features = {'window_day':window_day, 'limit':limit}
 
         if plot:
             fig, axs = plt.subplots(1, 3,figsize=(17,5))
 
-            axs[0].plot(self.df['norm_dow_input']) 
+            axs[0].plot(self.df['norm_dow_input'])
             axs[0].plot(self.df['up_dow_input'], linestyle='--')
             axs[0].plot(self.df['low_dow_input'], linestyle='--')
 
             plot_acf(self.df['norm_dow_input'].dropna(),lags=25,ax = axs[1])
             axs[1].set_title('acf day feature')
 
             plot_pacf(self.df['norm_dow_input'].dropna(),lags=25,ax = axs[2])
             axs[2].set_title('pacf day feature')
 
             fig.show()
     #######################
-    
+
     def days_features_bands(self, window, threshold, plot = False, save_features = False):
+        """
+        compute mean returns for a given day of the week in a window scope per day 
 
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         self.df['dow'] = self.df.Date.dt.dayofweek
         self.df['dow'] = self.df['dow'].astype('str')
 
         feature_name = 'target_mean_dow'
 
         self.df[feature_name] = (self.df.sort_values("Date").groupby('dow')['roll_mean_log_return'].transform(lambda x: x.rolling(window, min_periods=1).mean()))
 
@@ -943,19 +1446,19 @@
         if save_features:
 
             self.log_features_standard(feature_name)
             self.settings_days_features_v2 = {'window':window, 'threshold':threshold}
 
         if plot:
             self.signal_plotter(feature_name)
-            
+
     #######################
     #### to be deprecated ####
     def analysis_volume(self,lag_volume, threshold, window, plot = False, save_features = False):
-    
+
         self.df['log_Volume'] = np.log(self.df['Volume'])
         self.df['ret_log_Volume'] = self.df['log_Volume'].pct_change(lag_volume)
 
         self.df['norm_ret_log_Volume'] = (self.df['ret_log_Volume'] - self.df['ret_log_Volume'].mean())/ self.df['ret_log_Volume'].std()
         mean_ = self.df['norm_ret_log_Volume'].mean()
         self.df[f'std_norm_ret_log_Volume'] = (self.df.sort_values("Date")["norm_ret_log_Volume"].transform(lambda x: x.rolling(window, min_periods=1).std()))
 
@@ -999,17 +1502,30 @@
             axs[0].set_title('norm_ret_log_Volume')
 
             axs[1].plot(self.df.Date, self.df.std_norm_ret_log_Volume)
             axs[1].set_title('std_norm_ret_log_Volume')
 
             plt.show()
     #######################
-    
+
     def analysis_smooth_volume(self, window, threshold, plot = False, save_features = False):
-    
+        """
+        compute feature of thrading volumes
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'smooth_Volume'
         self.df[feature_name] = np.log(self.df['Volume'])
         # self.df[feature_name] = self.df['log_Volume'].rolling(window).mean()
 
         self.df[f'roll_mean_{feature_name}'] = self.df[feature_name].rolling(window).mean()
         self.df[f'roll_std_{feature_name}'] = self.df[feature_name].rolling(window).std()
 
@@ -1035,132 +1551,232 @@
 
             plt.show()
 
             print('--------------------------------------------------------------')
 
             fig, axs = plt.subplots(1,2,figsize=(10,4))
 
-            axs[0].plot(self.df[f'{feature_name}']) 
+            axs[0].plot(self.df[f'{feature_name}'])
             axs[0].set_title(f'{feature_name}')
 
             axs[1].plot(self.df[f'z_{feature_name}'], linestyle='--')
             axs[1].set_title(f'z_{feature_name}')
 
             plt.show()
 
     def roc_feature(self, window, threshold, plot = False, save_features = False):
+        """
+        perform price rate of change
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'ROC'
         roc = ROCIndicator(close = self.df['Close'], window = window).roc()
         self.df[feature_name] = roc.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_roc_feature = {'window':window, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
-    
+
     def stoch_feature(self, window, smooth1, smooth2, threshold, plot = False, save_features = False):
+        """
+        perform stochastic oscilator RSI feature
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        smooth1 (int): smoothing parameter 1
+        smooth2 (int): smoothing parameter 2
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'STOCH'
         stoch = StochRSIIndicator(close = self.df['Close'], window = window, smooth1=smooth1, smooth2=smooth2).stochrsi()
         self.df[feature_name] = stoch.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_stoch_feature = {'window':window, 'smooth1':smooth1, 'smooth2':smooth2, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def stochastic_feature(self, window, smooth, threshold, plot = False, save_features = False):
+        """
+        perform stochastic oscilator feature
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        smooth (int): smoothing parameter 
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'STOCHOSC'
         stochast = StochasticOscillator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], window = window,smooth_window=smooth).stoch()
         self.df[feature_name] = stochast.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_stochastic_feature = {'window':window, 'smooth':smooth,'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def william_feature(self, lbp, threshold, plot = False, save_features = False):
+        """
+        perfom fast stochastic oscilator or william indicator
+
+        Parameters
+        ----------
+        lbp (int): look back parameter
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'WILL'
-        will = WilliamsRIndicator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], lbp = lbp).williams_r() 
+        will = WilliamsRIndicator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], lbp = lbp).williams_r()
         self.df[feature_name] = will.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_william_feature = {'lbp':lbp,'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def vortex_feature(self, window, threshold, plot = False, save_features = False):
+        """
+        perform vortex oscilator
+
+        Parameters
+        ----------
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         feature_name = 'VORTEX'
         vortex = VortexIndicator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], window = window).vortex_indicator_diff()
         self.df[feature_name] = vortex.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_vortex_feature = {'window':window, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def pair_index_feature(self, pair_symbol, feature_label, window, threshold, plot = False, save_features = False):
+        """
+        perform additional asset ROC feature, then a new feature is created in the main dataframe
+
+        Parameters
+        ----------
+        pair_symbol (str): symbol of the asset to extract the data
+        feature_label (str): name of the resulting feature
+        window (int): window to apply to the feature
+        threshold (float): alpha or z thrsholds for the normalized feature
+        plot (boolean): True to display plot
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         self.pair_index = pair_symbol
         begin_date = self.today - relativedelta(days = self.n_days)
         begin_date_str = begin_date.strftime('%Y-%m-%d')
-        
+
         if feature_label in self.df.columns:
             self.df = self.df.drop(columns = [feature_label])
 
         stock = yf.Ticker(self.pair_index)
         df = stock.history(period=self.data_window)
         df = df.sort_values('Date')
         df.reset_index(inplace=True)
         df['Date'] = pd.to_datetime(df['Date'], format='mixed',utc=True).dt.date
         df['Date'] = pd.to_datetime(df['Date'])
         df = df[df.Date >= begin_date_str ]
         self.pair_index_df = df
-        
+
         #### converting the same index ####
         dates_vector = self.df.Date.to_frame()
         self.pair_index_df = dates_vector.merge(self.pair_index_df, on ='Date',how = 'left')
         self.pair_index_df = self.pair_index_df.fillna(method = 'bfill')
         self.pair_index_df = self.pair_index_df.fillna(method = 'ffill')
-        
+
         self.pair_index_df[feature_label] = ROCIndicator(close = self.pair_index_df['Close'], window = window).roc()
         df_to_merge = self.pair_index_df[['Date',feature_label]]
         self.df = self.df.merge(df_to_merge, on ='Date',how = 'left')
 
         ########
         self.compute_clip_bands(feature_label,threshold)
 
         if save_features:
             self.log_features_standard(feature_label)
             parameters = {feature_label:{'pair_symbol':pair_symbol, 'feature_label':feature_label, 'window':window,'threshold':threshold}}
-            try: 
+            try:
                 len(self.settings_pair_index_feature)
                 print('existing')
                 self.settings_pair_index_feature.append(parameters)
             except:
                 print('creation')
                 self.settings_pair_index_feature = list()
                 self.settings_pair_index_feature.append(parameters)
 
         if plot:
             self.signal_plotter(feature_label)
 
     def produce_order_features(self, feature_name, save_features = False):
+        """
+        perform a feature that captures high and low values in an index. this is usefull to know duration/persistence of a signal
 
+        Parameters
+        ----------
+        feature_name (str): name of the feature
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
         signal_feature_name = f'discrete_signal_{feature_name}'
         order_feature_name = f'order_signal_{feature_name}'
-        
+
         self.df[signal_feature_name] = np.where(
             self.df[f'signal_up_{feature_name}'] == 1,1,
             np.where(
                 self.df[f'signal_low_{feature_name}'] == 1,-1,0
             )
         )
 
@@ -1169,55 +1785,83 @@
         self.df['breack'] = np.where(self.df[f'lag_{signal_feature_name}'] != self.df[signal_feature_name],1,0)
         self.df["chain_id"] = self.df.groupby("breack")["Date"].rank(method="first", ascending=True)
         self.df["chain_id"] = np.where(self.df['breack'] == 1,self.df["chain_id"],np.nan)
         self.df["chain_id"] = self.df["chain_id"].fillna(method='ffill')
         self.df[order_feature_name] = self.df.groupby('chain_id')["Date"].rank(method="first", ascending=True)
         self.df[order_feature_name] = self.df[order_feature_name]*self.df[signal_feature_name]
         self.df = self.df.drop(columns = [f'lag_{signal_feature_name}', 'breack', "chain_id"])
-        
+
         ## saving features
         if save_features:
             self.signals.append(signal_feature_name)
             self.signals.append(order_feature_name)
-            
+
     def create_hmm_derived_features(self, lag_returns):
-        
+        """
+        create features derived from hmm states features. Features are the index of the state, the duration of the state, chain raturn
+
+        Parameters
+        ----------
+        lag_returns (int): lag paramter (not used)
+        
+        Returns
+        -------
+        None
+        """
         self.df = self.df.sort_values('Date')
         ## indexing chains
         self.df['lag_hmm_feature'] = self.df['hmm_feature'].shift(1)
         self.df['breack'] = np.where(self.df['lag_hmm_feature'] != self.df['hmm_feature'],1,0)
         self.df["chain_id"] = self.df.groupby("breack")["Date"].rank(method="first", ascending=True)
         self.df["chain_id"] = np.where(self.df['breack'] == 1,self.df["chain_id"],np.nan)
         self.df["chain_id"] = self.df["chain_id"].fillna(method='ffill')
         self.df["hmm_chain_order"] = self.df.groupby('chain_id')["Date"].rank(method="first", ascending=True)
-        
+
         ### returns using the first element in a chain
         self.df['first'] = np.where(self.df['hmm_chain_order'] == 1, self.df['Close'], np.nan)
         self.df['first'] = self.df.sort_values('Date')['first'].fillna(method='ffill')
         self.df['chain_return'] = (self.df['Close']/self.df['first'] -1) * 100
 
         self.df = self.df.drop(columns = ['breack','first'])
 
     def cluster_hmm_analysis(self, n_clusters,features_hmm, test_data_size, seed, lag_returns_state=7, plot = False, save_features = False, model = False):
+        """
+        create or use a hmm model
+
+        Parameters
+        ----------
+        n_clusters (int): number of clusters or states to calculate
+        features_hmm (list): features to be considered in hmm model when training
+        test_data_size (int): size of the test data. Note that the remaining is going to be used as training data
+        seed (int): seed for the model inizialization
+        lag_returns_state (int) : lags for returns of the state
+        plot (boolean): True to display hmm states analysis
+        save_features (boolean): True to save features and configurations
+        model (obj): if provided, no model will be trainend and the provided model will be used to get hmm features
+        
+        Returns
+        -------
+        None
+        """
         if not model:
-            
+
             df_new = self.df
             pipeline_hmm = Pipeline([
                 ('selector', FeatureSelector(columns=features_hmm)),
                 ('fillna', MeanMedianImputer(imputation_method='median',variables=features_hmm)),
                 ('hmm',GaussianHMM(n_components =  n_clusters, covariance_type = 'full', random_state = seed))
                 ])
             data_train = df_new.iloc[:-test_data_size,:]
             data_test = df_new.iloc[-test_data_size:,:]
 
             pipeline_hmm.fit(data_train)
 
             self.model_hmm = pipeline_hmm
             self.test_data_hmm = data_test
-            
+
             ### first feature: the hidden state
             self.df['hmm_feature'] = self.model_hmm.predict(self.df)
             self.create_hmm_derived_features(lag_returns = lag_returns_state)
 
             ## completion
 
             hidden_states = pipeline_hmm.predict(data_train)
@@ -1226,19 +1870,19 @@
 
             data_train['HMM'] = hidden_states
             data_train['HMM_state'] =  data_train['HMM'].map(map_)
 
             hidden_states = pipeline_hmm.predict(data_test)
             data_test['HMM'] = hidden_states
             data_test['HMM_state'] =  data_test['HMM'].map(map_)
-            
+
         if model:
             self.df['hmm_feature'] = model.predict(self.df)
             self.create_hmm_derived_features(lag_returns = lag_returns_state)
-            
+
         if save_features:
             self.features.append('hmm_feature')
             self.features.append('hmm_chain_order')
             self.settings_hmm = {'n_clusters':n_clusters,'features_hmm':features_hmm, 'test_data_size':test_data_size, 'seed':seed,'lag_returns_state':lag_returns_state }
 
         if plot:
 
@@ -1259,22 +1903,46 @@
                 dfi = data_test[data_test['HMM_state'] == state]
                 hmm_id = dfi['HMM'].unique()[0]
                 fig.add_trace(go.Scatter(x=dfi['Date'], y=dfi['Close'], mode='markers',name = state, marker_color = color_map[hmm_id]))
             fig.update_layout(height=500, width=1200)
             fig.show()
 
     def sharpe_ratio(self, return_series, n_trad_days = 255, rf = 0.01):
+        """
+        perform sharpe ratio of a given time series return
+
+        Parameters
+        ----------
+        return_series (pd.series): time series of the returns
+        n_trad_days (int): trading days to anualize returns
+        rf (float): anual free risk rate
+        
+        Returns
+        -------
+        sharpe_ratio (float): sharpe ratio 
+        """
         nsqrt = np.sqrt(n_trad_days)
         mean = return_series.mean() * n_trad_days
         sigma = return_series.std() * nsqrt
         sharpe_ratio = round((mean-rf)/sigma,2)
         return sharpe_ratio
-    
+
     def treat_signal_strategy(self,test_data, strategy):
-    
+        """
+        helper method that treats signals and converts signals to 1 or 0
+
+        Parameters
+        ----------
+        test_data (pd.DataFrame): test data
+        strategy (list): features to get the strategy
+        
+        Returns
+        -------
+        test_data (pd.DataFrame): test data with extra columns that are the strategy (main_signal)
+        """
         hmm_states_list = [x for x in strategy if 'hmm_state_' in x]
         other_features = [x for x in strategy if x not in hmm_states_list]
 
         test_data['hmm_signal'] = 0
         test_data['features_signal'] = 0
         test_data['main_signal'] = 0
 
@@ -1295,18 +1963,29 @@
 
         elif len(hmm_states_list) > 0 and len(other_features) == 0:
             test_data['main_signal'] = np.where((test_data['features_signal'] == 0) & (test_data['hmm_signal'] == 1),1,0)
 
         elif len(hmm_states_list) == 0 and len(other_features) > 0:
             test_data['main_signal'] = np.where((test_data['features_signal'] == 1) & (test_data['hmm_signal'] == 0),1,0)
 
-        return test_data  
+        return test_data
 
     def stategy_simulator(self, features, hmm_feature = True):
+        """
+        execute strategy and get some performance metrics like sharpe ratio, return. This method creates some new attributes
 
+        Parameters
+        ----------
+        features (list): list of features to be tested as strategies
+        hmm_feature (boolean): include hmm feature
+        
+        Returns
+        -------
+        None
+        """
         columns_ = ['Date', 'Close','Open'] + features + ['HMM']
         states = list(self.df.hmm_feature.unique())
         states.sort()
         test_data = self.test_data_hmm[columns_]
 
         ## benchmark return
         test_data['lrets_bench'] = np.log(test_data['Close']/test_data['Close'].shift(1))
@@ -1368,16 +2047,27 @@
 
             }
             df_returns_log = pd.DataFrame(returns_log).T.sort_values('strat_rets', ascending = False)
 
         self.strategy_log = df_returns_log
         self.best_strategy =  df_returns_log.iloc[0,:].strategy
         self.top_10_strategy = list(df_returns_log.iloc[0:10,:].strategy.values)
-        
+
     def viz_strategy(self, strategy):
+        """
+        display analysis plot of a given strategy
+
+        Parameters
+        ----------
+        strategy (list): list of features of the strategy
+        
+        Returns
+        -------
+        None
+        """
         test_data = self.test_data_strategy
 
         test_data = self.treat_signal_strategy(test_data, strategy)
 
         ## strategy return
         # test_data['lrets_strat'] = np.log(test_data['Open'].shift(-1)/test_data['Open']) * test_data['main_signal']
         test_data['lrets_strat'] = np.log(test_data['Close'].shift(-1)/test_data['Close']) * test_data['main_signal']
@@ -1404,15 +2094,15 @@
         plt.plot(test_data['bench_prod_exp'], label= 'benchmark')
         plt.plot(test_data['strat_prod_exp'], label= 'strategy')
         plt.legend()
         plt.show()
 
     ### deprecated ############################
     def create_strategy(self, favourable_states):
-
+        
         test_data = self.test_data_hmm
         # add MA signal
         test_data.loc[test_data[self.ma1_column] > test_data[self.ma2_column], 'MA_signal'] = 1
         test_data.loc[test_data[self.ma1_column] <= test_data[self.ma2_column], 'MA_signal'] = 0
 
         # add hnn signal
 
@@ -1448,24 +2138,35 @@
         print(f'sharpe strategy {strat_sharpe}')
 
         fig = plt.figure(figsize = (10,4))
         plt.plot(test_data['bench_prod_exp'])
         plt.plot(test_data['strat_prod_exp'])
         self.settings_hmm_states = {'favourable_states':favourable_states}
     ################################################
-    
+
     def deep_dive_analysis_hmm(self, test_data_size, split = 'train'):
-    
+        """
+        display analysis plot hmm model
+
+        Parameters
+        ----------
+        test_data_size (int): test data size, the remaining is the train data
+        split (str): options (train or test). Split type to assess
+        
+        Returns
+        -------
+        None
+        """
         if split == 'train':
             df = self.df.iloc[:-test_data_size,:]
         elif split == 'test':
             df = self.df.iloc[-test_data_size:,:]
 
         ## returns plot
-        fig = px.box(df.sort_values('hmm_feature'), y = 'chain_return',x = 'hmm_feature', color = 'hmm_feature', 
+        fig = px.box(df.sort_values('hmm_feature'), y = 'chain_return',x = 'hmm_feature', color = 'hmm_feature',
                     height=400, width=1000, title = 'returns chain hmm feature')
         fig.add_shape(type='line',x0=-0.5,y0=0,x1=max(df.hmm_feature)+0.5,y1=0,line=dict(color='grey',width=1),xref='x',yref='y')
         fig.show()
         print('--------------------------------------------------------------')
         ## time series plot
         fig = px.line(
             df.sort_values(['hmm_feature','hmm_chain_order']),
@@ -1486,28 +2187,51 @@
         ax.set_xlabel('State To')
         ax.set_ylabel('State From')
         fig.show()
         print('--------------------------------------------------------------')
         del df
 
     def get_targets(self, steps):
+        """
+        produce regression target return taking future prices
+
+        Parameters
+        ----------
+        steps (int): number of lags and steps for future returns
+        
+        Returns
+        -------
+        None
+        """
         self.targets = list()
         self.target = list()
         columns = list()
         for i in range(1,steps+1):
             self.df[f'target_{i}'] = self.df.log_return.shift(-i)
             self.targets.append(f'target_{i}')
             columns.append(f'target_{i}')
 
         self.df[f'mean_target'] = self.df[columns].mean(axis=1)
         self.target.append(f'mean_target')
         self.settings_target_lasts = {'steps':steps, 'type':'regression'}
-        
+
     def get_categorical_targets(self, horizon, flor_loss, top_gain):
-    
+        """
+        produce binary target return taking future prices. it produce two targets, one for high returns and another for low returns
+
+        Parameters
+        ----------
+        horizon (int): number of lags and steps for future returns
+        flor_loss (float): min loss return
+        top_gain (float): max gain return
+
+        Returns
+        -------
+        None
+        """
         self.target = list()
         self.targets = list()
         columns = list()
 
         ## loops
         for i in range(1,horizon+1):
             self.df[f'target_{i}'] = self.df.High.shift(-i)
@@ -1531,209 +2255,465 @@
 
         self.targets.append('target_up')
         self.targets.append('target_down')
 
         self.settings_target_lasts = {'horizon':horizon, 'flor_loss':flor_loss, 'top_gain':top_gain, 'type': 'classification'}
 
     def get_configurations(self,test_data_size =250, val_data_size = 250, model_type = False):
-        
+        """
+        produce configuration dictionary that were saved in the feature generation methods if save_features was activated
+
+        Parameters
+        ----------
+        test_data_size (int): test data size
+        val_data_size (int): validation data size 
+        model_type (str): model type, options: 'Forecaster','Classifier'
+
+        Returns
+        -------
+        None
+        """
         self.settings = {
             'features':list(set(self.features)),
             'signals' :list(set(self.signals)),
             'test_data_size': test_data_size,
             'val_data_size': val_data_size,
             'settings' : {
                 'general' : self.settings_general,
                 'volatility' : self.settings_volatility,
                 'outlier': self.settings_outlier,
             }
         }
-        
+
         if model_type in ['Forecaster','Classifier']:
-            
+
             target_list = list(set(self.targets))
             target_list.sort()
             self.settings['model_type'] = model_type
             self.settings['target'] = list(set(self.target))
             self.settings['targets'] = target_list
-        
+
         ## for now this is hard coded
         feature_list = ['spread_ma','relative_spread_ma','pair_feature','count_features','bidirect_count_features','price_range','relative_price_range','rsi_feature',
                         'rsi_feature_v2', 'days_features','days_features_v2', 'volume_feature','smooth_volume', 'roc_feature', 'stoch_feature', 'stochastic_feature',
                         'william_feature', 'vortex_feature', 'pair_index_feature','hmm']
 
         for feature in feature_list:
             try:
                 self.settings['settings'][feature] = getattr(self, f'settings_{feature}')
             except:
                 pass
         try:
             self.settings['settings']['target_lasts'] = self.settings_target_lasts
         except:
             pass
-        
+
         try:
             self.settings['settings']['strategies'] = {
                 'best_strategy':self.best_strategy,
                 'top_10_strategies': self.top_10_strategy
             }
         except:
             pass
 
 class produce_model:
+    """
+    Class that produces a machine learning model in a scikit-learn pipeline wrapper.
+
+    Attributes
+    ----------
+    data  : pd.DataFrame
+        symbol of the asset
+    X_train : pd.DataFrame
+    y_train : pd.Series
+    X_test : pd.DataFrame
+    y_test : pd.Series
+    X_val : pd.DataFrame
+    y_val : pd.Series
+    pipeline : obj
+        trained pipeline that includes a ml model
+    features_to_model: list
+        features in end step of the pipeline
+
+    Methods
+    -------
+    preprocess(test_data_size=int, target=str, val_data_size=int):
+        prepare data, split train, test, validation data and X and Y
+    get_sample(x=pd.DataFrame, sample=int, max_=int):
+        sample data
+    """
     def __init__(self,data):
+        """
+        Initialize object
+
+        Parameters
+        ----------
+        data (pd.DataFrame): data
+
+        Returns
+        -------
+        None
+        """
         self.data = data.copy()
-    
+
     def preprocess(self, test_data_size, target, val_data_size = False):
-        
+        """
+        prepare data, split train, test, validation data and X and Y
+
+        Parameters
+        ----------
+        test_data_size (int): test data size
+        target (str): target column
+        val_data_size (int): validation data size
+
+        Returns
+        -------
+        None
+        """
         train_data, test_data = self.data.iloc[:-test_data_size,:].dropna() , self.data.iloc[-test_data_size:,:].dropna()
-        
+
         if val_data_size:
             train_data, val_data = train_data.iloc[:-val_data_size,:], train_data.iloc[-val_data_size:,:]
-            
+
         self.test_data = test_data
-        
+
         X_train, y_train = train_data.iloc[0:,1:], train_data[target]
         X_test, y_test = test_data.iloc[0:,1:], test_data[target]
         self.X_train = X_train
         self.y_train = y_train
         self.X_test = X_test
         self.y_test = y_test
-        
+
         if val_data_size:
             X_val, y_val = val_data.iloc[0:,1:], val_data[target]
             self.X_val = X_val
             self.y_val = y_val
-        
+
     def get_sample(self, x, sample, max_=900):
+        """
+        sample data
+
+        Parameters
+        ----------
+        x (pd.DataFrame): input data
+        sample (int): sample size
+        max_ (int): max sample
+
+        Returns
+        -------
+        sample (float): sample size
+        """
         length = len(x)
         if length > max_:
             return 1.0
         else:
             return sample
-    
+
     def train_model(self, pipe, model, cv_ = False):
+        """
+        train pipeline
+
+        Parameters
+        ----------
+        pipe (obj): pipeline object
+        model (obj): model object
+        cv_ (obj): cross validation procedure
+
+        Returns
+        -------
+        sample (float): sample size
+        """
         self.model = model
         self.pipe_transform = pipe
         self.pipeline = Pipeline([('pipe_transform',self.pipe_transform), ('model',self.model)])
         self.features_to_model = self.pipe_transform.fit_transform(self.X_train).columns
         self.pipeline.fit(self.X_train, self.y_train)
-        
-        
+
+
 class hmm_feature_selector():
-    
+    """
+    class that is going to train hmm models to perform feature selection
+
+    Attributes
+    ----------
+    data  : pd.DataFrame
+        symbol of the asset
+    n_clusters : int
+        number of clusters to search
+    init_features_hmm : list
+        list of features to consider in the search
+    test_data_size :int
+        test data size, meaning that the remaining is going to be used as training data
+    select_n_features : int
+        number of features to select
+    n_trials : int
+        total number of trials per combination
+    limit_search : int
+        limit number of combinations
+    default_benchmark_sd : float
+        default value to bias standard deviation
+    t_threshold : float
+        alpha or z threshold
+    pipeline_hmm: obj
+        pipeline object of the hmm model
+    features_used_in_model:list
+        features in model
+    train_model(features_hmm=list):
+        train hmm model
+    feature_combinations: list
+        list of combination of features
+    mean_relevance: float
+        relevance score of the model
+    best_features: list
+        list of best performing features
+
+    Methods
+    -------
+    split_data():
+        split data in train and test
+    train_model(features_hmm=list):
+        train hmm model
+    feature_list_generator():
+        perform combination of features
+    get_error():
+        get error or score of a given model using relevance score
+    execute_selector():
+        select the best combination of features
+    """
     def __init__(self, data, n_clusters, init_features_hmm, test_data_size, select_n_features, n_trials = 1,limit_search = False, default_benchmark_sd = 0.00003, t_threshold = 2):
+        """
+        Initialize object
+
+        Parameters
+        ----------
+        data (pd.DataFrame): data
+        n_clusters (int): number of clusters to search
+        init_features_hmm (list): list of features to consider in the search
+        test_data_siz:(int:  test data size, meaning that the remaining is going to be used as training data
+        select_n_features (int): number of features to select
+        n_trials (int): total number of trials per combination
+        limit_search (int): limit number of combinations
+        default_benchmark_sd (float): default value to bias standard deviation
+        t_threshold (float): alpha or z threshold
+
+        Returns
+        -------
+        None
+        """
         self.data = data.copy()
         self.n_clusters = n_clusters
         self.init_features_hmm = init_features_hmm
         self.test_data_size = test_data_size
         self.select_n_features = select_n_features
         self.n_trials = n_trials
         self.limit_search= limit_search
         self.default_benchmark_sd = default_benchmark_sd
         self.t_threshold = t_threshold
-        
+
     def split_data(self):
-        
+        """
+        split data in train and test
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         self.data_train = self.data.iloc[:-self.test_data_size,:]
         self.data_test = self.data.iloc[-self.test_data_size:,:]
-        
+
     def train_model(self,features_hmm):
+        """
+        train hmm model
+
+        Parameters
+        ----------
+        features_hmm (list): list of features to be selected in the model
+
+        Returns
+        -------
+        None
+        """
         pipeline_hmm = Pipeline([
                 ('selector', FeatureSelector(columns=features_hmm)),
                 ('fillna', MeanMedianImputer(imputation_method='median',variables=features_hmm)),
                 ('hmm',GaussianHMM(n_components =  self.n_clusters, covariance_type = 'full'))
                 ])
-        
+
         self.pipeline_hmm = pipeline_hmm.fit(self.data_train)
         self.features_used_in_model = features_hmm
-        
+
     def feature_list_generator(self):
-        
+        """
+        perform combination of features
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         feature_combinations = set(list(combinations(self.init_features_hmm, self.select_n_features)))
         feature_combinations = list(map(list, feature_combinations))
-        
+
         self.feature_combinations = feature_combinations
-        
+
     def get_error(self):
-        
+        """
+        get error or score of a given model using relevance score
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         self.data_train_ = self.data_train.copy()
-        
+
         self.data_train_['hmm_feature'] = self.pipeline_hmm.predict(self.data_train_)
         self.data_train_ = self.data_train_[['Date','hmm_feature','Close']].sort_values('Date')
-        
+
         ## indexing chains
         self.data_train_['lag_hmm_feature'] = self.data_train_['hmm_feature'].shift(1)
         self.data_train_['breack'] = np.where(self.data_train_['lag_hmm_feature'] != self.data_train_['hmm_feature'],1,0)
         self.data_train_["chain_id"] = self.data_train_.groupby("breack")["Date"].rank(method="first", ascending=True)
         self.data_train_["chain_id"] = np.where(self.data_train_['breack'] == 1,self.data_train_["chain_id"],np.nan)
         self.data_train_["chain_id"] = self.data_train_["chain_id"].fillna(method='ffill')
         self.data_train_["hmm_chain_order"] = self.data_train_.groupby('chain_id')["Date"].rank(method="first", ascending=True)
-        
+
         ### returns using the first element in a chain
         self.data_train_['first'] = np.where(self.data_train_['hmm_chain_order'] == 1, self.data_train_['Close'], np.nan)
         self.data_train_['first'] = self.data_train_.sort_values('Date')['first'].fillna(method='ffill')
         self.data_train_['chain_return'] = (self.data_train_['Close']/self.data_train_['first'] -1) * 100
-        
+
         self.data_train_ = self.data_train_.drop(columns = ['first'])
-        
+
         mean_relevance, cluster_returns, number_relevant_states = states_relevance_score(self.data_train_)
         self.mean_relevance = mean_relevance
-        
+
     def execute_selector(self):
-        
+        """
+        select the best combination of features
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         self.split_data()
         self.feature_list_generator()
         maxi = -1
         print(f'it is expected {len(self.feature_combinations)} combinations')
         feature_results = dict()
-        
+
         if self.limit_search:
             print(f' taking just {self.limit_search} combinations')
             maxi = self.limit_search
-            
+
         for i,features_hmm in enumerate(self.feature_combinations[0:maxi]):
-    
+
             feature_results[f'group_{i}'] = {
                 'features':list(features_hmm),
                 'relevances':list()
             }
-            
+
             for _ in range(self.n_trials):
                 try:
                     self.train_model(features_hmm)
                     self.get_error()
                     feature_results[f'group_{i}']['relevances'].append(self.mean_relevance)
                 except:
                     print('error')
             feature_results[f'group_{i}']['mean relevance'] = np.mean(feature_results[f'group_{i}']['relevances'])
         self.feature_results = feature_results
         self.best_features = pd.DataFrame(self.feature_results).T.sort_values('mean relevance').iloc[-1,:].features
-        
+
 class signal_analyser_object:
-    
+    """
+    class that is going to analyse signals
+
+    Attributes
+    ----------
+    data  : pd.DataFrame
+        symbol of the asset
+    ticket_name :str
+        asset symbol
+    show_plot : boolean
+        if true show plot for every method
+    save_path : str
+        if true, save results in file
+    save_aws : str
+        if true, export results to remote repo
+    aws_credentials : dict
+        credentials for aws
+    return_fig : boolean
+        if true, methods will return objects
+    create_backtest_signal(days_strategy=list, test_size=int, feature_name=str, high_exit=float, low_exit=float):
+        perform backtest signal analysis
+        
+    Methods
+    -------
+    signal_analyser(test_size=int, feature_name=str, days_list=list, threshold=float,verbose=boolean, signal_position=boolean):
+        perform signal analysis and feature extraction
+
+    """
+
     def __init__(self, data,symbol_name, show_plot = True, save_path = False, save_aws = False, aws_credentials = False, return_fig = False):
         """
-        data: pandas df
-        symbol_name: str name of the asset
-        show_plot: bool
-        save_path: str local path for saving e.g r'C:/path/to/the/file/'
-        save_aws: str remote key in s3 bucket path e.g. 'path/to/file/'
-        aws_credentials: dict
-        return_fig: boolean return the image function as result
+        Initialize object
+
+        Parameters
+        ----------
+        data (pd.DataFrame): data
+        ticket_name (str): name of the asset
+        show_plot (boolean): if true show plot for every method
+        save_path (str): if true, save results in file e.g r'C:/path/to/the/file/'
+        save_aws (str): if true, export results to remote repo e.g. 'path/to/file/'
+        aws_credentials (dict): credentials for aws
+        return_fig (boolean): if true, methods will return objects
+
+        Returns
+        -------
+        None
         """
         self.data = data.copy()
         self.ticket_name = symbol_name
         self.show_plot = show_plot
         self.save_path = save_path
         self.save_aws = save_aws
         self.aws_credentials = aws_credentials
         self.return_fig = return_fig
 
     def signal_analyser(self, test_size, feature_name, days_list, threshold = 0.05,verbose = False, signal_position = False):
+        """
+        perform signal analysis and feature extraction
+
+        Parameters
+        ----------
+        test_size (int): test data size
+        feature_name (str): name of the feature to assess
+        days_list (list): list of integers [3,8,10] to assess
+        threshold (float): alpha or z threshold
+        verbose (boolean): print metrics
+        signal_position (int): if true, the signal is taken at the given step in the signal
+
+        Returns
+        -------
+        None
+        """
         data = self.data
         self.feature_name = feature_name
         up_signal, low_signal= f'signal_up_{feature_name}', f'signal_low_{feature_name}'
         features_base = ['Date', up_signal, low_signal, 'Close']
 
         df = data[features_base].sort_values('Date').iloc[0:-test_size,:]
         returns_list = list()
@@ -1741,18 +2721,18 @@
         for days in days_list:
 
             feature_ = f'return_{days}d'
             df[feature_] = (df['Close'].shift(-days)/df['Close']-1)*100
             returns_list.append(feature_)
 
         df['signal_type'] = np.where(
-            df[up_signal] == 1, 
-            'up', 
+            df[up_signal] == 1,
+            'up',
             np.where(
-                df[low_signal] == 1, 
+                df[low_signal] == 1,
                 'down',
                 None
             )
         )
         df = df[~df.signal_type.isna()]
         # df['Date'] = df.index
         df['lag_Date'] = df['Date'].shift(1)
@@ -1768,15 +2748,15 @@
         df['inv_internal_rn'] = df.sort_values(['Date'],ascending = False).groupby(['chain_id']).cumcount() + 1
 
         df['first_in_chain'] = np.where(df['internal_rn'] == 1, True, False)
         df['last_in_chain'] = np.where(df['inv_internal_rn'] == 1, True, False)
 
         df = df.drop(columns = ['break','span','lag_Date','inv_internal_rn']).sort_values('Date')
         self.df_signal = df
-        
+
         n_signals_up = len(list(df[df.signal_type == 'up'].chain_id.unique()))
         n_signals_down = len(list(df[df.signal_type == 'down'].chain_id.unique()))
         p_scores = list()
         medians_down = list()
         validations = list()
         if not signal_position: ### for now it is based on the last signal on a chain
             df_melt = df[df.last_in_chain == True].melt(id_vars=['signal_type'], value_vars=returns_list, var_name='time', value_name='value')
@@ -1784,15 +2764,15 @@
 
         for evalx in returns_list:
 
             sample1 = df_melt[(df_melt.time == evalx) & (df_melt.signal_type == 'up')].value.values
             sample2 = df_melt[(df_melt.time == evalx) & (df_melt.signal_type == 'down')].value.values
             pvalue = stats.ttest_ind(sample1, sample2).pvalue
             median_down = np.median(sample2)
-            median_up = np.median(sample1) 
+            median_up = np.median(sample1)
             validations.append(median_up < 0)
             validations.append(median_down > 0)
             p_scores.append(pvalue)
             medians_down.append(median_down)
         self.df_melt = df_melt
         null_ho_eval = threshold > np.mean(p_scores)
         mean_median_return = np.median(medians_down)  ## end metric
@@ -1826,18 +2806,18 @@
         axs[0].set_title('span between last signals')
         del df2
         sns.boxplot(data=df[df.last_in_chain == True], y="internal_rn",ax = axs[1])
         axs[1].set_title('signal duration distribution')
         sns.boxplot(data=df_melt, x="time", y="value", hue="signal_type",ax = axs[2])
         axs[2].axhline(y=0, color='grey', linestyle='--')
         axs[2].set_title('signal type expected returns distribution at different time lapses')
-            
+
         if self.show_plot:
             plt.show()
-            
+
         if self.save_path:
             result_plot_name = f'signals_strategy_distribution_{feature_name}.png'
             fig.savefig(self.save_path+result_plot_name)
             # pickle.dump(axs, open(self.save_path+result_plot_name, 'wb'))
 
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_plot_name, input_path = self.save_path+result_plot_name)
@@ -1845,248 +2825,363 @@
         if not self.show_plot:
             plt.close()
 
         del df
 
         if self.return_fig:
             return fig
-        
+
     def create_backtest_signal(self,days_strategy, test_size, feature_name, high_exit = False, low_exit = False):
+        """
+        perform backtest signal analysis
+
+        Parameters
+        ----------
+        days_strategy (list): list of days to assess returns
+        test_size (str): test data size
+        feature_name (str): name of the feature to assess
+        high_exit (float): high exit thrshold return in backtest
+        low_exit (float): loss exit thrshold return in backtest
+
+        Returns
+        -------
+        fig (obj): plots
+        messages (dict): dictionary with key metrics
+        """
         asset_1 = 'Close'
         up_signal, low_signal= f'signal_up_{feature_name}', f'signal_low_{feature_name}'
         df1 = self.data.iloc[-test_size:,:].copy()
         df2 = df1.copy()
         df2['signal_type'] = np.where(
-                    df2[up_signal] == 1, 
-                    'up', 
+                    df2[up_signal] == 1,
+                    'up',
                     np.where(
-                        df2[low_signal] == 1, 
+                        df2[low_signal] == 1,
                         'down',
                         None
                     )
                 )
         df2 = df2[~df2.signal_type.isna()]
         # df2['Date_'] = df2.index
         df2['lag_Date'] = df2['Date'].shift(1)
         df2['span'] = (pd.to_datetime(df2['Date']) - pd.to_datetime(df2['lag_Date'])).dt.days - 1
         df2['break'] = np.where(df2['span'] > 3, 1, 0)
         df2['break'] = np.where(df2['span'].isna(), 1, df2['break'])
-    
+
         df2['chain_id'] = df2.sort_values(['Date']).groupby(['break']).cumcount() + 1
         df2['chain_id'] = np.where(df2['break'] == 1, df2['chain_id'], np.nan )
         df2['chain_id'] = df2['chain_id'].fillna(method = 'ffill')
-    
+
         df2['internal_rn'] = df2.sort_values(['Date']).groupby(['chain_id']).cumcount() + 1
         df2['inv_internal_rn'] = df2.sort_values(['Date'],ascending = False).groupby(['chain_id']).cumcount() + 1
-    
+
         df2['first_in_chain'] = np.where(df2['internal_rn'] == 1, True, False)
         df2['last_in_chain'] = np.where(df2['inv_internal_rn'] == 1, True, False)
-    
+
         df2 = df2.drop(columns = ['break','span','lag_Date','inv_internal_rn']).sort_values('Date')
-    
+
         df2 = df2[(df2.last_in_chain == True) & (df2.signal_type == 'down')][['last_in_chain']]
         dft = df1.merge(df2,how = 'left',left_index=True, right_index=True )
-    
+
         dft['chain_id'] = dft.sort_values(['Date']).groupby(['last_in_chain']).cumcount() + 1
         dft['chain_id'] = np.where(dft['last_in_chain'] == True, dft['chain_id'], np.nan )
         dft['chain_id'] = dft['chain_id'].fillna(method = 'ffill')
-    
+
         dft['internal_rn'] = dft.sort_values(['Date']).groupby(['chain_id']).cumcount() + 1
         dft['flag'] = np.where(dft['internal_rn'] < days_strategy, 1,0)
-        
+
         dft['lrets_bench'] = np.log(dft[asset_1]/dft[asset_1].shift(1))
         dft['bench_prod'] = dft['lrets_bench'].cumsum()
         dft['bench_prod_exp'] = np.exp(dft['bench_prod']) - 1
-        
+
         if high_exit and low_exit:
             dft['open_strat'] = np.where(dft.last_in_chain == True, dft.Open, np.nan)
             dft['open_strat'] = dft['open_strat'].fillna(method = 'ffill')
             dft['open_strat'] = np.where(dft.flag == 1, dft.open_strat, np.nan)
             dft['high_strat_ret'] = (dft['High']/dft['open_strat']-1)*100
             dft['low_strat_ret'] = (dft['Low']/dft['open_strat']-1)*100
             dft['high_exit'] =  np.where(((dft['high_strat_ret'] >= high_exit) | (dft['internal_rn'] == days_strategy)), 1, np.nan)
             dft['low_exit'] =  np.where((dft['low_strat_ret'] <= low_exit), -1, np.nan)
-            
+
             dft["exit_type"] = dft[["high_exit", "low_exit"]].max(axis=1)
             dft['exit_type'] = np.where(dft["exit_type"] == 1, 1, np.where(dft["exit_type"] == -1,-1,np.nan))
             dft['exit'] = np.where(dft['exit_type'].isnull(), np.nan, 1)
             dft['exit_order'] = dft.sort_values(['Date']).groupby(['chain_id','exit']).cumcount() + 1
             dft['exit'] = np.where(dft['exit_order'] == 1, True, np.nan)
             dft = dft.drop(columns = ['exit_order'])
             ## if last signal is near
             max_id = dft.chain_id.max()
             dft['max_internal_rn'] = dft.sort_values(['Date']).groupby(['chain_id']).internal_rn.transform('max')
             dft['exit'] = np.where((dft.chain_id == max_id) & (dft.max_internal_rn < days_strategy) & (dft.max_internal_rn == dft.internal_rn), 1, dft['exit'])
-            
+
             dft['exit_step'] = np.where(dft.exit == 1, dft.internal_rn, np.nan)
             dft['exit_step'] = dft.sort_values(['Date']).groupby(['chain_id']).exit_step.transform('max')
-            
+
             dft['flag'] = np.where(dft.internal_rn <= dft.exit_step, 1, 0)
             dft = dft.drop(columns = ['open_strat', 'high_strat_ret', 'low_strat_ret','exit_step', 'exit','exit_type','high_exit','low_exit', 'max_internal_rn'])
-        
+
         dft['lrets_strat'] = np.log(dft[asset_1].shift(-1)/dft[asset_1]) * dft['flag']
         dft['lrets_strat'] = np.where(dft['lrets_strat'].isna(),-0.0,dft['lrets_strat'])
         dft['lrets_prod'] = dft['lrets_strat'].cumsum()
         dft['strat_prod_exp'] = np.exp(dft['lrets_prod']) - 1
-    
+
         bench_rets = round(dft['bench_prod_exp'].values[-1]*100,1)
         strat_rets = round(dft['strat_prod_exp'].values[-1]*100,1)
-        
+
         bench_sr = round(sharpe_ratio(dft.bench_prod_exp.dropna()),1)
         strat_sr = round(sharpe_ratio(dft.strat_prod_exp.dropna()),1)
-        
+
         message1 = f'{bench_rets}%'
         message2 = f'{strat_rets}%'
-        
+
         messages = {
             'benchmark return:':message1,
             'benchmark sharpe ratio:': bench_sr,
             'strategy return:':message2,
             'strategy sharpe ratio:': strat_sr,
         }
         if self.show_plot:
             print('----------------------------')
             print(messages)
             print('----------------------------')
-            
+
         fig = plt.figure(1)
         plt.plot(dft.bench_prod_exp.values, label = 'benchmark')
         plt.scatter(range(len(dft)),np.where(dft[low_signal] == 1,dft.bench_prod_exp.values,np.nan),color = 'red', label = 'signal')
         plt.plot(dft.strat_prod_exp.values, label = 'strategy')
         plt.legend()
         plt.title('strategy and cumulative returns based on signal strategy')
         if self.show_plot:
             plt.plot()
-            
+
         if self.save_path:
             result_json_name = f'signals_strategy_return_{feature_name}.json'
             result_plot_name = f'signals_strategy_return_{feature_name}.png'
-            
+
             plt.savefig(self.save_path+result_plot_name)
             # pickle.dump(fig, open(self.save_path+result_plot_name, 'wb'))
-            
-            with open(self.save_path+result_json_name, "w") as outfile: 
+
+            with open(self.save_path+result_json_name, "w") as outfile:
                 json.dump(messages, outfile)
-                
+
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_json_name ,input_path = self.save_path+result_json_name)
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.ticket_name}/'+result_plot_name,input_path = self.save_path+result_plot_name)
-            
+
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_json_name, input_path = self.save_path + result_json_name, aws_credentials = self.aws_credentials)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_plot_name, input_path = self.save_path + result_plot_name, aws_credentials = self.aws_credentials)
-    
+
         if not self.show_plot:
             plt.close()
-            
+
         del df1,df2,dft
-    
+
         if self.return_fig:
             return fig, messages
-        
+
 def execute_signal_analyser(test_data_size, feature_name, days_list, configuration, method, object_stock, signal_analyser_object, plot = False, backtest= False, exit_params = {}):
-     
+    '''
+    code snippet that is going run some objects. The analysis is signal analyse which is backtesting
+
+            Parameters:
+                    test_data_size (int): test data size
+                    feature_name (str): name of the feature to assess
+                    days_list (list): tome scope to assess the returns
+                    configuration (dict): parameters of the method to run
+                    object_stock (obj): object with data to assess
+                    signal_analyser_object (obj): signal_analyser object
+                    plot (boolean): if true, plot results
+                    backtest (boolean): if true, run backtest 
+                    exit_params (dict): parameters of exit returns
+
+            Returns:
+                    mean_median_return (float): median return of the backtests
+    '''
     method(**configuration)
     signal_assess = signal_analyser_object(object_stock.df,object_stock.stock_code,show_plot = plot)
     signal_assess.signal_analyser(test_size = test_data_size, feature_name = feature_name, days_list = days_list, threshold = 1)
 
     if backtest:
         print('-----------------------back test ---------------------------')
         signal_assess.create_backtest_signal(backtest, test_data_size, feature_name, **exit_params )
-    
+
     return signal_assess.mean_median_return
 
 def iterate_signal_analyser(test_data_size,feature_name, days_list, arguments_to_test, method, object_stock, signal_analyser_object, plot = True):
+    '''
+    code snippet is going to iterate signal analyser
 
+            Parameters:
+                    test_data_size (int): test data size
+                    feature_name (str): name of the feature to assess
+                    days_list (list): tome scope to assess the returns
+                    arguments_to_test: parameters to test
+                    method: methods to run
+                    object_stock (obj): object with data to assess
+                    signal_analyser_object (obj): signal_analyser object
+                    plot (boolean): if true, plot results
+
+            Returns:
+                    best_result (int): index from the arguments_to_test with the best result
+    '''
     results = list()
     for key in arguments_to_test.keys():
         configuration = arguments_to_test.get(key)
         mean_median_return = execute_signal_analyser(test_data_size, feature_name, days_list, configuration, method, object_stock, signal_analyser_object)
         results.append(mean_median_return)
-    
+
     df_result = pd.DataFrame({'keys':arguments_to_test.keys(),'results':results})
     if plot:
         plt.plot(df_result['keys'], df_result['results'])
         plt.scatter(df_result['keys'], df_result['results'])
         plt.title('simulation between configurations')
-        plt.ylabel('median expected return') 
+        plt.ylabel('median expected return')
         plt.show()
-        
+
     best_result = df_result.sort_values('results',ascending = False)['keys'].values[0]
     return best_result
-    
+
 class analyse_index(stock_eda_panel):
-    def __init__(self, index, asset, n_obs, lag, data_window = '5y', show_plot = True, save_path = False, save_aws = False, aws_credentials = False):
+    """
+    class that is going to train hmm models to perform feature selection
+
+    Attributes
+    ----------
+    data  : pd.DataFrame
+        symbol of the asset
+    index : str
+         name of the index
+    asset : str
+         name of the asset
+    n_obs : int
+         number of rows to extract
+    lag : int
+         lag to apply
+    data_window : str
+         5y 10y 15y
+    show_plot : bool
+         If True, show plots
+    save_path : str
+         local path for saving e.g r'C:/path/to/the/file/'
+    save_aws : str
+         remote key in s3 bucket path e.g. 'path/to/file/'
+    aws_credentials : dict
+         dict with the aws credentials
+    merger_df : pd.DataFrame
+        dataframe with the index and asset data
+    states_result = dict
+        betas and correlation score results
+
+    Methods
+    -------
+    process_data():
+        using stock_eda_panel, get data and merge data
+    plot_betas(sample_size=int, offset=int, subsample_ts=int):
+        display beta analysis plot
+    get_betas(subsample_ts=int)
+        get general beta and last sample beta, correlation score is included too
+    """
 
+    def __init__(self, index, asset, n_obs, lag, data_window = '5y', show_plot = True, save_path = False, save_aws = False, aws_credentials = False):
         """
-        data: pandas df
-        index: str name of the index
-        asset: str name of the asset
-        n_obs: int
-        lag: int
-        data_window: str eg 5y 10y 15y
-        show_plot: bool
-        save_path: str local path for saving e.g r'C:/path/to/the/file/'
-        save_aws: str remote key in s3 bucket path e.g. 'path/to/file/'
-        aws_credentials: dict
+        Initialize object
+
+        Parameters
+        ----------
+        index (str): name of the index
+        asset (str): name of the asset
+        n_obs (int): number of rows to extract
+        lag (int): lag to apply
+        data_window (str): 5y 10y 15y
+        show_plot (bool): If True, show plots
+        save_path (str): local path for saving e.g r'C:/path/to/the/file/'
+        save_aws (str): remote key in s3 bucket path e.g. 'path/to/file/'
+        aws_credentials (dict): dict with the aws credentials
+
+        Returns
+        -------
+        None
         """
-         
+
         self.index = index
         self.asset = asset
         self.n_obs = n_obs
         self.data_window = data_window
         self.lag = lag
-        
+
         self.show_plot = show_plot
         self.save_path = save_path
         self.save_aws = save_aws
-        
+
     def process_data(self):
-        
+        """
+        using stock_eda_panel, get data and merge data
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         index = stock_eda_panel(self.index, self.n_obs, self.data_window)
         index.get_data()
         index.df['shift'] = index.df.Close.shift(self.lag)
         index.df['index_return'] = index.df.Close/index.df['shift'] - 1
 
         asset =  stock_eda_panel(self.asset, self.n_obs, self.data_window)
         asset.get_data()
         asset.df['shift'] = asset.df.Close.shift(self.lag)
         asset.df['asset_return'] = asset.df.Close/asset.df['shift'] - 1
-        
+
         df1 = index.df[['Date','index_return']]
         df2 = asset.df[['Date','asset_return','Close']]
         merger = df1.merge(df2, on = 'Date', how = 'inner')
         merger.dropna(inplace = True)
         self.merger_df = merger
-        
+
     def plot_betas(self,sample_size, offset, subsample_ts =False):
-    
+        """
+        display beta analysis plot
+
+        Parameters
+        ----------
+        sample_size (int): number of days or window size to calculate beta
+        offset (int): overlap between windows
+        subsample_ts (int): subsample size of data 
+
+        Returns
+        -------
+        None
+        """
         ### extracting data
 
         self.process_data()
-        
+
          ### ploting analysis
         figure, ax = plt.subplot_mosaic(
             [["scatter_total", "scatter_sample",'ts','ts']],
             layout="constrained",
             figsize=(18, 5)
         )
-        
+
         ax['scatter_total'].scatter(self.merger_df.asset_return, self.merger_df.index_return)
         b, a = np.polyfit(self.merger_df.asset_return, self.merger_df.index_return, 1)
         ax['scatter_total'].plot(self.merger_df.asset_return, b*self.merger_df.asset_return+a, color='red')
 
         ax['ts'].plot(self.merger_df.Date, self.merger_df.Close, color = 'grey', alpha = 0.3)
-        
+
         if subsample_ts:
             self.merger_df = self.merger_df.iloc[-subsample_ts:,:].dropna()
-        
+
         for i in range(0,len(self.merger_df)-sample_size,offset):
 
             merger_ = self.merger_df.sort_values('Date', ascending = False).iloc[i:i+sample_size,:]
-            x = merger_.index_return 
+            x = merger_.index_return
             y = merger_.asset_return
             b, a = np.polyfit(x,y, 1)
 
             normalize = mcolors.Normalize(vmin=-1, vmax=1)
             colormap = cm.jet
 
             ax['scatter_sample'].plot(x, y,'o', color = 'blue', alpha = 0.1)
@@ -2094,94 +3189,161 @@
             ax['scatter_sample'].set_xlim(-0.06, 0.06)
             ax['scatter_sample'].set_ylim(-0.06, 0.06)
 
             plot = ax['ts'].scatter(merger_.Date, merger_.Close, color=colormap(normalize(b)), s = 10)
 
         scalarmappaple = cm.ScalarMappable(norm=normalize, cmap=colormap)
         scalarmappaple.set_array(x)
-        
+
         plt.title(f'{self.asset} using index: {self.index}')
         plt.colorbar(scalarmappaple)
-        
+
         if self.show_plot:
             plt.show()
         if self.save_path:
             result_plot_name = f'market_best_fit.png'
             figure.savefig(self.save_path+result_plot_name)
 
         if self.save_path and self.save_aws:
             # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'market_plots/{self.asset}/'+result_plot_name,input_path = self.save_path+result_plot_name)
             upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = self.save_aws + result_plot_name, input_path = self.save_path + result_plot_name, aws_credentials = self.aws_credentials)
         if not self.show_plot:
             plt.close()
-        
+
     def get_betas(self,subsample_ts=False):
-        
+        """
+        get general beta and last sample beta, correlation score is included too
+
+        Parameters
+        ----------
+        subsample_ts (int): subsample size of data 
+
+        Returns
+        -------
+        None
+        """
         self.process_data()
         general_beta, a = np.polyfit(self.merger_df.asset_return, self.merger_df.index_return, 1)
         general_r = stats.mstats.pearsonr(self.merger_df.asset_return, self.merger_df.index_return)[0]
-        
+
         self.process_data()
         if subsample_ts:
             self.merger_df = self.merger_df.iloc[-subsample_ts:,:].dropna()
         sample_beta, a = np.polyfit(self.merger_df.asset_return, self.merger_df.index_return, 1)
         sample_r = stats.mstats.pearsonr(self.merger_df.asset_return, self.merger_df.index_return)[0]
-        
+
         result = {
             'general_beta':general_beta,
             'general_r':general_r,
             'sample_beta':sample_beta,
             'sample_r':sample_r
         }
-        
+
         self.states_result = result
-        
+
 class evaluate_markets(analyse_index):
+    """
+    object that is going to evaluate multiple indexes
+
+    Attributes
+    ----------
+    stock_code : str
+        asset to assess
+    indexes : list
+        list of indexes
+    best_result : dict
+        best result beta and correlation
+
+    Methods
+    -------
+    process_data():
+        using stock_eda_panel, get data and merge data
+    plot_betas(sample_size=int, offset=int, subsample_ts=int):
+        display beta analysis plot
+    get_betas(subsample_ts=int)
+        get general beta and last sample beta, correlation score is included too
+    evaluate_best_market_fit(sample_size=int, offset=int,lag=int, n_obs=int, verbose=boolean, plot_best=boolean):
+        iterate every index in the index list and get results
+    """
+
     def __init__(self, stock_code, indexes):
+        """
+        Initialize object
+
+        Parameters
+        ----------
+        stock_code  (str): asset to assess
+        indexes (list): list of indexes
+
+        Returns
+        -------
+        None
+        """
         self.stock_code = stock_code
         self.indexes = indexes
     def evaluate_best_market_fit(self,sample_size, offset,lag= 3, n_obs = 3500, verbose = False, plot_best = False):
+        """
+        iterate every index in the index list and get results
 
+        Parameters
+        ----------
+        sample_size (int): sample size to get betas
+        offset (int): overlap size
+        lag (int): number of lags of the returns
+        n_obs (int): number of observations of the data extraction
+        verbose (boolean): if true, print results
+        plot_best (boolean): if true, display plot of the best result
+
+        Returns
+        -------
+        None
+        """
         results_dicts = dict()
         for index in self.indexes:
             betex = analyse_index(index = index,asset = self.stock_code,n_obs = n_obs, lag = lag)
             betex.get_betas(sample_size)
             results_dicts[index] = betex.states_result
         pd_result = pd.DataFrame(results_dicts).T
         pd_result['gen_r2'] = pd_result.general_r ** 2
         pd_result['sampl_r2'] = pd_result.sample_r ** 2
         self.stat_results = pd_result
-        
+
         best_result = pd_result.sort_values('gen_r2',ascending = False).head(2).sort_values('sampl_r2',ascending = False).head(1)
         best_fit_index = best_result.index.values[0]
-        
+
         self.stat_results = self.stat_results.drop(columns = ['gen_r2','sampl_r2'])
-        
+
         if verbose:
             print(best_result)
         if plot_best:
             betex = analyse_index(index = best_fit_index,asset = self.stock_code, n_obs = n_obs, lag = lag)
             betex.plot_betas(sample_size = sample_size, offset = offset, subsample_ts = False)
-            
+
         self.best_result = best_result
-        
+
 def get_relevant_beta(data_market, ticket_name,  show_plot = True, save_path = False, save_aws = False, aws_credentials = False):
-    """
-        data_market: pandas df
-        ticket_name: str name of the asset
-        show_plot: bool
-        save_path: str local path for saving e.g r'C:/path/to/the/file/'
-        save_aws: str remote key in s3 bucket path e.g. 'path/to/file/'
-        aws_credentials: dict
-        """
+    '''
+    select relevant beta result data of a given asset
+
+            Parameters:
+                    data_market (pd.DataFrame): dataframe of the market results 
+                    ticket_name (str): name of the asset
+                    show_plot (bool): If tru, plot results
+                    save_path (str): local path for saving e.g r'C:/path/to/the/file/'
+                    save_aws (str):  remote key in s3 bucket path e.g. 'path/to/file/'
+                    aws_credentials (dict): dict of the aws credentials
+
+            Returns:
+                    selection (pd.DataFrame): dataframe of the most relevant beta
+    '''
     all_betas = data_market[data_market.asset == ticket_name].sort_values('general_r', ascending = False)
     all_betas['gen_r2'] = all_betas.general_r ** 2
     all_betas['sampl_r2'] = all_betas.sample_r ** 2
     selection = all_betas.sort_values('gen_r2',ascending =False).head(2).sort_values('sampl_r2',ascending =False).head(1).drop(columns = ['gen_r2','sampl_r2'])
-    
+
     if show_plot:
         print(selection)
     if save_path:
         result_plot_name = f'market_best_fit.csv'
         selection.to_csv(save_path+result_plot_name)
 
     if save_path and save_aws:
```

### Comparing `virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.75
+Version: 0.0.76
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.75/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.76/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*


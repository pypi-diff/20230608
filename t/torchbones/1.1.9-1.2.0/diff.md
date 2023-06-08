# Comparing `tmp/torchbones-1.1.9.tar.gz` & `tmp/torchbones-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.9.tar", last modified: Mon Jun  5 23:56:53 2023, max compression
+gzip compressed data, was "torchbones-1.2.0.tar", last modified: Tue Jun  6 08:49:04 2023, max compression
```

## Comparing `torchbones-1.1.9.tar` & `torchbones-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:56:53.547087 torchbones-1.1.9/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:56:53.547087 torchbones-1.1.9/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-05 23:56:53.547087 torchbones-1.1.9/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-05 23:56:17.000000 torchbones-1.1.9/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:56:53.547087 torchbones-1.1.9/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.9/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    17104 2023-06-05 23:56:12.000000 torchbones-1.1.9/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-05 23:56:53.547087 torchbones-1.1.9/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-05 23:56:53.000000 torchbones-1.1.9/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-06 08:49:04.689027 torchbones-1.2.0/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-06 08:49:04.689027 torchbones-1.2.0/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-06 08:49:04.689027 torchbones-1.2.0/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-06 08:48:30.000000 torchbones-1.2.0/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-06 08:49:04.689027 torchbones-1.2.0/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.0/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16880 2023-06-06 08:48:20.000000 torchbones-1.2.0/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-06 08:49:04.689027 torchbones-1.2.0/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-06 08:49:04.000000 torchbones-1.2.0/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.9/torchbones/main.py` & `torchbones-1.2.0/torchbones/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         self.init_lr = self.lr
         self.lr_decay = kwargs.get('lr_decay', 1)
         self.lr_min = kwargs.get('lr_min', 1e-10)
         self.optimizer = self.optim(self.net.parameters(), lr = self.lr)
     
             
         self.trainerr, self.testerr, self.err, self.epoch, self.loc, self.save_file = [], [], 0, 0, 0, None #just inits
-        self.plotev, self.printev = 10, 10
+        self.plotev = 10
         
         self.saving = kwargs.get('saving', False)
         self.save_tar = kwargs.get('save_weights', False)
         
         if self.save_tar and not os.path.isdir(weight_path):
             os.makedirs(weight_path)
         
@@ -251,15 +251,14 @@
                 
         train, traintruth, traincov, test, testtruth, testcov = self.data
         self.epochs = kwargs.get('epochs', 20)
         self.lr = kwargs.get('lr', self.lr)
         self.lr_decay = kwargs.get('lr_decay', self.lr_decay)
         self.lr_min = kwargs.get('lr_min', self.lr_min)
         training = kwargs.get('training', True)
-        self.printev = kwargs.get('print_ev', self.plotev)
         self.plotev = kwargs.get('plot_ev', self.plotev)
         e0 = self.epoch
         batches = round(len(traintruth)/self.batch_size)
         
         while self.epoch - e0 < self.epochs:
             l = 0
             shuffle = torch.randperm(len(traintruth)) #shuffle training set
@@ -286,22 +285,20 @@
             else:
                 self.err = self.cost(torch.squeeze(self.testout), torch.tensor(testtruth), testcov).mean().detach().numpy()
             self.testerr.append(self.err)
 
             if self.plotev:
                 if not (self.epoch-e0) % self.plotev:
                     self.plot()
+                    print(f"Epoch number {self.epoch}:")
+                    print(f" Test Loss: {np.round(self.testerr[-1], 3)}; Train Loss {np.round(self.trainerr[-1], 3)}")
+
                     if not training:
                         return []
 
-            if self.printev:
-                if not (self.epoch-e0) % self.printev and not np.isnan(self.trainerr[-1]):
-                    self.plot()
-                    print(f"Epoch number {self.epoch} Last 100 average test loss {np.mean(self.testerr[-100:])} train loss {np.mean(self.trainerr[-100:])}")
-              
             t = 10
             if not self.epoch%t or self.trainerr[-1]!=self.trainerr[-1]:   
                 self.checkpoint(t)
                 
             if self.saving:
                 self.save()
             self.epoch += 1
```


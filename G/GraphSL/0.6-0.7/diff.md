# Comparing `tmp/GraphSL-0.6.tar.gz` & `tmp/GraphSL-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSL-0.6.tar", last modified: Thu Apr  4 14:31:44 2024, max compression
+gzip compressed data, was "GraphSL-0.7.tar", last modified: Thu Apr  4 22:08:12 2024, max compression
```

## Comparing `GraphSL-0.6.tar` & `GraphSL-0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-04 14:31:44.627175 GraphSL-0.6/
-drwxr-xr-x   0 junwang   (8726) dsss      (5100)        0 2024-04-04 14:31:44.627175 GraphSL-0.6/GraphSL.egg-info/
--rw-r--r--   0 junwang   (8726) dsss      (5100)      828 2024-04-04 14:31:44.000000 GraphSL-0.6/GraphSL.egg-info/PKG-INFO
--rw-r--r--   0 junwang   (8726) dsss      (5100)      190 2024-04-04 14:31:44.000000 GraphSL-0.6/GraphSL.egg-info/SOURCES.txt
--rw-r--r--   0 junwang   (8726) dsss      (5100)        1 2024-04-04 14:31:44.000000 GraphSL-0.6/GraphSL.egg-info/dependency_links.txt
--rw-r--r--   0 junwang   (8726) dsss      (5100)       62 2024-04-04 14:31:44.000000 GraphSL-0.6/GraphSL.egg-info/requires.txt
--rw-r--r--   0 junwang   (8726) dsss      (5100)        1 2024-04-04 14:31:44.000000 GraphSL-0.6/GraphSL.egg-info/top_level.txt
--rw-r--r--   0 junwang   (8726) dsss      (5100)     1070 2024-04-01 15:50:38.000000 GraphSL-0.6/LICENSE
--rw-r--r--   0 junwang   (8726) dsss      (5100)      828 2024-04-04 14:31:44.627175 GraphSL-0.6/PKG-INFO
--rw-r--r--   0 junwang   (8726) dsss      (5100)     8951 2024-04-04 14:16:01.000000 GraphSL-0.6/README.md
--rw-r--r--   0 junwang   (8726) dsss      (5100)       79 2024-04-04 14:31:44.627175 GraphSL-0.6/setup.cfg
--rw-r--r--   0 junwang   (8726) dsss      (5100)     1726 2024-04-04 14:28:52.000000 GraphSL-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 22:08:12.184435 GraphSL-0.7/
+drwxrwxrwx   0        0        0        0 2024-04-04 22:08:12.180382 GraphSL-0.7/GraphSL.egg-info/
+-rw-rw-rw-   0        0        0      732 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.7/LICENSE
+-rw-rw-rw-   0        0        0      732 2024-04-04 22:08:12.184435 GraphSL-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.7/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-04 22:08:12.186496 GraphSL-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1729 2024-04-04 22:08:07.000000 GraphSL-0.7/setup.py
```

### Comparing `GraphSL-0.6/LICENSE` & `GraphSL-0.7/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Junxiang Wang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Junxiang Wang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `GraphSL-0.6/README.md` & `GraphSL-0.7/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-[![Documentation Status](https://readthedocs.org/projects/graphsl/badge/?version=latest)](https://graphsl.readthedocs.io/en/latest/?badge=latest)
-[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
-
-# GraphSL: Graph Source Localization Library
-
-This is the source code of the GraphSL (Graph Source Localization) library to support the research and development of the graph learning community.
-
-# Introduction
-
-## Problem Definition
-
-![image](SL_example.png)
-
-Graph diffusion is a fundamental task in graph learning, which aims to predict future graph cascade patterns given source nodes. Conversely, its inverse problem, graph source localization, though rarely explored, stands as an extremely important topic: it focuses on the detection of source nodes given their future graph cascade patterns. As illustrated in the above figure, graph diffusion seeks to predict the cascade pattern $\lbrace b,c,d,e \rbrace$ from a source node $b$, whereas graph source localization aims to identify source nodes $b$ from the cascade pattern $\lbrace b,c,d,e \rbrace$. 
-
-Graph source localization spans a broad spectrum of promising research and real-world applications. For instance, online social media platforms like Twitter and Facebook have been instrumental in disseminating rumors and misinformation with significant repercussions. Additionally, the rapid propagation of computer viruses across the Internet, infecting millions of computers, underscores the critical need for tracking their sources. Moreover, in smart grids, where isolated failures can trigger rolling blackouts leading to substantial financial losses, graph source localization plays a pivotal role. Hence, the graph source localization problem demands attention and extensive investigations from machine learning researchers.
-
-The GraphSL library includes six state-of-the-art approaches and eight benchmark datasets.
-
-
-## Approaches
-
-![image](overview.png)
-
- Existing graph source localization methods can be categorized into two groups: Prescribed methods and Graph Neural Networks (GNN)-based methods.
-
-Prescribed methods rely on hand-crafted rules and heuristics. For instance, LPSI propagates infection in networks and labels local peaks as source nodes. NetSleuth employed the Minimum Description Length principle to identify the optimal set of source nodes and virus propagation ripple. OJC identified a set of nodes (Jordan cover) that cover all observed infected nodes with the minimum radius.
-
-GNN-based methods learn rules from graph data in an end-to-end manner by capturing graph topology and neighboring information. For example, GCNSI utilized LPSI to enhance input and then applied Graph Convolutional Networks (GCN) for source identification; IVGD introduced a graph residual scenario to make existing graph diffusion models invertible, and it devises a new set of validity-aware layers to project inferred sources to feasible regions. SLVAE used forward diffusion estimation and deep generative models to approximate source distribution, leveraging prior knowledge for generalization under arbitrary diffusion patterns.
-
-## Benchmark Datasets
-
-|       Dataset      |  #Node |  #Edge | Average Degree | Seed-Diffusion Pairs |
-|:------------------:|:------:|:------:|:--------------:|:--------------------------:|
-|       Karate       |   34   |   78   |      4.588     |             No             |
-|      Dolphins      |   62   |   159  |      5.129     |             No             |
-|         Jazz       |   198  |  2,742 |     27.697     |             No             |
-| Network   Science  |  1,589 |  2,742 |      3.451     |             No             |
-|       Cora-ML      |  2,810 |  7,981 |      5.68      |             No             |
-|    Power   Grid    |  4,941 |  6,594 |      2.669     |             No             |
-|     Memetracker    |  7,884 | 47,911 |     12.154     |            Yes             |
-|        Digg        | 15,912 | 78,649 |      9.885     |            Yes             |
-
-
-Aside from methods, we also provide eight benchmark datasets to facilitate the research of the graph source localization problem. Memetracker and Digg provide Seed-Diffusion vector pairs. While others do not have such pairs, they can be generated by information diffusion simulations. All datasets are introduced as follows:
-
-1. Karate: Karate depicts the social ties among members of a university karate club.
-
-2. Dolphins: Dolphins represents a social network of bottlenose dolphins, with edges indicating frequent associations between dolphins.
-
-3. Jazz: Jazz illustrates a collaboration network among Jazz musicians, where edges signify instances of playing together in a band.
-
-4. Network Science: Network Science portrays a coauthorship network of scientists engaged in network theory and experimentation, with each edge representing co-authorship of a paper.
-
-5. Cora-ML: Cora-ML is a portal network of computer science research papers obtained through machine learning techniques.
-
-6. Power Grid: Power Grid delineates the topology network of the Western States Power Grid in the United States.
-
-7. Memetracker: Memetracker tracks frequently used phrases on news social media, and a small subset of the whole Memetracker network was retrieved here.
-
-8. Digg: Digg showcases a reply network within social news, and a small subset of the whole Digg network was retrieved here.
-
-# Installation
-
-#### Installation via PyPI
-```bash
-pip install GraphSL
-```
-
-#### Installation via GitHub
-Clone the repo from [here](https://github.com/xianggebenben/GraphSL) (this repo).
-
-Install requirements:
-```bash
-pip install -r requirements.txt
-```
-
-# Quickstart
-``` python
-
-   from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
-   from GraphSL.Prescribed import LPSI, NetSleuth, OJC
-   from GraphSL.GNN.GCNSI.main import GCNSI
-   from GraphSL.GNN.IVGD.main import IVGD
-   from GraphSL.GNN.SLVAE.main import SLVAE
-   data_name = 'karate'  # 'karate', 'dolphins', 'jazz', 'netscience', 'cora_ml', 'power_grid', , 'meme8000', 'digg16000'
-   graph = load_dataset(data_name)
-   if data_name not in ['meme8000', 'digg16000']:
-       dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.3)
-   else:
-       dataset = graph
-   adj, train_dataset, test_dataset =split_dataset(dataset)
-   lpsi = LPSI()
-   alpha, thres, auc, f1, pred =lpsi.train(adj, train_dataset)
-   print("LPSI:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric=lpsi.test(adj, test_dataset, alpha, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   netSleuth = NetSleuth()
-   k, auc, f1=netSleuth.train(adj, train_dataset)
-   print("NetSleuth:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = netSleuth.test(adj, test_dataset, k)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   ojc = OJC()
-   Y, auc, f1 =ojc.train(adj, train_dataset)
-   print("OJC:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric=ojc.test(adj, test_dataset, Y)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   gcnsi = GCNSI()
-   gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
-   print("GCNSI:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = gcnsi.test(adj, test_dataset, gcnsi_model, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   ivgd = IVGD()
-   diffusion_model = ivgd.train_diffusion(adj, train_dataset)
-   ivgd_model, thres, auc, f1, pred =ivgd.train(adj, train_dataset, diffusion_model)
-   print("IVGD:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = ivgd.test(test_dataset, diffusion_model, ivgd_model, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-   slave = SLVAE()
-   slvae_model, seed_vae_train, thres, auc, f1, pred = slave.train(adj, train_dataset)
-   print("SLVAE:")
-   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
-   metric = slave.infer(test_dataset, slvae_model, seed_vae_train, thres)
-   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
-```
-
-# Documentation
-
-Official documentation, including a detailed [API reference](https://graphsl.readthedocs.io/en/latest/modules.html), is available on [Read the Docs](https://graphsl.readthedocs.io/en/latest/#).
-
-# Contact
-
-Feel free to Email Junxiang Wang (junxiang.wang@alumni.emory.edu) if you have any questions.
+[![Documentation Status](https://readthedocs.org/projects/graphsl/badge/?version=latest)](https://graphsl.readthedocs.io/en/latest/?badge=latest)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+
+# GraphSL: Graph Source Localization Library
+
+This is the source code of the GraphSL (Graph Source Localization) library to support the research and development of the graph learning community.
+
+# Introduction
+
+## Problem Definition
+
+![image](SL_example.png)
+
+Graph diffusion is a fundamental task in graph learning, which aims to predict future graph cascade patterns given source nodes. Conversely, its inverse problem, graph source localization, though rarely explored, stands as an extremely important topic: it focuses on the detection of source nodes given their future graph cascade patterns. As illustrated in the above figure, graph diffusion seeks to predict the cascade pattern $\lbrace b,c,d,e \rbrace$ from a source node $b$, whereas graph source localization aims to identify source nodes $b$ from the cascade pattern $\lbrace b,c,d,e \rbrace$. 
+
+Graph source localization spans a broad spectrum of promising research and real-world applications. For instance, online social media platforms like Twitter and Facebook have been instrumental in disseminating rumors and misinformation with significant repercussions. Additionally, the rapid propagation of computer viruses across the Internet, infecting millions of computers, underscores the critical need for tracking their sources. Moreover, in smart grids, where isolated failures can trigger rolling blackouts leading to substantial financial losses, graph source localization plays a pivotal role. Hence, the graph source localization problem demands attention and extensive investigations from machine learning researchers.
+
+The GraphSL library includes six state-of-the-art approaches and eight benchmark datasets.
+
+
+## Approaches
+
+![image](overview.png)
+
+ Existing graph source localization methods can be categorized into two groups: Prescribed methods and Graph Neural Networks (GNN)-based methods.
+
+Prescribed methods rely on hand-crafted rules and heuristics. For instance, LPSI propagates infection in networks and labels local peaks as source nodes. NetSleuth employed the Minimum Description Length principle to identify the optimal set of source nodes and virus propagation ripple. OJC identified a set of nodes (Jordan cover) that cover all observed infected nodes with the minimum radius.
+
+GNN-based methods learn rules from graph data in an end-to-end manner by capturing graph topology and neighboring information. For example, GCNSI utilized LPSI to enhance input and then applied Graph Convolutional Networks (GCN) for source identification; IVGD introduced a graph residual scenario to make existing graph diffusion models invertible, and it devises a new set of validity-aware layers to project inferred sources to feasible regions. SLVAE used forward diffusion estimation and deep generative models to approximate source distribution, leveraging prior knowledge for generalization under arbitrary diffusion patterns.
+
+## Benchmark Datasets
+
+|       Dataset      |  #Node |  #Edge | Average Degree | Seed-Diffusion Pairs |
+|:------------------:|:------:|:------:|:--------------:|:--------------------------:|
+|       Karate       |   34   |   78   |      4.588     |             No             |
+|      Dolphins      |   62   |   159  |      5.129     |             No             |
+|         Jazz       |   198  |  2,742 |     27.697     |             No             |
+| Network   Science  |  1,589 |  2,742 |      3.451     |             No             |
+|       Cora-ML      |  2,810 |  7,981 |      5.68      |             No             |
+|    Power   Grid    |  4,941 |  6,594 |      2.669     |             No             |
+|     Memetracker    |  7,884 | 47,911 |     12.154     |            Yes             |
+|        Digg        | 15,912 | 78,649 |      9.885     |            Yes             |
+
+
+Aside from methods, we also provide eight benchmark datasets to facilitate the research of the graph source localization problem. Memetracker and Digg provide Seed-Diffusion vector pairs. While others do not have such pairs, they can be generated by information diffusion simulations. All datasets are introduced as follows:
+
+1. Karate: Karate depicts the social ties among members of a university karate club.
+
+2. Dolphins: Dolphins represents a social network of bottlenose dolphins, with edges indicating frequent associations between dolphins.
+
+3. Jazz: Jazz illustrates a collaboration network among Jazz musicians, where edges signify instances of playing together in a band.
+
+4. Network Science: Network Science portrays a coauthorship network of scientists engaged in network theory and experimentation, with each edge representing co-authorship of a paper.
+
+5. Cora-ML: Cora-ML is a portal network of computer science research papers obtained through machine learning techniques.
+
+6. Power Grid: Power Grid delineates the topology network of the Western States Power Grid in the United States.
+
+7. Memetracker: Memetracker tracks frequently used phrases on news social media, and a small subset of the whole Memetracker network was retrieved here.
+
+8. Digg: Digg showcases a reply network within social news, and a small subset of the whole Digg network was retrieved here.
+
+# Installation
+
+#### Installation via PyPI
+```bash
+pip install GraphSL
+```
+
+#### Installation via GitHub
+Clone the repo from [here](https://github.com/xianggebenben/GraphSL) (this repo).
+
+Install requirements:
+```bash
+pip install -r requirements.txt
+```
+
+# Quickstart
+``` python
+
+   from GraphSL.data.utils import load_dataset, diffusion_generation, split_dataset
+   from GraphSL.Prescribed import LPSI, NetSleuth, OJC
+   from GraphSL.GNN.GCNSI.main import GCNSI
+   from GraphSL.GNN.IVGD.main import IVGD
+   from GraphSL.GNN.SLVAE.main import SLVAE
+   data_name = 'karate'  # 'karate', 'dolphins', 'jazz', 'netscience', 'cora_ml', 'power_grid', , 'meme8000', 'digg16000'
+   graph = load_dataset(data_name)
+   if data_name not in ['meme8000', 'digg16000']:
+       dataset = diffusion_generation(graph=graph, infect_prob=0.3, diff_type='IC', sim_num=100, seed_ratio=0.3)
+   else:
+       dataset = graph
+   adj, train_dataset, test_dataset =split_dataset(dataset)
+   lpsi = LPSI()
+   alpha, thres, auc, f1, pred =lpsi.train(adj, train_dataset)
+   print("LPSI:")
+   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+   metric=lpsi.test(adj, test_dataset, alpha, thres)
+   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+   netSleuth = NetSleuth()
+   k, auc, f1=netSleuth.train(adj, train_dataset)
+   print("NetSleuth:")
+   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+   metric = netSleuth.test(adj, test_dataset, k)
+   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+   ojc = OJC()
+   Y, auc, f1 =ojc.train(adj, train_dataset)
+   print("OJC:")
+   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+   metric=ojc.test(adj, test_dataset, Y)
+   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+   gcnsi = GCNSI()
+   gcnsi_model, thres, auc, f1, pred =gcnsi.train(adj, train_dataset)
+   print("GCNSI:")
+   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+   metric = gcnsi.test(adj, test_dataset, gcnsi_model, thres)
+   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+   ivgd = IVGD()
+   diffusion_model = ivgd.train_diffusion(adj, train_dataset)
+   ivgd_model, thres, auc, f1, pred =ivgd.train(adj, train_dataset, diffusion_model)
+   print("IVGD:")
+   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+   metric = ivgd.test(test_dataset, diffusion_model, ivgd_model, thres)
+   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+   slave = SLVAE()
+   slvae_model, seed_vae_train, thres, auc, f1, pred = slave.train(adj, train_dataset)
+   print("SLVAE:")
+   print(f"train auc: {auc:.3f}, train f1: {f1:.3f}")
+   metric = slave.infer(test_dataset, slvae_model, seed_vae_train, thres)
+   print(f"test acc: {metric.acc:.3f}, test pr: {metric.pr:.3f}, test re: {metric.re:.3f}, test f1: {metric.f1:.3f}, test auc: {metric.auc:.3f}")
+```
+
+# Documentation
+
+Official documentation, including a detailed [API reference](https://graphsl.readthedocs.io/en/latest/modules.html), is available on [Read the Docs](https://graphsl.readthedocs.io/en/latest/#).
+
+# Contact
+
+Feel free to Email Junxiang Wang (junxiang.wang@alumni.emory.edu) if you have any questions.
```


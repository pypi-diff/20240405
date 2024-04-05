# Comparing `tmp/codeflare_sdk-0.8.0.tar.gz` & `tmp/codeflare_sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.8.0.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.9.0.tar", max compression
```

## Comparing `codeflare_sdk-0.8.0.tar` & `codeflare_sdk-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-09-20 13:29:00.136572 codeflare_sdk-0.8.0/LICENSE
--rw-r--r--   0        0        0     4851 2023-09-20 13:29:00.136572 codeflare_sdk-0.8.0/README.md
--rw-r--r--   0        0        0     1232 2023-09-20 13:29:13.316635 codeflare_sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     6989 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0     3420 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/awload.py
--rw-r--r--   0        0        0    23839 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1726 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2159 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6660 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    15141 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0        0 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/utils/__init__.py
--rw-r--r--   0        0        0     5766 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/utils/generate_cert.py
--rwxr-xr-x   0        0        0    14267 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     1556 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/utils/kube_api_helpers.py
--rw-r--r--   0        0        0     6663 2023-09-20 13:29:00.144573 codeflare_sdk-0.8.0/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 codeflare_sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-11 18:35:55.540625 codeflare_sdk-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4851 2023-10-11 18:35:55.540625 codeflare_sdk-0.9.0/README.md
+-rw-r--r--   0        0        0     1203 2023-10-11 18:36:08.956786 codeflare_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     6989 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0     3420 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/awload.py
+-rw-r--r--   0        0        0    25080 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1798 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2214 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6660 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    15141 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0        0 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     5766 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/utils/generate_cert.py
+-rwxr-xr-x   0        0        0    15249 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     1556 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/utils/kube_api_helpers.py
+-rw-r--r--   0        0        0     6663 2023-10-11 18:35:55.548625 codeflare_sdk-0.9.0/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     5906 1970-01-01 00:00:00.000000 codeflare_sdk-0.9.0/PKG-INFO
```

### Comparing `codeflare_sdk-0.8.0/LICENSE` & `codeflare_sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/README.md` & `codeflare_sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/pyproject.toml` & `codeflare_sdk-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
@@ -19,21 +19,20 @@
 
 keywords = ['codeflare', 'python', 'sdk', 'client', 'batch', 'scale']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 openshift-client = "1.0.18"
 rich = "^12.5"
-ray = {version = "2.5.0", extras = ["default"]}
+ray = {version = "2.7.0", extras = ["default"]}
 kubernetes = ">= 25.3.0, < 27"
 codeflare-torchx = "0.6.0.dev1"
 cryptography = "40.0.2"
 executing = "1.2.0"
 pydantic = "< 2"
-pytorch-lightning = "^2.0.8"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 pdoc3 = "0.10.0"
```

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/auth.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/auth.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/awload.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/awload.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,17 @@
                     "Invalid Cluster Configuration, AppWrapper not generated"
                 )
         else:
             priority_val = None
 
         name = self.config.name
         namespace = self.config.namespace
+        head_cpus = self.config.head_cpus
+        head_memory = self.config.head_memory
+        head_gpus = self.config.head_gpus
         min_cpu = self.config.min_cpus
         max_cpu = self.config.max_cpus
         min_memory = self.config.min_memory
         max_memory = self.config.max_memory
         gpu = self.config.num_gpus
         workers = self.config.num_workers
         template = self.config.template
@@ -122,14 +125,17 @@
         env = self.config.envs
         local_interactive = self.config.local_interactive
         image_pull_secrets = self.config.image_pull_secrets
         dispatch_priority = self.config.dispatch_priority
         return generate_appwrapper(
             name=name,
             namespace=namespace,
+            head_cpus=head_cpus,
+            head_memory=head_memory,
+            head_gpus=head_gpus,
             min_cpu=min_cpu,
             max_cpu=max_cpu,
             min_memory=min_memory,
             max_memory=max_memory,
             gpu=gpu,
             workers=workers,
             template=template,
@@ -254,37 +260,50 @@
     def is_dashboard_ready(self) -> bool:
         response = requests.get(self.cluster_dashboard_uri(), timeout=5)
         if response.status_code == 200:
             return True
         else:
             return False
 
-    def wait_ready(self, timeout: Optional[int] = None):
+    def wait_ready(self, timeout: Optional[int] = None, dashboard_check: bool = True):
         """
         Waits for requested cluster to be ready, up to an optional timeout (s).
         Checks every five seconds.
         """
         print("Waiting for requested resources to be set up...")
         ready = False
         dashboard_ready = False
         status = None
         time = 0
-        while not ready or not dashboard_ready:
+        while not ready:
             status, ready = self.status(print_to_console=False)
-            dashboard_ready = self.is_dashboard_ready()
             if status == CodeFlareClusterStatus.UNKNOWN:
                 print(
                     "WARNING: Current cluster status is unknown, have you run cluster.up yet?"
                 )
-            if not ready or not dashboard_ready:
+            if not ready:
+                if timeout and time >= timeout:
+                    raise TimeoutError(
+                        f"wait() timed out after waiting {timeout}s for cluster to be ready"
+                    )
+                sleep(5)
+                time += 5
+        print("Requested cluster is up and running!")
+
+        while dashboard_check and not dashboard_ready:
+            dashboard_ready = self.is_dashboard_ready()
+            if not dashboard_ready:
                 if timeout and time >= timeout:
-                    raise TimeoutError(f"wait() timed out after waiting {timeout}s")
+                    raise TimeoutError(
+                        f"wait() timed out after waiting {timeout}s for dashboard to be ready"
+                    )
                 sleep(5)
                 time += 5
-        print("Requested cluster and dashboard are up and running!")
+        if dashboard_ready:
+            print("Dashboard is ready!")
 
     def details(self, print_to_console: bool = True) -> RayCluster:
         cluster = _copy_to_ray(self)
         if print_to_console:
             pretty_print.print_clusters([cluster])
         return cluster
 
@@ -604,14 +623,23 @@
         ][0]["resources"]["requests"]["memory"],
         worker_cpu=rc["spec"]["workerGroupSpecs"][0]["template"]["spec"]["containers"][
             0
         ]["resources"]["limits"]["cpu"],
         worker_gpu=0,  # hard to detect currently how many gpus, can override it with what the user asked for
         namespace=rc["metadata"]["namespace"],
         dashboard=ray_route,
+        head_cpus=rc["spec"]["headGroupSpec"]["template"]["spec"]["containers"][0][
+            "resources"
+        ]["limits"]["cpu"],
+        head_mem=rc["spec"]["headGroupSpec"]["template"]["spec"]["containers"][0][
+            "resources"
+        ]["limits"]["memory"],
+        head_gpu=rc["spec"]["headGroupSpec"]["template"]["spec"]["containers"][0][
+            "resources"
+        ]["limits"]["nvidia.com/gpu"],
     )
 
 
 def _map_to_app_wrapper(aw) -> AppWrapper:
     if "status" in aw and "canrun" in aw["status"]:
         return AppWrapper(
             name=aw["metadata"]["name"],
@@ -634,11 +662,14 @@
         workers=cluster.config.num_workers,
         worker_mem_min=cluster.config.min_memory,
         worker_mem_max=cluster.config.max_memory,
         worker_cpu=cluster.config.min_cpus,
         worker_gpu=cluster.config.num_gpus,
         namespace=cluster.config.namespace,
         dashboard=cluster.cluster_dashboard_uri(),
+        head_cpus=cluster.config.head_cpus,
+        head_mem=cluster.config.head_memory,
+        head_gpu=cluster.config.head_gpus,
     )
     if ray.status == CodeFlareClusterStatus.READY:
         ray.status = RayClusterStatus.READY
     return ray
```

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,21 +30,24 @@
     This dataclass is used to specify resource requirements and other details, and
     is passed in as an argument when creating a Cluster object.
     """
 
     name: str
     namespace: str = None
     head_info: list = field(default_factory=list)
+    head_cpus: int = 2
+    head_memory: int = 8
+    head_gpus: int = 0
     machine_types: list = field(default_factory=list)  # ["m4.xlarge", "g4dn.xlarge"]
     min_cpus: int = 1
     max_cpus: int = 1
     num_workers: int = 1
     min_memory: int = 2
     max_memory: int = 2
     num_gpus: int = 0
     template: str = f"{dir}/templates/base-template.yaml"
     instascale: bool = False
     envs: dict = field(default_factory=dict)
-    image: str = "quay.io/project-codeflare/ray:2.5.0-py38-cu116"
+    image: str = "quay.io/project-codeflare/ray:latest-py39-cu118"
     local_interactive: bool = False
     image_pull_secrets: list = field(default_factory=list)
     dispatch_priority: str = None
```

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/cluster/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 class RayCluster:
     """
     For storing information about a Ray cluster.
     """
 
     name: str
     status: RayClusterStatus
+    head_cpus: int
+    head_mem: str
+    head_gpu: int
     workers: int
     worker_mem_min: str
     worker_mem_max: str
     worker_cpu: int
     worker_gpu: int
     namespace: str
     dashboard: str
```

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/job/jobs.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/templates/base-template.yaml` & `codeflare_sdk-0.9.0/src/codeflare_sdk/templates/base-template.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             controller-tools.k8s.io: "1.0"
             # A unique identifier for the head node and workers of this cluster.
           name: kuberay-cluster
           # finalizers:
           # - kubernetes
         spec:
           # The version of Ray you are using. Make sure all Ray containers are running this version of Ray.
-          rayVersion: '2.5.0'
+          rayVersion: '2.7.0'
           # If enableInTreeAutoscaling is true, the autoscaler sidecar will be added to the Ray head pod.
           # Ray autoscaler integration is supported only for Ray versions >= 1.11.0
           # Ray autoscaler integration is Beta with KubeRay >= 0.3.0 and Ray >= 2.0.0.
           enableInTreeAutoscaling: false
           # autoscalerOptions is an OPTIONAL field specifying configuration overrides for the Ray autoscaler.
           # The example configuration shown below below represents the DEFAULT values.
           # (You may delete autoscalerOptions if the defaults are suitable.)
@@ -158,15 +158,15 @@
                     mountPath: "/home/ray/workspace/tls"
                     readOnly: true
                 initContainers:
                 - command:
                   - sh
                   - -c
                   - cd /home/ray/workspace/tls && openssl req -nodes -newkey rsa:2048 -keyout server.key -out server.csr -subj '/CN=ray-head' && printf "authorityKeyIdentifier=keyid,issuer\nbasicConstraints=CA:FALSE\nsubjectAltName = @alt_names\n[alt_names]\nDNS.1 = 127.0.0.1\nDNS.2 = localhost\nDNS.3 = ${FQ_RAY_IP}\nDNS.4 = $(awk 'END{print $1}' /etc/hosts)\nDNS.5 = rayclient-deployment-name-$(cat /var/run/secrets/kubernetes.io/serviceaccount/namespace).server-name">./domain.ext && cp /home/ray/workspace/ca/* . && openssl x509 -req -CA ca.crt -CAkey ca.key -in server.csr -out server.crt -days 365 -CAcreateserial -extfile domain.ext
-                  image: rayproject/ray:2.5.0
+                  image: rayproject/ray:2.7.0
                   name: create-cert
                   # securityContext:
                   #   runAsUser: 1000
                   #   runAsGroup: 1000
                   volumeMounts:
                   - name: ca-vol
                     mountPath: "/home/ray/workspace/ca"
@@ -223,15 +223,15 @@
                           - "aw-kuberay"
                 initContainers:
                 # the env var $RAY_IP is set by the operator if missing, with the value of the head service name
                 - name: init-myservice
                   image: busybox:1.28
                   command: ['sh', '-c', "until nslookup $RAY_IP.$(cat /var/run/secrets/kubernetes.io/serviceaccount/namespace).svc.cluster.local; do echo waiting for myservice; sleep 2; done"]
                 - name: create-cert
-                  image: rayproject/ray:2.5.0
+                  image: rayproject/ray:2.7.0
                   command:
                   - sh
                   - -c
                   - cd /home/ray/workspace/tls && openssl req -nodes -newkey rsa:2048 -keyout server.key -out server.csr -subj '/CN=ray-head' && printf "authorityKeyIdentifier=keyid,issuer\nbasicConstraints=CA:FALSE\nsubjectAltName = @alt_names\n[alt_names]\nDNS.1 = 127.0.0.1\nDNS.2 = localhost\nDNS.3 = ${FQ_RAY_IP}\nDNS.4 = $(awk 'END{print $1}' /etc/hosts)">./domain.ext && cp /home/ray/workspace/ca/* . && openssl x509 -req -CA ca.crt -CAkey ca.key -in server.csr -out server.crt -days 365 -CAcreateserial -extfile domain.ext
                   # securityContext:
                   #   runAsUser: 1000
                   #   runAsGroup: 1000
```

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/utils/generate_cert.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/utils/generate_cert.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,43 +103,59 @@
         head["template"]["spec"]["priorityClassName"] = dispatch_priority
         worker["template"]["spec"]["priorityClassName"] = dispatch_priority
     else:
         spec.pop("priority")
 
 
 def update_custompodresources(
-    item, min_cpu, max_cpu, min_memory, max_memory, gpu, workers
+    item,
+    min_cpu,
+    max_cpu,
+    min_memory,
+    max_memory,
+    gpu,
+    workers,
+    head_cpus,
+    head_memory,
+    head_gpus,
 ):
     if "custompodresources" in item.keys():
         custompodresources = item.get("custompodresources")
         for i in range(len(custompodresources)):
+            resource = custompodresources[i]
             if i == 0:
                 # Leave head node resources as template default
-                continue
-            resource = custompodresources[i]
-            for k, v in resource.items():
-                if k == "replicas" and i == 1:
-                    resource[k] = workers
-                if k == "requests" or k == "limits":
-                    for spec, _ in v.items():
-                        if spec == "cpu":
-                            if k == "limits":
-                                resource[k][spec] = max_cpu
-                            else:
-                                resource[k][spec] = min_cpu
-                        if spec == "memory":
-                            if k == "limits":
-                                resource[k][spec] = str(max_memory) + "G"
-                            else:
-                                resource[k][spec] = str(min_memory) + "G"
-                        if spec == "nvidia.com/gpu":
-                            if i == 0:
-                                resource[k][spec] = 0
-                            else:
-                                resource[k][spec] = gpu
+                resource["requests"]["cpu"] = head_cpus
+                resource["limits"]["cpu"] = head_cpus
+                resource["requests"]["memory"] = str(head_memory) + "G"
+                resource["limits"]["memory"] = str(head_memory) + "G"
+                resource["requests"]["nvidia.com/gpu"] = head_gpus
+                resource["limits"]["nvidia.com/gpu"] = head_gpus
+
+            else:
+                for k, v in resource.items():
+                    if k == "replicas" and i == 1:
+                        resource[k] = workers
+                    if k == "requests" or k == "limits":
+                        for spec, _ in v.items():
+                            if spec == "cpu":
+                                if k == "limits":
+                                    resource[k][spec] = max_cpu
+                                else:
+                                    resource[k][spec] = min_cpu
+                            if spec == "memory":
+                                if k == "limits":
+                                    resource[k][spec] = str(max_memory) + "G"
+                                else:
+                                    resource[k][spec] = str(min_memory) + "G"
+                            if spec == "nvidia.com/gpu":
+                                if i == 0:
+                                    resource[k][spec] = 0
+                                else:
+                                    resource[k][spec] = gpu
     else:
         sys.exit("Error: malformed template")
 
 
 def update_affinity(spec, appwrapper_name, instascale):
     if instascale:
         node_selector_terms = (
@@ -201,19 +217,23 @@
     max_memory,
     gpu,
     workers,
     image,
     instascale,
     env,
     image_pull_secrets,
+    head_cpus,
+    head_memory,
+    head_gpus,
 ):
     if "generictemplate" in item.keys():
         head = item.get("generictemplate").get("spec").get("headGroupSpec")
-        worker = item.get("generictemplate").get("spec").get("workerGroupSpecs")[0]
+        head["rayStartParams"]["num-gpus"] = str(int(head_gpus))
 
+        worker = item.get("generictemplate").get("spec").get("workerGroupSpecs")[0]
         # Head counts as first worker
         worker["replicas"] = workers
         worker["minReplicas"] = workers
         worker["maxReplicas"] = workers
         worker["groupName"] = "small-group-" + appwrapper_name
         worker["rayStartParams"]["num-gpus"] = str(int(gpu))
 
@@ -221,15 +241,17 @@
             spec = comp.get("template").get("spec")
             update_affinity(spec, appwrapper_name, instascale)
             update_image_pull_secrets(spec, image_pull_secrets)
             update_image(spec, image)
             update_env(spec, env)
             if comp == head:
                 # TODO: Eventually add head node configuration outside of template
-                continue
+                update_resources(
+                    spec, head_cpus, head_cpus, head_memory, head_memory, head_gpus
+                )
             else:
                 update_resources(spec, min_cpu, max_cpu, min_memory, max_memory, gpu)
 
 
 def update_ca_secret(ca_secret_item, cluster_name, namespace):
     from . import generate_cert
 
@@ -346,14 +368,17 @@
         yaml.dump(user_yaml, outfile, default_flow_style=False)
     print(f"Written to: {output_file_name}")
 
 
 def generate_appwrapper(
     name: str,
     namespace: str,
+    head_cpus: int,
+    head_memory: int,
+    head_gpus: int,
     min_cpu: int,
     max_cpu: int,
     min_memory: int,
     max_memory: int,
     gpu: int,
     workers: int,
     template: str,
@@ -371,29 +396,41 @@
     resources = user_yaml.get("spec", "resources")
     item = resources["resources"].get("GenericItems")[0]
     route_item = resources["resources"].get("GenericItems")[1]
     update_names(user_yaml, item, appwrapper_name, cluster_name, namespace)
     update_labels(user_yaml, instascale, instance_types)
     update_priority(user_yaml, item, dispatch_priority, priority_val)
     update_custompodresources(
-        item, min_cpu, max_cpu, min_memory, max_memory, gpu, workers
+        item,
+        min_cpu,
+        max_cpu,
+        min_memory,
+        max_memory,
+        gpu,
+        workers,
+        head_cpus,
+        head_memory,
+        head_gpus,
     )
     update_nodes(
         item,
         appwrapper_name,
         min_cpu,
         max_cpu,
         min_memory,
         max_memory,
         gpu,
         workers,
         image,
         instascale,
         env,
         image_pull_secrets,
+        head_cpus,
+        head_memory,
+        head_gpus,
     )
     update_dashboard_route(route_item, cluster_name, namespace)
     if local_interactive:
         enable_local_interactive(resources, cluster_name, namespace)
     else:
         disable_raycluster_tls(resources["resources"])
     outfile = appwrapper_name + ".yaml"
```

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/utils/kube_api_helpers.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/utils/kube_api_helpers.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.9.0/src/codeflare_sdk/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.8.0/PKG-INFO` & `codeflare_sdk-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflare-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python SDK for codeflare client
 Home-page: https://github.com/project-codeflare/codeflare-sdk
 License: Apache-2.0
 Keywords: codeflare,python,sdk,client,batch,scale
 Author: Michael Clifford
 Author-email: mcliffor@redhat.com
 Requires-Python: >=3.8,<4.0
@@ -16,16 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: codeflare-torchx (==0.6.0.dev1)
 Requires-Dist: cryptography (==40.0.2)
 Requires-Dist: executing (==1.2.0)
 Requires-Dist: kubernetes (>=25.3.0,<27)
 Requires-Dist: openshift-client (==1.0.18)
 Requires-Dist: pydantic (<2)
-Requires-Dist: pytorch-lightning (>=2.0.8,<3.0.0)
-Requires-Dist: ray[default] (==2.5.0)
+Requires-Dist: ray[default] (==2.7.0)
 Requires-Dist: rich (>=12.5,<13.0)
 Project-URL: Repository, https://github.com/project-codeflare/codeflare-sdk
 Description-Content-Type: text/markdown
 
 # Codeflare-SDK
 
 [![Python application](https://github.com/project-codeflare/codeflare-sdk/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/project-codeflare/codeflare-sdk/actions/workflows/unit-tests.yml)
```


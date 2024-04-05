# Comparing `tmp/binharness-0.1.0.tar.gz` & `tmp/binharness-0.1.1.tar.gz`

## Comparing `binharness-0.1.0.tar` & `binharness-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0     1001      127      547 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_common/Cargo.toml
--rw-r--r--   0     1001      127     1742 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_common/src/agent_error.rs
--rw-r--r--   0     1001      127      104 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_common/src/lib.rs
--rw-r--r--   0     1001      127     3205 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_common/src/service.rs
--rw-r--r--   0     1001      127     1880 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_common/src/types.rs
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 binharness-0.1.0/crates/bh_agent_client/Cargo.toml
--rw-r--r--   0     1001      127    12435 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_client/src/bindings.rs
--rw-r--r--   0     1001      127      502 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_client/src/client.rs
--rw-r--r--   0     1001      127       62 2024-02-14 04:04:46.000000 binharness-0.1.0/crates/bh_agent_client/src/lib.rs
--rw-r--r--   0     1001      127    34770 2024-02-14 04:04:52.000000 binharness-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      144 1970-01-01 00:00:00.000000 binharness-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2117 2024-02-14 04:04:46.000000 binharness-0.1.0/pyproject.toml
--rw-r--r--   0     1001      127     3211 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/serialize.py
--rw-r--r--   0     1001      127     4538 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/localenvironment.py
--rw-r--r--   0     1001      127     1539 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/util.py
--rw-r--r--   0     1001      127    10794 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/agentenvironment.py
--rw-r--r--   0     1001      127     1348 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/__init__.py
--rw-r--r--   0     1001      127     1493 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/agentprovider.py
--rw-r--r--   0     1001      127        0 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/py.typed
--rw-r--r--   0     1001      127     2762 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/bootstrap/ssh.py
--rw-r--r--   0     1001      127     2761 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/bootstrap/docker.py
--rw-r--r--   0     1001      127       65 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/bootstrap/__init__.py
--rw-r--r--   0     1001      127     1155 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/bootstrap/subprocess.py
--rw-r--r--   0     1001      127     2655 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/common/qemu.py
--rw-r--r--   0     1001      127     2933 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/common/busybox.py
--rw-r--r--   0     1001      127      272 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/common/__init__.py
--rw-r--r--   0     1001      127     1326 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/stat.py
--rw-r--r--   0     1001      127     2628 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/environment.py
--rw-r--r--   0     1001      127     3376 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/injection.py
--rw-r--r--   0     1001      127     1851 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/executor.py
--rw-r--r--   0     1001      127     1997 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/io.py
--rw-r--r--   0     1001      127     2478 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/process.py
--rw-r--r--   0     1001      127      931 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/__init__.py
--rw-r--r--   0     1001      127      992 2024-02-14 04:04:46.000000 binharness-0.1.0/python/binharness/types/target.py
--rw-r--r--   0     1001      127     5603 2024-02-14 04:04:46.000000 binharness-0.1.0/README.md
--rw-r--r--   0     1001      127     1307 2024-02-14 04:04:46.000000 binharness-0.1.0/LICENSE
--rw-r--r--   0        0        0     6835 1970-01-01 00:00:00.000000 binharness-0.1.0/PKG-INFO
+-rw-r--r--   0     1001      127      547 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_common/Cargo.toml
+-rw-r--r--   0     1001      127     1742 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_common/src/agent_error.rs
+-rw-r--r--   0     1001      127      104 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_common/src/lib.rs
+-rw-r--r--   0     1001      127     3704 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_common/src/service.rs
+-rw-r--r--   0     1001      127     1880 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_common/src/types.rs
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 binharness-0.1.1/crates/bh_agent_client/Cargo.toml
+-rw-r--r--   0     1001      127    14262 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_client/src/bindings.rs
+-rw-r--r--   0     1001      127      502 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_client/src/client.rs
+-rw-r--r--   0     1001      127       62 2024-04-05 01:00:48.000000 binharness-0.1.1/crates/bh_agent_client/src/lib.rs
+-rw-r--r--   0     1001      127    38115 2024-04-05 01:00:55.000000 binharness-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      144 1970-01-01 00:00:00.000000 binharness-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     2154 2024-04-05 01:00:48.000000 binharness-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      127     1411 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/__init__.py
+-rw-r--r--   0     1001      127      272 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/common/__init__.py
+-rw-r--r--   0     1001      127     2933 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/common/busybox.py
+-rw-r--r--   0     1001      127     2655 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/common/qemu.py
+-rw-r--r--   0     1001      127     8186 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/localenvironment.py
+-rw-r--r--   0     1001      127        0 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/py.typed
+-rw-r--r--   0     1001      127    12017 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/agentenvironment.py
+-rw-r--r--   0     1001      127      931 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/__init__.py
+-rw-r--r--   0     1001      127      992 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/target.py
+-rw-r--r--   0     1001      127     3527 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/environment.py
+-rw-r--r--   0     1001      127     2173 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/io.py
+-rw-r--r--   0     1001      127     1326 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/stat.py
+-rw-r--r--   0     1001      127     3376 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/injection.py
+-rw-r--r--   0     1001      127     2606 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/process.py
+-rw-r--r--   0     1001      127     1851 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/types/executor.py
+-rw-r--r--   0     1001      127     1539 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/util.py
+-rw-r--r--   0     1001      127     1493 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/agentprovider.py
+-rw-r--r--   0     1001      127       65 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/bootstrap/__init__.py
+-rw-r--r--   0     1001      127     2762 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/bootstrap/ssh.py
+-rw-r--r--   0     1001      127     1180 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/bootstrap/subprocess.py
+-rw-r--r--   0     1001      127     2761 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/bootstrap/docker.py
+-rw-r--r--   0     1001      127     3535 2024-04-05 01:00:48.000000 binharness-0.1.1/python/binharness/serialize.py
+-rw-r--r--   0     1001      127     5603 2024-04-05 01:00:48.000000 binharness-0.1.1/README.md
+-rw-r--r--   0     1001      127     1307 2024-04-05 01:00:48.000000 binharness-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6835 1970-01-01 00:00:00.000000 binharness-0.1.1/PKG-INFO
```

### Comparing `binharness-0.1.0/crates/bh_agent_common/Cargo.toml` & `binharness-0.1.1/crates/bh_agent_common/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "bh_agent_common"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 anyhow = { version = "1.0.75", features = [] }
-tarpc = { version = "0.33.0", features = ["tokio1"] }
+tarpc = { version = "0.34.0", features = ["tokio1"] }
 serde = { version = "1.0.188", features = ["derive"] }
 thiserror = "1.0.48"
-pyo3 = { version = "0.19.0", optional = true }
+pyo3 = { version = "0.20.3", optional = true }
 
 [target.'cfg(target_family = "unix")'.dependencies]
-nix = { version = "0.27.1", features = ["fs", "user"] }
+nix = { version = "0.28.0", features = ["fs", "user"] }
 
 [features]
 python = ["pyo3"]
```

### Comparing `binharness-0.1.0/crates/bh_agent_common/src/agent_error.rs` & `binharness-0.1.1/crates/bh_agent_common/src/agent_error.rs`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/crates/bh_agent_common/src/service.rs` & `binharness-0.1.1/crates/bh_agent_common/src/service.rs`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
     // Process management
     async fn run_command(
         env_id: EnvironmentId,
         config: RemotePOpenConfig,
     ) -> Result<ProcessId, AgentError>;
 
+    async fn get_process_ids(env_id: EnvironmentId) -> Result<Vec<ProcessId>, AgentError>;
+
     async fn get_process_channel(
         env_id: EnvironmentId,
         proc_id: ProcessId,
         channel: ProcessChannel,
     ) -> Result<FileId, AgentError>;
 
     async fn process_poll(
@@ -83,18 +85,34 @@
     async fn file_tell(env_id: EnvironmentId, fd: FileId) -> Result<i32, AgentError>;
 
     async fn file_is_writable(env_id: EnvironmentId, fd: FileId) -> Result<bool, AgentError>;
 
     async fn file_write(env_id: EnvironmentId, fd: FileId, data: Vec<u8>)
         -> Result<(), AgentError>;
 
+    async fn file_set_blocking(
+        env_id: EnvironmentId,
+        fd: FileId,
+        blocking: bool,
+    ) -> Result<(), AgentError>;
+
     async fn chown(
         env_id: EnvironmentId,
         path: String,
         user: Option<UserId>,
         group: Option<UserId>,
     ) -> Result<(), AgentError>;
 
     async fn chmod(env_id: EnvironmentId, path: String, mode: u32) -> Result<(), AgentError>;
 
     async fn stat(env_id: EnvironmentId, path: String) -> Result<FileStat, AgentError>;
+
+    // Metadata API
+    async fn get_metadata(env_id: EnvironmentId, key: String)
+        -> Result<Option<String>, AgentError>;
+
+    async fn set_metadata(
+        env_id: EnvironmentId,
+        key: String,
+        value: String,
+    ) -> Result<(), AgentError>;
 }
```

### Comparing `binharness-0.1.0/crates/bh_agent_common/src/types.rs` & `binharness-0.1.1/crates/bh_agent_common/src/types.rs`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/crates/bh_agent_client/src/bindings.rs` & `binharness-0.1.1/crates/bh_agent_client/src/bindings.rs`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 };
 use log::debug;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 use pyo3::{pyclass, pymethods, pymodule, PyResult, Python};
 use std::future::Future;
-use std::net::{IpAddr, SocketAddr};
+use std::net::{IpAddr, SocketAddr, ToSocketAddrs};
 use std::str::FromStr;
 use tarpc::client::RpcError;
 use tarpc::context;
 use tokio::runtime;
 
 #[pyclass]
 struct BhAgentClient {
@@ -33,19 +33,31 @@
         .map(|r| r.map_err(|e| PyRuntimeError::new_err(e.to_string())))
         .and_then(|r| r)
 }
 
 #[pymethods]
 impl BhAgentClient {
     #[staticmethod]
-    fn initialize_client(ip_addr: String, port: u16) -> PyResult<Self> {
-        debug!("Initializing client with {}:{}", ip_addr, port);
+    fn initialize_client(host: String, port: u16) -> PyResult<Self> {
+        debug!("Initializing client with {}:{}", host, port);
 
-        let ip_addr = IpAddr::from_str(&ip_addr)?;
-        let socket_addr = SocketAddr::new(ip_addr, port);
+        let socket_addr = match format!("{}:{}", host, port).to_socket_addrs() {
+            Ok(mut addrs) => match addrs.next() {
+                Some(addr) => addr,
+                None => {
+                    return Err(PyRuntimeError::new_err("Failed to resolve address"));
+                }
+            },
+            Err(e) => {
+                return Err(PyRuntimeError::new_err(format!(
+                    "Failed to resolve address: {}",
+                    e
+                )));
+            }
+        };
 
         let tokio_runtime = runtime::Builder::new_current_thread()
             .enable_all()
             .build()
             .unwrap();
         match tokio_runtime.block_on(build_client(socket_addr)) {
             Ok(client) => Ok(Self {
@@ -81,18 +93,18 @@
         stdout: bool,
         stderr: bool,
         executable: Option<String>,
         env: Option<Vec<(String, String)>>,
         cwd: Option<String>,
         setuid: Option<u32>,
         setgid: Option<u32>,
-        setpgid: bool,
+        setpgid: Option<bool>,
     ) -> PyResult<ProcessId> {
         debug!(
-            "Running process with argv {:?}, stdin {}, stdout {}, stderr {}, executable {:?}, env {:?}, cwd {:?}, setuid {:?}, setgid {:?}, setpgid {}",
+            "Running process with argv {:?}, stdin {}, stdout {}, stderr {}, executable {:?}, env {:?}, cwd {:?}, setuid {:?}, setgid {:?}, setpgid {:?}",
             argv,
             stdin,
             stdout,
             stderr,
             executable,
             env,
             cwd,
@@ -115,22 +127,31 @@
                 false => Redirection::None,
             },
             executable,
             env,
             cwd,
             setuid,
             setgid,
-            setpgid,
+            setpgid: setpgid.unwrap_or(false),
         };
         run_in_runtime(
             self,
             self.client.run_command(context::current(), env_id, config),
         )
     }
 
+    fn get_process_ids(&self, env_id: EnvironmentId) -> PyResult<Vec<ProcessId>> {
+        debug!("Getting process ids for environment {}", env_id);
+
+        run_in_runtime(
+            self,
+            self.client.get_process_ids(context::current(), env_id),
+        )
+    }
+
     fn get_process_channel(
         &self,
         env_id: EnvironmentId,
         proc_id: ProcessId,
         channel: i32, // TODO: This is just 0, 1, 2 for now
     ) -> PyResult<FileId> {
         debug!(
@@ -379,14 +400,27 @@
 
         run_in_runtime(
             self,
             self.client.file_write(context::current(), env_id, fd, data),
         )
     }
 
+    fn file_set_blocking(&self, env_id: EnvironmentId, fd: FileId, blocking: bool) -> PyResult<()> {
+        debug!(
+            "Setting file blocking for environment {}, fd {}, blocking {}",
+            env_id, fd, blocking
+        );
+
+        run_in_runtime(
+            self,
+            self.client
+                .file_set_blocking(context::current(), env_id, fd, blocking),
+        )
+    }
+
     fn chown(
         &self,
         env_id: EnvironmentId,
         path: String,
         user: Option<String>,
         group: Option<String>,
     ) -> PyResult<()> {
@@ -424,14 +458,36 @@
     }
 
     fn stat(&self, env_id: EnvironmentId, path: String) -> PyResult<FileStat> {
         debug!("Stating file for environment {}, path {}", env_id, path);
 
         run_in_runtime(self, self.client.stat(context::current(), env_id, path))
     }
+
+    // Metadata API
+    fn get_metadata(&self, env_id: EnvironmentId, key: String) -> PyResult<Option<String>> {
+        debug!("Getting metadata for environment {}, key {}", env_id, key);
+        run_in_runtime(
+            self,
+            self.client.get_metadata(context::current(), env_id, key),
+        )
+    }
+
+    fn set_metadata(&self, env_id: EnvironmentId, key: String, value: String) -> PyResult<()> {
+        debug!(
+            "Setting metadata for environment {}, key {}, value {}",
+            env_id, key, value
+        );
+
+        run_in_runtime(
+            self,
+            self.client
+                .set_metadata(context::current(), env_id, key, value),
+        )
+    }
 }
 
 #[pymodule]
 pub fn bh_agent_client(_py: Python, m: &PyModule) -> PyResult<()> {
     pyo3_log::init();
     m.add_class::<FileStat>()?;
     m.add_class::<BhAgentClient>()?;
```

### Comparing `binharness-0.1.0/Cargo.lock` & `binharness-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,72 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "anstream"
+version = "0.6.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+dependencies = [
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "3.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+dependencies = [
+ "anstyle",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "anyhow"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "arc-swap"
-version = "1.6.0"
+version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "argh"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7af5ba06967ff7214ce4c7419c7d185be7ecd6cc4965a8f6e1d8ce0398aad219"
 dependencies = [
@@ -44,100 +92,101 @@
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56df0aeedf6b7a2fc67d06db35b09684c3e8da0c95f8f27685cb17e08413d87a"
 dependencies = [
  "argh_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "argh_shared"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5693f39141bda5760ecc4111ab08da40565d1771038c4a0250f03457ec707531"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.77"
+version = "0.1.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
+checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "bh_agent_client"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "bh_agent_common",
  "log",
  "pyo3",
  "pyo3-log",
  "tarpc",
  "tokio",
 ]
 
 [[package]]
 name = "bh_agent_common"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "nix",
  "pyo3",
  "serde",
  "tarpc",
  "thiserror",
 ]
 
 [[package]]
 name = "bh_agent_server"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "argh",
  "bh_agent_common",
  "bimap",
  "daemonize",
  "env_logger",
  "futures",
  "log",
  "nix",
  "subprocess",
  "tarpc",
  "tokio",
  "unicode_reader",
+ "which",
 ]
 
 [[package]]
 name = "bimap"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "230c5f1ca6a325a32553f8640d31ac9b49f2411e901e427570154868b46da4f7"
@@ -155,50 +204,59 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cfg_aliases"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "crossbeam-channel"
-version = "0.5.11"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176dc175b78f56c0f321911d9c8eb2b77a78a4860b9c19db83835fea1a46649b"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
@@ -223,36 +281,62 @@
  "enum-ordinalize",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "either"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+
+[[package]]
 name = "enum-ordinalize"
 version = "3.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bf1fa3f06bbff1ea5b1a9c7b14aa992a39657db60a2759457328d7e058f49ee"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "env_filter"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a009aa4810eb158359dda09d0c87378e4bbb89b5a801f016885a4707ba24f7ea"
+dependencies = [
+ "log",
 ]
 
 [[package]]
 name = "env_logger"
-version = "0.10.2"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
+checksum = "38b35839ba51819680ba087cd351788c9a3c476841207e0b8cee0b04722343b9"
 dependencies = [
+ "anstream",
+ "anstyle",
+ "env_filter",
  "humantime",
- "is-terminal",
  "log",
- "termcolor",
+]
+
+[[package]]
+name = "errno"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+dependencies = [
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
@@ -309,15 +393,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -366,18 +450,33 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
+
+[[package]]
+name = "home"
+version = "0.5.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
+dependencies = [
+ "windows-sys 0.52.0",
+]
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
@@ -389,40 +488,29 @@
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "is-terminal"
-version = "0.4.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
-dependencies = [
- "hermit-abi",
- "libc",
- "windows-sys 0.52.0",
-]
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -432,40 +520,46 @@
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+
+[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.7.2"
@@ -473,31 +567,32 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nix"
-version = "0.27.1"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2eb04e9c688eff1c89d72b407f168cf79bb9e867a9d3323ed6c01519eb9cc053"
+checksum = "ab2156c4fce2f8df6c499cc1c763e4394b7482525bf2a9701c9d79d215f519e4"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cfg-if",
+ "cfg_aliases",
  "libc",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -621,91 +716,98 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project"
-version = "1.1.4"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0302c4a0442c456bd56f841aee5c3bfd17967563f6fadc9ceb9f9c23cf3807e0"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.4"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266c042b60c9c76b8d53061e52b2e0d1116abc57cefc8c5cd671619a56ac3690"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -716,33 +818,35 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -792,50 +896,63 @@
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
+name = "rustix"
+version = "0.38.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+dependencies = [
+ "bitflags 2.5.0",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -854,26 +971,26 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -897,34 +1014,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tarpc"
-version = "0.33.0"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f41bce44d290df0598ae4b9cd6ea7f58f651fd3aa4af1b26060c4fa32b08af7"
+checksum = "93a1870169fb9490fb3b37df7f50782986475c33cb90955f9f9b9ae659124200"
 dependencies = [
  "anyhow",
  "fnv",
  "futures",
  "humantime",
  "opentelemetry",
  "pin-project",
@@ -938,67 +1055,58 @@
  "tokio-util",
  "tracing",
  "tracing-opentelemetry",
 ]
 
 [[package]]
 name = "tarpc-plugins"
-version = "0.12.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ee42b4e559f17bce0385ebf511a7beb67d5cc33c12c96b7f4e9789919d9c10f"
+checksum = "ad8302bea2fb8a2b01b025d23414b0b4ed32a783b95e5d818c3320a8bc4baada"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "termcolor"
-version = "1.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
@@ -1052,15 +1160,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1113,17 +1221,23 @@
 dependencies = [
  "smallvec",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
+
+[[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
@@ -1131,65 +1245,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
+
+[[package]]
+name = "which"
+version = "6.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "8211e4f58a2b2805adfbefbc07bab82958fc91e3836339b1ab7ae32465dce0d7"
+dependencies = [
+ "either",
+ "home",
+ "rustix",
+ "winsafe",
+]
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -1200,23 +1326,14 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-util"
-version = "0.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
@@ -1229,15 +1346,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1249,103 +1366,109 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+
+[[package]]
+name = "winsafe"
+version = "0.0.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "d135d17ab770252ad95e9a872d365cf3090e3be864a34ab46f48555993efc904"
```

### Comparing `binharness-0.1.0/pyproject.toml` & `binharness-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 [tool.maturin]
 bindings = "pyo3"
 manifest-path = "crates/bh_agent_client/Cargo.toml"
 python-source = "python"
 python-packages = ["binharness"]
 strip = true
 sdist-generator = "cargo"
+features = ["pyo3/extension-module"]
 
 [tool.pytest.ini_options]
 addopts = "-ra --cov=binharness --cov-report lcov:.lcov --cov-report term-missing --mypy"
 markers = ["linux", "darwin", "win32"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `binharness-0.1.0/python/binharness/serialize.py` & `binharness-0.1.1/python/binharness/serialize.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,7 +87,14 @@
         return Target(
             environment,
             env_install_dir / main_binary,
             [env_install_dir / binary for binary in extra_binaries],
             args,
             env,
         )
+
+
+def transport_target(target: Target, new_env: Environment) -> Target:
+    """Transport a target to a new environment by exporting and importing it."""
+    with tempfile.NamedTemporaryFile() as export_file:
+        export_target(target, Path(export_file.name))
+        return import_target(new_env, Path(export_file.name))
```

### Comparing `binharness-0.1.0/python/binharness/util.py` & `binharness-0.1.1/python/binharness/util.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/agentenvironment.py` & `binharness-0.1.1/python/binharness/agentenvironment.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         """Write to the file."""
         return self._client.file_write(self._environment_id, self._fd, s)
 
     def writelines(self: AgentIO, lines: list[bytes]) -> None:
         """Write lines to the file."""
         self._client.file_write(self._environment_id, self._fd, b"\n".join(lines))
 
+    def set_blocking(self: AgentIO, blocking: bool) -> None:  # noqa: FBT001
+        """Set the file to non-blocking mode."""
+        self._client.file_set_blocking(self._environment_id, self._fd, blocking)
+
 
 class AgentProcess(Process):
     """A process running in an agent environment."""
 
     _client: BhAgentClient
     _env_id: int
     _pid: int
@@ -111,14 +115,19 @@
     ) -> None:
         """Create an AgentProcess."""
         super().__init__(environment, args, env, cwd)
         self._client = client
         self._env_id = env_id
         self._pid = pid
 
+    @property
+    def pid(self: AgentProcess) -> int:
+        """Get the process' PID."""
+        return self._pid
+
     @cached_property
     def stdin(self: AgentProcess) -> AgentIO | None:
         """Get the standard input stream of the process."""
         try:
             fd = self._client.get_process_channel(self._env_id, self._pid, 0)
             return AgentIO(self._client, self._env_id, fd)
         except RuntimeError:
@@ -197,14 +206,24 @@
             pid,
             self,
             normalized_args,
             env,
             cwd,
         )
 
+    def get_process_ids(self: AgentEnvironment) -> list[int]:
+        """Get the PIDs of all processes managed by binharness in the environment."""
+        return self._client.get_process_ids(self._id)
+
+    def get_process(self: AgentEnvironment, pid: int) -> Process:
+        """Get a process by PID."""
+        # TODO: These last three arguments are a lie. We need to store these on
+        # the agent at the time of process creation, and then retrieve them here.
+        return AgentProcess(self._client, self._id, pid, self, [], None, None)
+
     def inject_files(self: AgentEnvironment, files: list[tuple[Path, Path]]) -> None:
         """Inject files into the environment."""
         for src, dst in files:
             # TODO: Need a more robust solution to this. Current solution fixes
             #  the common case where we're injecting into the system temp dir,
             #  which presumably already exists.
             try:
@@ -259,14 +278,24 @@
         """Change the mode of a file."""
         self._client.chmod(self._id, str(path), mode)
 
     def stat(self: AgentEnvironment, path: Path) -> FileStat:
         """Get the stat of a file."""
         return FileStat.from_agent(self._client.stat(self._id, str(path)))
 
+    # Metadata API
+
+    def get_metadata(self: AgentEnvironment, key: str) -> str | None:
+        """Get a metadata value."""
+        return self._client.get_metadata(self._id, key)
+
+    def set_metadata(self: AgentEnvironment, key: str, value: str) -> None:
+        """Set a metadata value."""
+        self._client.set_metadata(self._id, key, value)
+
 
 class AgentConnection:
     """AgentConnection represents a connection to an agent.
 
     It serves as the main interface for interacting with the agent client.
     """
```

### Comparing `binharness-0.1.0/python/binharness/__init__.py` & `binharness-0.1.1/python/binharness/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """binharness - A library for analyzing a program in its environment."""
 
 from __future__ import annotations
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 from binharness.agentenvironment import AgentConnection, AgentEnvironment
 from binharness.agentprovider import AgentProvider, DevEnvironmentAgentProvider
 from binharness.common import BusyboxInjection
 from binharness.localenvironment import LocalEnvironment
-from binharness.serialize import TargetImportError, export_target, import_target
+from binharness.serialize import (
+    TargetImportError,
+    export_target,
+    import_target,
+    transport_target,
+)
 from binharness.types import (
     IO,
     Environment,
     ExecutableInjection,
     Executor,
     ExecutorEnvironmentMismatchError,
     ExecutorError,
@@ -46,8 +51,9 @@
     "LocalEnvironment",
     "NullExecutor",
     "Process",
     "Target",
     "TargetImportError",
     "export_target",
     "import_target",
+    "transport_target",
 ]
```

### Comparing `binharness-0.1.0/python/binharness/agentprovider.py` & `binharness-0.1.1/python/binharness/agentprovider.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/bootstrap/ssh.py` & `binharness-0.1.1/python/binharness/bootstrap/ssh.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/bootstrap/docker.py` & `binharness-0.1.1/python/binharness/bootstrap/docker.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/common/qemu.py` & `binharness-0.1.1/python/binharness/common/qemu.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/common/busybox.py` & `binharness-0.1.1/python/binharness/common/busybox.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/types/stat.py` & `binharness-0.1.1/python/binharness/types/stat.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/types/environment.py` & `binharness-0.1.1/python/binharness/types/environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,24 @@
 
         The command is run as a process in the environment. For now, arguments
         are passed to Process as-is.
         """
         raise NotImplementedError
 
     @abstractmethod
+    def get_process_ids(self: Environment) -> list[int]:
+        """Get the PIDs of all processes managed by binharness in the environment."""
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_process(self: Environment, pid: int) -> Process:
+        """Get a process by PID."""
+        raise NotImplementedError
+
+    @abstractmethod
     def inject_files(
         self: Environment,
         files: list[tuple[Path, Path]],
     ) -> None:
         """Inject files into the environment.
 
         The first element of the tuple is the path to the file on the host
@@ -79,7 +89,22 @@
         """Change the mode of a file."""
         raise NotImplementedError
 
     @abstractmethod
     def stat(self: Environment, path: Path) -> FileStat:
         """Get the stat of a file."""
         raise NotImplementedError
+
+    # Metadata API
+    # Binharness environments have a simple key-value store applications can use
+    # to persistantly store metadata about processes and files, or any other
+    # information they need to persist between runs.
+
+    @abstractmethod
+    def get_metadata(self: Environment, key: str) -> str | None:
+        """Get a metadata value."""
+        raise NotImplementedError
+
+    @abstractmethod
+    def set_metadata(self: Environment, key: str, value: str) -> None:
+        """Set a metadata value."""
+        raise NotImplementedError
```

### Comparing `binharness-0.1.0/python/binharness/types/injection.py` & `binharness-0.1.1/python/binharness/types/injection.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/types/executor.py` & `binharness-0.1.1/python/binharness/types/executor.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/types/io.py` & `binharness-0.1.1/python/binharness/types/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,7 +60,11 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Exit the runtime context and close the file if it's open."""
         if not self.closed:
             self.close()
+
+    def set_blocking(self: IO[AnyStr], blocking: bool) -> None:  # noqa: FBT001
+        """Set the file to blocking or non-blocking mode."""
+        raise NotImplementedError
```

### Comparing `binharness-0.1.0/python/binharness/types/process.py` & `binharness-0.1.1/python/binharness/types/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,19 @@
         """Create a Process."""
         self.environment = environment
         self.args = args
         self.env = env or {}
         self.cwd = cwd or environment.get_tempdir()
 
     @abstractproperty
+    def pid(self: Process) -> int:
+        """Get the process' PID."""
+        raise NotImplementedError
+
+    @abstractproperty
     def stdin(self: Process) -> IO[bytes] | None:
         """Get the standard input stream of the process."""
         raise NotImplementedError
 
     @abstractproperty
     def stdout(self: Process) -> IO[bytes] | None:
         """Get the standard output stream of the process."""
```

### Comparing `binharness-0.1.0/python/binharness/types/__init__.py` & `binharness-0.1.1/python/binharness/types/__init__.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/python/binharness/types/target.py` & `binharness-0.1.1/python/binharness/types/target.py`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/README.md` & `binharness-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/LICENSE` & `binharness-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `binharness-0.1.0/PKG-INFO` & `binharness-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: binharness
-Version: 0.1.0
+Version: 0.1.1
 Requires-Dist: black >=23.3.0 ; extra == 'dev'
 Requires-Dist: coverage[toml] >=7.2.3 ; extra == 'dev'
 Requires-Dist: docker >=7.0.0 ; extra == 'dev'
 Requires-Dist: mock-ssh-server >=0.9.1 ; extra == 'dev'
 Requires-Dist: mypy >=1.2.0 ; extra == 'dev'
 Requires-Dist: paramiko >=3.4.0 ; extra == 'dev'
 Requires-Dist: pre-commit >=3.2.2 ; extra == 'dev'
```


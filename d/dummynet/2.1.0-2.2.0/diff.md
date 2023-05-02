# Comparing `tmp/dummynet-2.1.0-py2.py3-none-any.whl.zip` & `tmp/dummynet-2.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11958 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      421 b- defN 23-Jan-10 14:33 dummynet/__init__.py
--rw-rw-r--  2.0 unx     9610 b- defN 23-Jan-11 09:36 dummynet/dummy_net.py
--rw-rw-r--  2.0 unx     1869 b- defN 23-Jan-10 14:33 dummynet/errors.py
--rw-rw-r--  2.0 unx     2746 b- defN 23-Jan-11 09:36 dummynet/host_shell.py
--rw-rw-r--  2.0 unx      772 b- defN 22-Dec-22 13:38 dummynet/namespace_shell.py
--rw-rw-r--  2.0 unx      508 b- defN 23-Jan-10 14:33 dummynet/process.py
--rw-rw-r--  2.0 unx     9450 b- defN 23-Jan-10 14:33 dummynet/process_monitor.py
--rw-rw-r--  2.0 unx     4435 b- defN 23-Jan-10 14:33 dummynet/run_info.py
--rw-rw-r--  2.0 unx     1505 b- defN 23-Jan-11 09:41 dummynet-2.1.0.dist-info/LICENSE.rst
--rw-rw-r--  2.0 unx     1948 b- defN 23-Jan-11 09:41 dummynet-2.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jan-11 09:41 dummynet-2.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jan-11 09:41 dummynet-2.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1022 b- defN 23-Jan-11 09:41 dummynet-2.1.0.dist-info/RECORD
-13 files, 34405 bytes uncompressed, 10264 bytes compressed:  70.2%
+Zip file size: 12089 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      421 b- defN 23-May-02 07:21 dummynet/__init__.py
+-rw-rw-r--  2.0 unx     9719 b- defN 23-May-02 08:15 dummynet/dummy_net.py
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-02 08:15 dummynet/errors.py
+-rw-rw-r--  2.0 unx     3071 b- defN 23-May-02 08:15 dummynet/host_shell.py
+-rw-rw-r--  2.0 unx      772 b- defN 22-Dec-25 13:20 dummynet/namespace_shell.py
+-rw-rw-r--  2.0 unx      508 b- defN 23-May-02 07:21 dummynet/process.py
+-rw-rw-r--  2.0 unx     9586 b- defN 23-May-02 08:15 dummynet/process_monitor.py
+-rw-rw-r--  2.0 unx     4610 b- defN 23-May-02 08:15 dummynet/run_info.py
+-rw-rw-r--  2.0 unx     1505 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/LICENSE.rst
+-rw-rw-r--  2.0 unx     1948 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1022 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/RECORD
+13 files, 35028 bytes uncompressed, 10395 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: dummynet/process_monitor.py
 Comment: 
 
 Filename: dummynet/run_info.py
 Comment: 
 
-Filename: dummynet-2.1.0.dist-info/LICENSE.rst
+Filename: dummynet-2.2.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: dummynet-2.1.0.dist-info/METADATA
+Filename: dummynet-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dummynet-2.1.0.dist-info/WHEEL
+Filename: dummynet-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dummynet-2.1.0.dist-info/top_level.txt
+Filename: dummynet-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dummynet-2.1.0.dist-info/RECORD
+Filename: dummynet-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dummynet/dummy_net.py

```diff
@@ -76,16 +76,15 @@
             result = parser.match(line)
 
             if result == None:
                 continue
 
             names.append(result.group("name"))
 
-        names.sort()
-        return names
+        return sorted(names)
 
     def link_delete(self, interface):
         """Deletes a specific network interface."""
 
         self.shell.run(cmd=f"ip link delete {interface}", cwd=None)
 
     def addr_add(self, ip, interface):
@@ -214,32 +213,34 @@
         names = []
 
         for line in result.stdout.splitlines():
             # The name is the first word followed by a space
             name = line.split(" ")[0]
             names.append(name)
 
-        names.sort()
-
-        return names
+        return sorted(names)
 
     def netns_process_list(self, name):
         """Returns a list of all processes in a network namespace"""
         result = self.shell.run(cmd=f"ip netns pids {name}", cwd=None)
         return result.stdout.splitlines()
 
     def netns_kill_process(self, name, pid):
         """Kills a process in a network namespace"""
         self.shell.run(cmd=f"ip netns exec {name} kill -9 {pid}", cwd=None)
 
     def netns_kill_all(self, name):
         """Kills all processes running in a network namespace"""
 
         for process in self.netns_process_list(name):
-            self.netns_kill_process(name, process)
+
+            try:
+                self.netns_kill_process(name, process)
+            except Exception:
+                self.shell.log.debug(f"Failed to kill process {process} in {name}")
 
     def netns_delete(self, name):
         """Deletes a specific network namespace.
         Note that before deleting a network namespace all processes in that
         namespace should be killed. Using e.g.::
 
             process_list = net.netns_get_process_list(ns_name).splitlines()
```

## dummynet/errors.py

```diff
@@ -58,12 +58,8 @@
 
 class ProcessExitError(DummyNetError):
     """Exception for when the process monitor is started with an already terminated process
     process
     """
 
     def __init__(self, process):
-        super().__init__(
-            f"Process {process.info.cmd} in {process.info.cwd} exited "
-            f"with {process.popen.returncode} before process monitor "
-            "was started."
-        )
+        super().__init__(f"Process exited before process monitor: {process.info} ")
```

## dummynet/host_shell.py

```diff
@@ -1,8 +1,10 @@
 import subprocess
+import sys
+import os
 
 from . import run_info
 from . import errors
 
 
 class HostShell(object):
     """A shell object for running commands"""
@@ -16,89 +18,100 @@
                                 to track running processes and to stop them when the test is
                                 finished.
         """
         self.log = log
         self.sudo = sudo
         self.process_monitor = process_monitor
 
-    def run(self, cmd: str, cwd=None):
+    def run(self, cmd: str, cwd=None, env=None):
         """Run a synchronous command (blocking).
 
         :param cmd: The command to run
         :param cwd: The current working directory i.e. where the command will
                     run
+        :param env: The environment variables to set
         """
 
         if self.sudo:
             cmd = "sudo " + cmd
 
+        if env is None:
+            env = os.environ.copy()
+
         self.log.debug(cmd)
 
         # Launch the command
         process = subprocess.Popen(
             cmd,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
+            env=env,
             shell=True,
             # Get stdout and stderr as text
             text=True,
         )
 
         # Here we wait for the process to exit
         # Warning: this can fail with large numbers of fds!
         stdout, stderr = process.communicate()
         returncode = process.wait()
 
         info = run_info.RunInfo(
             cmd=cmd,
             cwd=cwd,
+            pid=process.pid,
             stdout=stdout,
             stderr=stderr,
             returncode=returncode,
             is_async=False,
             is_daemon=False,
         )
 
         if info.returncode != 0:
             raise errors.RunInfoError(info=info)
 
         return info
 
-    def run_async(self, cmd: str, daemon=False, cwd=None):
+    def run_async(self, cmd: str, daemon=False, cwd=None, env=None):
         """Run an asynchronous command (non-blocking).
 
         :param cmd: The command to run
         :param cwd: The current working directory i.e. where the command will
                     run
         """
         if self.sudo:
             cmd = "sudo " + cmd
 
+        if env is None:
+            env = os.environ.copy()
+
         self.log.debug(cmd)
 
         # Launch the command
         popen = subprocess.Popen(
             cmd,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
+            env=env,
             shell=True,
             # Get stdout and stderr as text
             text=True,
         )
 
         info = run_info.RunInfo(
             cmd=cmd,
             cwd=cwd,
+            pid=popen.pid,
             stdout="",
             stderr="",
             returncode=None,
             is_async=True,
             is_daemon=daemon,
         )
 
-        self.process_monitor.add_process(popen, info)
+        self.process_monitor.add_process(popen=popen, info=info)
 
         return info
```

## dummynet/process_monitor.py

```diff
@@ -24,45 +24,41 @@
     class Poller:
         def __init__(self, log):
             self.poller = select.poll()
             self.fds = {}
             self.log = log
 
         def add_fd(self, fd, callback):
-
             # Note that flags POLLHUP and POLLERR can be returned at any time
             # (even if were not asked for). So we don't need to explicitly
             # register for them.
             self.poller.register(fd, select.POLLIN)
 
             self.fds[fd] = callback
 
             self.log.debug(f"Poller: register process fd {fd}")
 
         def del_fd(self, fd):
-
             self.poller.unregister(fd)
             del self.fds[fd]
 
             self.log.debug(f"Poller: unregister process fd {fd}")
 
         def read_fd(self, fd):
-
             data = os.read(fd, 4096)
 
             if not data:
                 return
 
             self.log.debug(f"Poller: read {len(data)} bytes from fd {fd}")
 
             # Call the callback
             self.fds[fd](data.decode("utf-8"))
 
         def poll(self, timeout):
-
             fds = self.poller.poll(timeout)
 
             self.log.debug(f"Poller: got {len(fds)} events")
 
             # First if we have any events, we need to read from the
             # file descriptors
             for fd, event in fds:
@@ -101,19 +97,17 @@
         def __init__(self):
             self.running = []
 
         def add_process(self, process):
             self.running.append(process)
 
         def validate(self):
-
             try:
                 self._validate()
             except Exception:
-
                 # Kill all processes
                 for process in self.running:
                     process.popen.kill()
                 raise
 
         def _validate(self):
             if not self.running:
@@ -139,20 +133,22 @@
 
             # The poller is used to wait for processes to terminate
             self.poller = ProcessMonitor.Poller(log=log)
 
             self.log = log
 
         def add_process(self, process):
-
             # Make sure the process is running
             process.popen.poll()
 
             # The returncode should be None if the process is running
             if not process.popen.returncode is None:
+                process.info.returncode = process.popen.returncode
+                process.info.stdout, process.info.stderr = process.popen.communicate()
+
                 raise errors.ProcessExitError(process)
 
             self.running.append(process)
 
             def stdout_callback(data):
                 process.info.stdout += data
 
@@ -173,80 +169,71 @@
 
             self.poller.add_fd(
                 process.popen.stderr.fileno(),
                 stderr_callback,
             )
 
         def poll(self, timeout):
-
             # Poll for events
             self.poller.poll(timeout)
 
             # Check if any process has died
             for process in self.running:
-
                 process.popen.poll()
 
                 if process.popen.returncode is not None:
                     self._died(process=process)
 
         def _died(self, process):
-
             self.died.append(process)
             self.running.remove(process)
 
             # Set the return code
             process.info.returncode = process.popen.returncode
 
             # Check if we had a normal exit
             if process.popen.returncode:
-
                 # The process had a non-zero return code
                 raise errors.RunInfoError(info=process.info)
 
             if process.info.is_daemon:
-
                 # The process was a daemon - these should not exit
                 # until after the test is over
                 raise errors.DaemonExitError(process)
 
         def stop(self):
             """Stop all running processes."""
 
             self.log.debug("Stopping all processes")
 
             for process in self.running:
-
                 self.poller.del_fd(process.popen.stdout.fileno())
                 self.poller.del_fd(process.popen.stderr.fileno())
 
                 process.popen.kill()
 
         def run(self, timeout):
-
             try:
                 # Poll for events
                 self.poll(timeout=timeout)
                 return self.keep_running()
 
             except Exception:
-
                 # Stop all processes
                 self.stop()
                 raise
 
         def keep_running(self):
             """Check if the test is over.
 
             The ProcessMonitor should continue running for as long as there
             are non daemon processes active.
             """
 
             for process in self.running:
-
                 if not process.info.is_daemon:
                     # A process which is not a daemon is still running
                     return True
 
             # Only daemon processes running
             return False
 
@@ -304,27 +291,24 @@
                     pass
         """
 
         try:
             return self._run(timeout=timeout)
 
         except Exception as e:
-
             self.state = ProcessMonitor.Stopped()
             raise e
 
     def _run(self, timeout):
-
         if isinstance(self.state, ProcessMonitor.Stopped):
             # It ok to be in the stopped state here. Likely it is the user
             # who has called stop() in the while run() loop.
             return False
 
         if isinstance(self.state, ProcessMonitor.Initializing):
-
             # We are waiting to run
             self.state.validate()
 
             # Switch to the running state
             running = ProcessMonitor.Running(log=self.log)
 
             for process in self.state.running:
```

## dummynet/run_info.py

```diff
@@ -4,14 +4,15 @@
 
 
 class RunInfo:
     """Stores the results from running a command
 
     :ivar cmd: see :meth:`RunInfo.__init__`
     :ivar cwd: see :meth:`RunInfo.__init__`
+    :ivar pid: see :meth:`RunInfo.__init__`
     :ivar stdout: see :meth:`RunInfo.__init__`
     :ivar stderr: see :meth:`RunInfo.__init__`
     :ivar returncode: see :meth:`RunInfo.__init__`
     :ivar is_async: see :meth:`RunInfo.__init__`
     :ivar is_daemon: see :meth:`RunInfo.__init__`
     :ivar stdout_callback: The callback to be called when the standard output
                             stream is received  (default: None). The callback
@@ -19,28 +20,30 @@
                             received.
     :ivar stderr_callback: The callback to be called when the standard error
                             stream is received  (default: None). The callback
                             should accept a single argument which is the data
                             received.
     """
 
-    def __init__(self, cmd, cwd, stdout, stderr, returncode, is_async, is_daemon):
+    def __init__(self, cmd, cwd, pid, stdout, stderr, returncode, is_async, is_daemon):
         """Create a new object
 
         :param cmd: The command that was executed
         :param cwd: Current working directory i.e. path where the command was executed
+        :param pid: The process ID of the command
         :param stdout: The standard output stream generated by the command
         :param stderr: The standard error stream generated by the command
         :param returncode: The return code set after invoking the command
         :param is_async: Whether the command was run asynchronously
         :param is_daemon: Whether the command was run as a daemon
         """
 
         self.cmd = cmd
         self.cwd = cwd
+        self.pid = pid
         self.stdout = stdout
         self.stderr = stderr
         self.returncode = returncode
         self.is_async = is_async
         self.is_daemon = is_daemon
         self.stdout_callback = None
         self.stderr_callback = None
@@ -96,23 +99,25 @@
 
     def __str__(self):
         """Print the RunInfo object as a string"""
         run_string = (
             "RunInfo\n"
             "command: {command}\n"
             "cwd: {cwd}\n"
+            "pid: {pid}\n"
             "returncode: {returncode}\n"
             "stdout: \n{stdout}"
             "stderr: \n{stderr}"
             "is_async: {is_async}\n"
             "is_daemon: {is_daemon}\n"
         )
 
         return run_string.format(
             command=self.cmd,
             cwd=self.cwd,
+            pid=self.pid,
             returncode=self.returncode,
             stdout=self.stdout,
             stderr=self.stderr,
             is_async=self.is_async,
             is_daemon=self.is_daemon,
         )
```

## Comparing `dummynet-2.1.0.dist-info/LICENSE.rst` & `dummynet-2.2.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `dummynet-2.1.0.dist-info/METADATA` & `dummynet-2.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummynet
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool for creating dummy networks using network namespaces.
 Home-page: https://github.com/steinwurf/dummynet
 Author: Steinwurf ApS
 Author-email: contact@steinwurf.com
 License: BSD 3-clause "New" or "Revised" License
 Keywords: dummynet,network,namespace
 Platform: UNKNOWN
```

## Comparing `dummynet-2.1.0.dist-info/RECORD` & `dummynet-2.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dummynet/__init__.py,sha256=fACqGaMLRCIrNKoPzeiA9h-0Iu5qDjuT_UpaRQ8ewG0,421
-dummynet/dummy_net.py,sha256=HMV3IOBW9gxHLpyPTE5h2XXyvX7xjRLACaOgZKsHaoE,9610
-dummynet/errors.py,sha256=eL649Y25zt3JQFboFlMF38B5EPvhydQb1kONbgopuY8,1869
-dummynet/host_shell.py,sha256=R-MT1kgGSWB803cPVk9OKXsgATroI8IpiERFWkOac-w,2746
+dummynet/dummy_net.py,sha256=BfDXzxL4UKeMzIvO4VwjIsB2udjqksFnGE8Kchs8aQQ,9719
+dummynet/errors.py,sha256=6r4-qB9QQtjBkz-t6_U9I9YEeqYElCKyJz_CWIsFdZ8,1747
+dummynet/host_shell.py,sha256=9rT6JkGwr4cysC3-uo39DGXFQ0FiRW6EjZQdEIpuf4c,3071
 dummynet/namespace_shell.py,sha256=89gHWWB67eXHJlSPQAf27y4rQO2ETs9B_Qy3fV4nPPk,772
 dummynet/process.py,sha256=_ip-Q46ho2BRtELcO8P-_1x0o_fCjfy3Yj56mPVLwlk,508
-dummynet/process_monitor.py,sha256=W7cjsk7Q-eburpmDtoAMKUqfwE22YcMp5oa7KPorRVQ,9450
-dummynet/run_info.py,sha256=PfY0aEw-Td7M1lUeMCTrR-36a4O7T8QjobfDa0Q7dEo,4435
-dummynet-2.1.0.dist-info/LICENSE.rst,sha256=lnhVy333OpPgt8lKvpJs9jdfAOTpzAhlk0Z2e4V2BDs,1505
-dummynet-2.1.0.dist-info/METADATA,sha256=VAT5camZRRDUnQjSNrK_D4nVsUqYiMSbZqVXcMbl4P4,1948
-dummynet-2.1.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-dummynet-2.1.0.dist-info/top_level.txt,sha256=beQt5cynnx7cpYC2J9i11U2IBQdl-bVPaINnhozkRoM,9
-dummynet-2.1.0.dist-info/RECORD,,
+dummynet/process_monitor.py,sha256=7x5Pl7Ly52P0mzfjXBSI_Vc4xnsLorp8kVt8Gj0BBrE,9586
+dummynet/run_info.py,sha256=Xug4AVXC3uee7pCB8TBw7RLP07VroOccgCKegQV7gR4,4610
+dummynet-2.2.0.dist-info/LICENSE.rst,sha256=lnhVy333OpPgt8lKvpJs9jdfAOTpzAhlk0Z2e4V2BDs,1505
+dummynet-2.2.0.dist-info/METADATA,sha256=KtkEcpz3bRg5swwiidXgl0CLB2hbDHlMl98pnG0_PrE,1948
+dummynet-2.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+dummynet-2.2.0.dist-info/top_level.txt,sha256=beQt5cynnx7cpYC2J9i11U2IBQdl-bVPaINnhozkRoM,9
+dummynet-2.2.0.dist-info/RECORD,,
```


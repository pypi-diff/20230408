# Comparing `tmp/pyalpa-0.3.2.tar.gz` & `tmp/pyalpa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.3.2.tar", max compression
+gzip compressed data, was "pyalpa-0.4.0.tar", max compression
```

## Comparing `pyalpa-0.3.2.tar` & `pyalpa-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-03-29 19:22:21.030065 pyalpa-0.3.2/LICENSE
--rw-r--r--   0        0        0     1416 2023-03-29 19:22:21.030065 pyalpa-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/cli/__init__.py
--rw-r--r--   0        0        0      709 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/cli/base.py
--rw-r--r--   0        0        0     5327 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/cli/local_repo.py
--rw-r--r--   0        0        0        0 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/config/__init__.py
--rw-r--r--   0        0        0      874 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/config/local_config.py
--rw-r--r--   0        0        0     1878 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/config/packit.py
--rw-r--r--   0        0        0      667 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/constants.py
--rw-r--r--   0        0        0      111 2023-03-29 19:22:21.030065 pyalpa-0.3.2/alpa/exceptions.py
--rw-r--r--   0        0        0     2869 2023-03-29 19:22:21.034065 pyalpa-0.3.2/alpa/gh.py
--rw-r--r--   0        0        0      971 2023-03-29 19:22:21.034065 pyalpa-0.3.2/alpa/messages.py
--rw-r--r--   0        0        0     8042 2023-03-29 19:22:21.034065 pyalpa-0.3.2/alpa/repository.py
--rw-r--r--   0        0        0     3239 2023-03-29 19:22:21.034065 pyalpa-0.3.2/alpa/upstream_integration.py
--rw-r--r--   0        0        0      740 2023-03-29 19:22:21.034065 pyalpa-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 pyalpa-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-07 22:30:15.199819 pyalpa-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-07 22:30:15.199819 pyalpa-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1230 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6330 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0        0 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/config/local_config.py
+-rw-r--r--   0        0        0     2243 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/config/packit.py
+-rw-r--r--   0        0        0      813 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/constants.py
+-rw-r--r--   0        0        0      111 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     3579 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/gh.py
+-rw-r--r--   0        0        0     1447 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/messages.py
+-rw-r--r--   0        0        0    12804 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/repository.py
+-rw-r--r--   0        0        0     3858 2023-04-07 22:30:15.199819 pyalpa-0.4.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      762 2023-04-07 22:30:15.199819 pyalpa-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 pyalpa-0.4.0/PKG-INFO
```

### Comparing `pyalpa-0.3.2/LICENSE` & `pyalpa-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.3.2/alpa/cli/alpa_repo.py` & `pyalpa-0.4.0/alpa/cli/alpa_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     """Delete existing package"""
     raise NotImplementedError("Not implemented yet (1.0 goal)")
 
 
 @click.command("request-package")
 @pkg_name
 def request_package(name: str) -> None:
-    """Request new branch for new package in upstream"""
+    """Request new branch for new package in Alpa repo"""
     raise NotImplementedError("Not implemented yet (1.0 goal)")
```

### Comparing `pyalpa-0.3.2/alpa/cli/base.py` & `pyalpa-0.4.0/alpa/cli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from alpa.cli.alpa_repo import create, delete, request_package
 from alpa.cli.local_repo import (
     show_history,
     switch,
     commit,
     pull,
     push,
-    list,
+    list_,
     genspec,
     add,
     get_pkg_archive,
     mockbuild,
     create_packit_config,
 )
 from alpa.repository import AlpaRepo
@@ -25,29 +25,30 @@
 
 
 # commands that don't require git repo at all
 
 
 @entry_point.command("clone")
 @click.argument("url", type=str)
-def clone(url: str) -> None:
+@click.option("--fork", is_flag=True, default=False)
+def clone(url: str, fork: bool) -> None:
     """Clone and prepare Alpa repository"""
-    AlpaRepo.clone(url)
+    AlpaRepo.clone(url, fork)
 
 
 entry_point.add_command(create)
 entry_point.add_command(delete)
 entry_point.add_command(request_package)
 
 entry_point.add_command(show_history)
 entry_point.add_command(switch)
 entry_point.add_command(commit)
 entry_point.add_command(pull)
 entry_point.add_command(push)
-entry_point.add_command(list)
+entry_point.add_command(list_)
 entry_point.add_command(genspec)
 entry_point.add_command(add)
 entry_point.add_command(get_pkg_archive)
 entry_point.add_command(mockbuild)
 entry_point.add_command(create_packit_config)
```

### Comparing `pyalpa-0.3.2/alpa/cli/local_repo.py` & `pyalpa-0.4.0/alpa/cli/local_repo.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 
 from os import getcwd
 from pathlib import Path
 from typing import List
 
 import click
-from alpa_conf.metadata import Metadata
+from alpa_conf import MetadataConfig
 from click import ClickException, Choice
+from specfile import Specfile
 
 from alpa.config.packit import PackitConfig
 from alpa.repository import LocalRepo, AlpaRepo
 from alpa.upstream_integration import UpstreamIntegration
 
 pkg_name = click.argument("name", type=str)
 
@@ -30,15 +31,15 @@
 def show_history(oneline: bool) -> None:
     """Show git history of current package"""
     params = []
     if oneline:
         params.append("--oneline")
 
     local_repo = LocalRepo(Path(getcwd()))
-    click.echo(local_repo.get_history_of_branch(local_repo.package, params))
+    click.echo(local_repo.get_history_of_branch(local_repo.branch, params))
 
 
 @click.command("switch")
 @pkg_name
 def switch(name: str) -> None:
     """Switch to specified package"""
     LocalRepo(Path(getcwd())).switch_to_package(name)
@@ -48,20 +49,21 @@
 @click.option(
     "-m",
     "--message",
     type=str,
     default="",
     help="Your commit message not longer than 80 characters.",
 )
-def commit(message: str) -> None:
+@click.option("-n", "--no-verify", is_flag=True, help="Do not run pre-commit")
+def commit(message: str, no_verify: bool) -> None:
     """Commit your changes in your package's repository"""
     if len(message) > 80:
         raise ClickException("Message longer than 80 characters")
 
-    LocalRepo(Path(getcwd())).commit(message)
+    LocalRepo(Path(getcwd())).commit(message, not no_verify)
 
 
 @click.command("add")
 @click.argument("files", type=str, nargs=-1, required=True)
 def add(files: List[str]) -> None:
     """Add files to git history. Basically calls `git add <input>`"""
     LocalRepo(Path(getcwd())).add(files)
@@ -73,54 +75,59 @@
     "--pull-request",
     is_flag=True,
     show_default=True,
     default=False,
     help="This will create pull request on GitHub for you.",
 )
 def push(pull_request: bool) -> None:
-    """Pushes your commited changes to the upstream so you can make PR"""
+    """Pushes your commited changes to the Alpa repo so you can make PR"""
     repo_path = Path(getcwd())
     local_repo = LocalRepo(repo_path)
 
     packit_conf = PackitConfig(local_repo.package)
     if not packit_conf.packit_config_file_exists():
         packit_conf.create_packit_config()
         local_repo.git_cmd.add(".packit.yaml")
         local_repo.git_cmd.commit(
             '-m "alpa: automatically add .packit.yaml config to the package"'
         )
 
     local_repo.push(local_repo.branch)
 
     if not pull_request:
+        local_repo.git_cmd.branch("-d", local_repo.feat_branch)
         return
 
     alpa = AlpaRepo(repo_path)
     pr = alpa.gh_repo.create_pr(
         title=f"[alpa-cli] Create update of package {local_repo.package}",
         body=(
             "This PR was created automatically via alpa-cli for "
             f"user {alpa.gh_api.gh_user}"
         ),
-        source_branch=f"{alpa.gh_api.gh_user}:{local_repo.feat_branch}",
+        source_branch=f"{local_repo.feat_branch}",
         target_branch=local_repo.package,
     )
     click.echo(f"PR#{pr.number} created. URL: {pr.html_url}")
 
+    # go from feat branch to package branch
+    local_repo.git_cmd.switch(local_repo.package)
+    local_repo.git_cmd.branch("-D", local_repo.feat_branch)
+
 
 @click.command("pull")
 def pull() -> None:
-    """Pull last recent changes of package you are on from upstream"""
+    """Pull last recent changes of package you are on from Alpa repo"""
     local_repo = LocalRepo(Path(getcwd()))
     local_repo.pull(local_repo.branch)
 
 
 @click.command("list")
 @click.option("-p", "--pattern", type=str, default="", help="Optional pattern to match")
-def list(pattern: str) -> None:
+def list_(pattern: str) -> None:
     """List all packages or packages matching regex"""
     for pkg in LocalRepo(Path(getcwd())).get_packages(pattern):
         click.echo(pkg)
 
 
 @click.command("genspec")
 @click.option(
@@ -155,36 +162,55 @@
     """Creates packit config based on metadata.yaml file in package"""
     if not LocalRepo(Path(getcwd())).create_packit_config(override):
         raise ClickException(
             "Packit file already exists. To override it use --override flag."
         )
 
 
+def _get_chroots_to_build(meta: MetadataConfig, distros: list[str]) -> list[str]:
+    chroots = []
+    for arch in meta.arch:
+        for distro in distros:
+            chroots.append(f"{distro}-{arch}")
+    return chroots
+
+
 @click.command("mockbuild")
 @click.option(
     "--chroot",
     type=str,
     default="",
     help="Override chroots specified in metadata.yaml by one specific chroot",
 )
 def mockbuild(chroot: str) -> None:
     """
     Uses mock tool to build package. WARNING: works only on rpm-based systems.
 
     Builds for all chroots specified in metadata.yaml. Can be overriden by --chroot
      option which does build against one specified chroot.
     """
-    if chroot:
-        chroots = [chroot]
-    else:
-        chroots = list(Metadata().targets)
-
+    meta = MetadataConfig.get_config()
+    distros = [chroot] if chroot else list(meta.targets)
+    chroots = _get_chroots_to_build(meta, distros)
     UpstreamIntegration(Path(getcwd())).mockbuild(chroots)
 
 
 @click.command("get-pkg-archive")
 def get_pkg_archive() -> None:
     """Gets archive from package config"""
-    meta = Metadata()
+    specfile_path = None
+    cwd = Path(getcwd())
+    for file in cwd.iterdir():
+        if str(file).endswith(".spec"):
+            specfile_path = file
+
+    if specfile_path is None:
+        raise ClickException(f"No specfile found in {cwd}")
+
+    specfile = Specfile(specfile_path)
+    with specfile.sources() as sources:
+        source0 = min(sources, key=lambda src: src.number)
+
     UpstreamIntegration.download_upstream_source(
-        meta.upstream_source_url, f"{meta.pkg_name}-{meta.upstream_ref}"
+        source0.expanded_location,
+        f"{specfile.expanded_name}-{specfile.expanded_version}",
     )
```

### Comparing `pyalpa-0.3.2/alpa/config/local_config.py` & `pyalpa-0.4.0/alpa/config/local_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-# TODO: this is just skeleton for configuration
-
 from os.path import isfile
 from pathlib import Path
 from typing import Optional
 
 from yaml import safe_load
 
 from alpa.constants import CONFIG_FILE_LOCATIONS
 
 
 class Config:
-    def __init__(self, api_token: str) -> None:
-        pass
+    def __init__(self, gh_api_token: str) -> None:
+        self.gh_api_token = gh_api_token
 
     @staticmethod
     def _get_config_file_path() -> Optional[Path]:
         for location in CONFIG_FILE_LOCATIONS:
             expanded_path = Path(location).expanduser()
             if isfile(str(expanded_path)):
                 return expanded_path
 
         return None
 
     @classmethod
-    def get_config(cls) -> Optional["Config"]:
+    def get_config(cls, repo_name: str) -> Optional["Config"]:
         cfg_file_path = cls._get_config_file_path()
         if cfg_file_path is None:
             return None
 
         with open(cfg_file_path) as alpa_cfg_file:
             config_dict = safe_load(alpa_cfg_file)
 
-        return Config(**config_dict)
+        for item in config_dict["api_keys"]:
+            if item["repo"]["name"] == repo_name:
+                return Config(gh_api_token=item["repo"]["key"])
+
+        return None
```

### Comparing `pyalpa-0.3.2/alpa/config/packit.py` & `pyalpa-0.4.0/alpa/config/packit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 from os import getcwd
 from pathlib import Path
 
 from yaml import dump
 
-from alpa_conf.constants import PACKIT_CONFIG_NAMES
-from alpa_conf.metadata import Metadata
+from alpa_conf import AlpaRepoConfig, MetadataConfig
+
+from alpa.constants import PACKIT_CONFIG_NAMES
 
 
 class PackitConfig:
     def __init__(self, package_name: str) -> None:
         self.package_name = package_name
         self.working_dir = Path(getcwd())
-        self.metadata = Metadata()
+        self.metadata = MetadataConfig.get_config(self.working_dir)
+        self.alpa_repo_config = AlpaRepoConfig.get_config()
 
     def get_packit_config(self) -> dict:
         return {
             "specfile_path": f"{self.package_name}.spec",
             "srpm_build_deps": ["pip"],
             "actions": {
                 "create-archive": [
-                    "pip install pyalpa alpa-conf",
+                    "pip install pyalpa",
                     'bash -c "alpa get-pkg-archive"',
                     f'bash -c "ls -1 ./{self.package_name}-*.tar.gz"',
                 ],
             },
             "jobs": [
                 {
                     "job": "copr_build",
                     "trigger": "pull_request",
                     "targets": list(self.metadata.targets),
+                    "owner": self.alpa_repo_config.copr_owner,
+                    "project": f"{self.alpa_repo_config.copr_repo}-pull-requests",
                 },
                 {
                     "job": "copr_build",
                     "trigger": "commit",
                     "branch": self.package_name,
                     "targets": list(self.metadata.targets),
+                    "owner": self.alpa_repo_config.copr_owner,
+                    "project": self.alpa_repo_config.copr_repo,
                 },
             ],
         }
 
     def packit_config_file_exists(self) -> bool:
         for packit_config_name in PACKIT_CONFIG_NAMES:
             files_in_dir = [
```

### Comparing `pyalpa-0.3.2/alpa/constants.py` & `pyalpa-0.4.0/alpa/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,17 +9,26 @@
 GH_API_TOKEN_NAME = "ALPA_GH_API_TOKEN"
 GH_WRITE_ACCESS = ["admin", "write"]
 
 ALPA_ISSUE_REPO_NAME = "issue-repo"
 ALPA_FEAT_BRANCH_PREFIX = "__feat_"
 ALPA_FEAT_BRANCH = ALPA_FEAT_BRANCH_PREFIX + "{pkgname}"
 
-GLOBAL_CFG_FILE = "/etc/vem.cfg"
-USER_CFG_FILE = "~/.config/vem.cfg"
+GLOBAL_CFG_FILE = "/etc/alpa.yaml"
+USER_CFG_FILE = "~/.config/alpa.yaml"
 # order is important! user cfg overrides global cfg
 CONFIG_FILE_LOCATIONS = [USER_CFG_FILE, GLOBAL_CFG_FILE]
 
+PACKIT_CONFIG_NAMES = [
+    ".packit.yaml",
+    ".packit.yml",
+    ".packit.json",
+    "packit.yaml",
+    "packit.yml",
+    "packit.json",
+]
+
 
 class PackageRequest(str, Enum):
     TITLE = "[alpa] New request for package {package_name}"
     BODY = "@{user} requested {package_name} for repo {repo_name}"
     LABEL = "request"
```

### Comparing `pyalpa-0.3.2/alpa/gh.py` & `pyalpa-0.4.0/alpa/gh.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 
 from os import getenv
 from typing import Optional
 
 import click
 from click import UsageError
-from github import Github, Issue, PullRequest
+from github import Github, Issue, PullRequest, UnknownObjectException
 
+from alpa.config.local_config import Config
 from alpa.constants import GH_API_TOKEN_NAME, GH_WRITE_ACCESS
 from alpa.messages import NO_GH_API_KEY_FOUND, RETURNING_CLONE_URL_MSG
 
 
 class GithubRepo:
     def __init__(self, api: Github, namespace: str, repo_name: str) -> None:
         self.namespace = namespace
@@ -38,30 +39,35 @@
     def upstream_clone_url(self) -> Optional[str]:
         upstream = self.get_upstream()
         if upstream is None:
             return None
 
         return upstream.clone_url
 
+    @property
     def is_fork(self) -> bool:
         return self._repo.fork
 
+    @property
+    def api_user(self) -> str:
+        return self._api.get_user().login
+
     def has_write_access(self, user: str) -> bool:
         for collaborator in self._repo.get_collaborators():
             if collaborator.login != user:
                 continue
 
             return (
                 self._repo.get_collaborator_permission(collaborator) in GH_WRITE_ACCESS
             )
 
         return False
 
     def get_upstream(self) -> Optional["GithubRepo"]:
-        if not self.is_fork():
+        if not self.is_fork:
             return None
 
         namespace, repo_name = self._repo.source.full_name.split("/")
         return GithubRepo(self._api, namespace, repo_name)
 
     def get_root_repo(self) -> "GithubRepo":
         root_repo = self.get_upstream()
@@ -76,26 +82,39 @@
     def create_pr(
         self, title: str, body: str, source_branch: str, target_branch: str = "main"
     ) -> PullRequest:
         return self.get_root_repo()._repo.create_pull(
             title, body, base=target_branch, head=source_branch
         )
 
+    def pr_exists(self, id: int) -> bool:
+        try:
+            self._repo.get_pull(id)
+            return True
+        except UnknownObjectException:
+            return False
+
 
 class GithubAPI:
-    def __init__(self) -> None:
-        self._gh_api = Github(self._get_access_token())
+    def __init__(self, repo_name: str) -> None:
+        self._gh_api = Github(self._get_access_token(repo_name))
 
     @property
     def gh_user(self) -> str:
         return self._gh_api.get_user().login
 
     @staticmethod
-    def _get_access_token() -> str:
-        access_token = getenv(GH_API_TOKEN_NAME)
-        if access_token is None:
+    def _get_access_token(repo_name: str) -> str:
+        access_token_env = getenv(GH_API_TOKEN_NAME)
+        if access_token_env is not None:
+            return access_token_env
+
+        # accessing config file here since it does not make sense to do it elsewhere,
+        # but in the future the config will be useful in many places
+        access_token_config = Config.get_config(repo_name)
+        if access_token_config is None:
             raise UsageError(NO_GH_API_KEY_FOUND.format(token=GH_API_TOKEN_NAME))
 
-        return access_token
+        return access_token_config.gh_api_token
 
     def get_repo(self, namespace: str, repo_name: str) -> GithubRepo:
         return GithubRepo(self._gh_api, namespace, repo_name)
```

### Comparing `pyalpa-0.3.2/alpa/messages.py` & `pyalpa-0.4.0/alpa/messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """
 File for really long messages.
 """
 
 
 NO_GH_API_KEY_FOUND = (
-    "No GitHub API key found. Please set the "
-    "{token} environment variable and pass "
-    "the GitHub API token to it. For more information please "
-    "see (link TODO)"
+    "No GitHub API key found. Please set the {token} environment variable and"
+    " pass the GitHub API token to it or set it in alpa.yaml config file. \n"
+    "For more information please see (link TODO)"
 )
 
+NO_PERMISSION_FOR_ALPA_REPO = (
+    "You don't have write permission to this repository. Please fork this Alpa "
+    "repository and work with your fork. Cloning a fork repo is done with "
+    "`--fork` flag. e.g. `alpa clone --fork my-fork-repo`"
+)
 CLONED_REPO_IS_NOT_FORK = (
-    "The url of GitHub repository isn't fork "
-    "(does not have upstream). Please provide repository which is "
-    "a forked form Alpa repository."
+    "You are trying to clone repository which is not a fork! Clone a fork "
+    "repository or do the clone command without `--fork` flag."
+)
+CLONED_REPO_IS_FORK = (
+    "The url of GitHub repository is a fork. Please provide repository which "
+    "is not a forked form Alpa repository or specify the clone command with "
+    "the `--fork` flag."
 )
 
 NO_WRITE_ACCESS_ERR = (
     "You don't have write access to this repository. If you "
     "want to create new package, please use `alpa request-package "
     "[PACKAGE NAME]` command instead."
 )
```

### Comparing `pyalpa-0.3.2/alpa/repository.py` & `pyalpa-0.4.0/alpa/repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Set of commands that helps with integration of Alpa
 repository.
 """
+import subprocess
 from os import getcwd, environ
 from pathlib import Path
 import re
 from subprocess import call
 from tempfile import NamedTemporaryFile
-from typing import List, Optional
+from typing import List, Optional, Iterable
 from urllib.parse import urlparse
 
 from click import UsageError, ClickException
 import click
 from git import Repo, Remote, GitCommandError
 
 from alpa.config.packit import PackitConfig
@@ -24,44 +25,68 @@
     PackageRequest,
 )
 from alpa.gh import GithubAPI, GithubRepo
 from alpa.messages import (
     CLONED_REPO_IS_NOT_FORK,
     NO_WRITE_ACCESS_ERR,
     NOT_IN_PREDEFINED_STATE,
+    CLONED_REPO_IS_FORK,
+    NO_PERMISSION_FOR_ALPA_REPO,
 )
 
 
 class LocalRepo:
     def __init__(self, repo_path: Path) -> None:
         self.repo_path = repo_path
         # TODO: this will differ in the future with repo_path
         self.repo_root_path = repo_path
         self.local_repo = Repo(str(self.repo_path))
         self.git_cmd = self.local_repo.git
 
         if not self._is_repo_in_predefined_state():
             raise ClickException(NOT_IN_PREDEFINED_STATE)
 
+        # do it after predefined state is checked since this depends on it
+        # (see comment in the _should_be_fork)
+        self.remote_name = UPSTREAM_NAME if self._should_be_fork() else ORIGIN_NAME
+
+        # lazy properties
+        self._namespace: Optional[str] = None
+        self._repo_name: Optional[str] = None
+
     @property
     def remote_associated_with_current_branch(self) -> str:
         return self.local_repo.active_branch.tracking_branch().remote_name
 
     @property
     def branch(self) -> str:
         return self.local_repo.active_branch.name
 
     @property
     def package(self) -> str:
         return self.branch.lstrip(ALPA_FEAT_BRANCH_PREFIX)
 
+    @staticmethod
+    def get_feat_branch_of_package(package: str) -> str:
+        return ALPA_FEAT_BRANCH.format(pkgname=package)
+
     @property
     def feat_branch(self) -> str:
         return ALPA_FEAT_BRANCH.format(pkgname=self.package)
 
+    @staticmethod
+    def _get_relevant_remote_refs(remote_refs: Iterable[str]) -> list[str]:
+        relevant_refs = []
+        for ref in remote_refs:
+            parsed_ref = ref.split("/")[-1]
+            if not parsed_ref.startswith(ALPA_FEAT_BRANCH_PREFIX):
+                relevant_refs.append(parsed_ref)
+
+        return relevant_refs
+
     def show_remote_branches(self, remote: str) -> List[str]:
         lines = [
             line.strip()
             for line in self.git_cmd.remote("--verbose", "show", remote).split("\n")
         ]
         # TODO: do a better job
         remote_branch_line = ["Remote branch:", "Remote branches:"]
@@ -90,36 +115,129 @@
         if end == -1:
             end = len(lines)
 
         lines_with_remote_branches = lines[start + 1 : end]
         return [line.split()[0] for line in lines_with_remote_branches]
 
     def get_packages(self, regex: str) -> List[str]:
-        # self.local_repo.remote(name=UPSTREAM_NAME).refs don't work on every case
+        # self.local_repo.remote(name=self.remote_name).refs don't work on every case
         refs_without_main = filter(
-            lambda ref: ref != "main", self.show_remote_branches(UPSTREAM_NAME)
+            lambda ref: ref != "main", self.show_remote_branches(self.remote_name)
         )
+        relevant_refs = self._get_relevant_remote_refs(refs_without_main)
+
         if regex == "":
-            return list(refs_without_main)
+            return list(relevant_refs)
 
         pattern = re.compile(regex)
-        return [ref for ref in refs_without_main if pattern.match(ref)]
+        return [ref for ref in relevant_refs if pattern.match(ref)]
 
     def _is_repo_in_predefined_state(self) -> bool:
         remotes_name_set = {remote.name for remote in self.local_repo.remotes}
-        return remotes_name_set == {ORIGIN_NAME, UPSTREAM_NAME}
+        return remotes_name_set == {ORIGIN_NAME, UPSTREAM_NAME} or remotes_name_set == {
+            ORIGIN_NAME
+        }
+
+    def _should_be_fork(self) -> bool:
+        remotes_name_set = {remote.name for remote in self.local_repo.remotes}
+        # if repo is prepared via alpa-cli, fork should have 2 remotes and non-fork 1
+        return len(remotes_name_set) > 1
+
+    @property
+    def untracked_files(self) -> list[str]:
+        return self.local_repo.untracked_files
+
+    def _get_dirty_files(self, staged: bool) -> list[str]:
+        result = []
+        status_output = self.git_cmd.status("--porcelain=1").split("\n")
+        for line in status_output:
+            file = line.split()[-1]
+            if line.startswith("MM"):
+                result.append(file)
+                continue
+
+            if not staged and line.startswith(" M"):
+                result.append(file)
+                continue
+
+            if staged and line.startswith("M "):
+                result.append(file)
+                continue
+
+        return result
+
+    @property
+    def modified_files(self) -> list[str]:
+        return self._get_dirty_files(False)
+
+    @property
+    def files_to_be_committed(self) -> list[str]:
+        return self._get_dirty_files(True)
+
+    @property
+    def namespace(self) -> str:
+        if self._namespace is not None:
+            return self._namespace
+
+        self._namespace = self.full_reponame().split("/")[0]
+        return self._namespace
+
+    @property
+    def repo_name(self) -> str:
+        if self._repo_name is not None:
+            return self._repo_name
+
+        self._repo_name = self.full_reponame().split("/")[1]
+        return self._repo_name
+
+    @staticmethod
+    def _format_files_to_status(files: list[str], msg: str) -> str:
+        if not files:
+            return ""
+
+        output = msg + "\n"
+        output += "\n".join(files)
+        return output + "\n"
+
+    def get_status_output(self) -> str:
+        output = self._format_files_to_status(
+            self.files_to_be_committed, "Files to commit:"
+        )
+        output += self._format_files_to_status(self.modified_files, "Modified files:")
+        output += self._format_files_to_status(self.untracked_files, "Untracked files:")
+        return output
+
+    def branch_exists(self, branch: str) -> bool:
+        for ref in self.local_repo.references:
+            if ref.name == branch:
+                return True
+
+        return False
 
     def switch_to_package(self, package: str) -> None:
+        if self.local_repo.is_dirty():
+            click.echo(
+                "Repo is dirty, please commit your changes before switching to"
+                f" another package.\n {self.get_status_output()}"
+            )
+            return None
+
+        feat_branch = self.get_feat_branch_of_package(package)
+        branch_to_switch = feat_branch if self.branch_exists(feat_branch) else package
         try:
-            click.echo(self.git_cmd.switch(package))
+            click.echo(
+                self.git_cmd.switch(branch_to_switch).replace("branch", "package")
+            )
         except GitCommandError:
             # switching to the package for the first time
             click.echo(f"Switching to the package {package} for the first time")
-            click.echo(self.git_cmd.fetch(UPSTREAM_NAME, package))
-            click.echo(self.git_cmd.switch(package))
+            click.echo(self.git_cmd.fetch(self.remote_name, branch_to_switch))
+            click.echo(
+                self.git_cmd.switch(branch_to_switch).replace("branch", "package")
+            )
 
     def get_history_of_branch(self, branch: str, *params: List[str]) -> str:
         return self.git_cmd.log("--decorate", "--graph", *params, branch)
 
     @staticmethod
     def _get_message_from_editor() -> str:
         with NamedTemporaryFile(suffix=".alpa.tmp") as temp_file:
@@ -134,36 +252,44 @@
     def _ensure_feature_branch(self) -> None:
         if self.branch != self.package:
             return None
 
         click.echo("Switching to feature branch")
         self.git_cmd.switch("-c", self.feat_branch)
 
-    def commit(self, message: str) -> None:
+    def commit(self, message: str, pre_commit: bool) -> bool:
+        if pre_commit:
+            ret = subprocess.run(["pre-commit", "run", "--all-files"])
+            if ret.returncode != 0:
+                return False
+
         self._ensure_feature_branch()
         index = self.local_repo.index
         if message:
             index.commit(message)
         else:
             index.commit(self._get_message_from_editor())
 
+        return True
+
     def add(self, files: List[str]) -> None:
         self._ensure_feature_branch()
         # FIXME: alpa add . acts weird
         self.git_cmd.add(files)
 
     def pull(self, branch: str) -> None:
-        click.echo(self.git_cmd.pull(UPSTREAM_NAME, branch))
+        click.echo(self.git_cmd.pull(self.remote_name, branch))
 
     def push(self, branch: str) -> None:
+        # you always want to push to origin, even from a fork
         click.echo(self.git_cmd.push(ORIGIN_NAME, branch))
 
-    def _get_full_reponame(self) -> str:
+    def full_reponame(self) -> str:
         for remote in self.local_repo.remotes:
-            if remote.name == ORIGIN_NAME:
+            if remote.name == self.remote_name:
                 return remote.url.split(":")[-1].rstrip(".git")
 
         return ""
 
     def create_packit_config(self, override: bool) -> bool:
         packit_conf = PackitConfig(self.package)
         if packit_conf.packit_config_file_exists() and not override:
@@ -173,31 +299,30 @@
         return True
 
 
 class AlpaRepo(LocalRepo):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path)
 
-        self.gh_api = gh_api or GithubAPI()
-        namespace, repo_name = self._get_full_reponame().split("/")
-        self.gh_repo = self.gh_api.get_repo(namespace, repo_name)
+        self.gh_api = gh_api or GithubAPI(self.repo_name)
+        self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
 
     def create_package(self, package: str) -> None:
         upstream = self.gh_repo.get_upstream()
         if upstream and not upstream.has_write_access(self.gh_api.gh_user):
             raise ClickException(NO_WRITE_ACCESS_ERR)
 
         self.git_cmd.switch(MAIN_BRANCH)
         self.git_cmd.switch("-c", package)
-        self.git_cmd.push(UPSTREAM_NAME, package)
+        self.git_cmd.push(self.remote_name, package)
         click.echo(f"Package {package} created")
 
     def request_package(self, package_name: str) -> None:
-        upstream = self.gh_repo.get_root_repo()
-        upstream_namespace = upstream.namespace
+        ensured_upstream = self.gh_repo.get_root_repo()
+        upstream_namespace = ensured_upstream.namespace
         issue_repo = self.gh_api.get_repo(upstream_namespace, self.gh_repo.repo_name)
         issue = issue_repo.create_issue(
             PackageRequest.TITLE.value.format(package_name=package_name),
             PackageRequest.BODY.value.format(
                 user=self.gh_api.gh_user,
                 package_name=package_name,
                 repo_name=self.gh_repo.repo_name,
@@ -206,28 +331,48 @@
         issue.add_to_labels(PackageRequest.LABEL)
 
     def delete_package(self) -> None:
         pass
 
     @staticmethod
     def _prepare_cloned_repo(local_repo: Repo, gh_repo: GithubRepo) -> None:
+        if not gh_repo.is_fork:
+            return
+
         Remote.create(local_repo, UPSTREAM_NAME, gh_repo.upstream_clone_url)
 
     @staticmethod
     def _get_repo_name_from_url(repo_url: str) -> str:
         return repo_url.split("/")[-1].rstrip(".git")
 
+    @staticmethod
+    def _check_for_permission_and_fork(
+        clone_fork: bool, gh_repo: GithubRepo
+    ) -> tuple[bool, str]:
+        if clone_fork and not gh_repo.is_fork:
+            return False, CLONED_REPO_IS_NOT_FORK
+
+        if not clone_fork and gh_repo.is_fork:
+            return False, CLONED_REPO_IS_FORK
+
+        if not gh_repo.is_fork and not gh_repo.has_write_access(gh_repo.api_user):
+            return False, NO_PERMISSION_FOR_ALPA_REPO
+
+        return True, ""
+
     @classmethod
-    def clone(cls, url: str) -> None:
+    def clone(cls, url: str, clone_fork: bool) -> None:
         # in case of `@` in url -> remove the `git@` prefix form it
         repo_path = urlparse(url.split("@")[-1]).path
         parsed_repo_path = repo_path.strip("/").strip(".git")
         namespace, repo_name = parsed_repo_path.split("/")
-        api = GithubAPI()
+        api = GithubAPI(repo_name)
         gh_repo = api.get_repo(namespace, repo_name)
-        if not gh_repo.is_fork():
-            raise UsageError(CLONED_REPO_IS_NOT_FORK)
+
+        check_result, stderr = cls._check_for_permission_and_fork(clone_fork, gh_repo)
+        if not check_result:
+            raise UsageError(stderr)
 
         cloned_repo = Repo.clone_from(
             url, f"{getcwd()}/{cls._get_repo_name_from_url(url)}"
         )
         cls._prepare_cloned_repo(cloned_repo, gh_repo)
```

### Comparing `pyalpa-0.3.2/pyproject.toml` & `pyalpa-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.3.2"
+version = "0.4.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
 exclude = ["test/"]
 packages = [{ include = "alpa" }]
 
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 click = ">=8.0.0"
 gitpython = ">=3.0"
 pygithub = ">=1.4"
 pyyaml = ">=5.0"
 alpa-conf = ">=0.3.2"
+specfile = ">=0.13.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
 
 
 [build-system]
```

### Comparing `pyalpa-0.3.2/PKG-INFO` & `pyalpa-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.3.2
+Version: 0.4.0
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alpa-conf (>=0.3.2)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: gitpython (>=3.0)
 Requires-Dist: pygithub (>=1.4)
 Requires-Dist: pyyaml (>=5.0)
+Requires-Dist: specfile (>=0.13.0)
 Project-URL: Repository, https://github.com/alpa-team/alpa
 Description-Content-Type: text/markdown
 
 ## Alpa
 
 Another cooL way to PAckage in copr
 
@@ -65,13 +65,29 @@
 ```bash
 $ dnf copr enable alpa-team/alpa
 $ dnf install alpa
 ```
 
 ### Usage
 
-TODO
+#### alpa.yaml config file
+
+Example:
+
+```yaml
+---
+api_keys:
+  - repo:
+      name: test-repo
+      key: abcd
+  - repo:
+      name: another-repo
+      key: abcd2
+  - repo:
+      name: yet-another-repo
+      key: abcd3
+```
 
 ### Contributing
 
 TODO
```


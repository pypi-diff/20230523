# Comparing `tmp/ssb_project_cli-1.0.9.tar.gz` & `tmp/ssb_project_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_project_cli-1.0.9.tar", max compression
+gzip compressed data, was "ssb_project_cli-1.1.0.tar", max compression
```

## Comparing `ssb_project_cli-1.0.9.tar` & `ssb_project_cli-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1073 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/LICENSE
--rw-r--r--   0        0        0     2881 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/README.md
--rw-r--r--   0        0        0     2398 2022-11-30 11:28:59.920012 ssb_project_cli-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       23 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/__init__.py
--rw-r--r--   0        0        0      221 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/__main__.py
--rw-r--r--   0        0        0        0 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/py.typed
--rw-r--r--   0        0        0       27 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/__init__.py
--rw-r--r--   0        0        0     2868 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/app.py
--rw-r--r--   0        0        0       29 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/build/__init__.py
--rw-r--r--   0        0        0     1392 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/build/build.py
--rw-r--r--   0        0        0      478 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/build/environment.py
--rw-r--r--   0        0        0     4527 2022-11-30 11:28:45.983828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/build/poetry.py
--rw-r--r--   0        0        0       69 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/build_cmds.md
--rw-r--r--   0        0        0       29 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/clean/__init__.py
--rw-r--r--   0        0        0     4697 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/clean/clean.py
--rw-r--r--   0        0        0       30 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/__init__.py
--rw-r--r--   0        0        0     3985 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/create.py
--rw-r--r--   0        0        0     5908 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/github.py
--rw-r--r--   0        0        0     4192 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/local_repo.py
--rw-r--r--   0        0        0     1631 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/prompt.py
--rw-r--r--   0        0        0      224 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/repo_privacy.py
--rw-r--r--   0        0        0     1303 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
--rw-r--r--   0        0        0      368 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/settings.py
--rw-r--r--   0        0        0     1043 2022-11-30 11:28:45.987828 ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/util.py
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 ssb_project_cli-1.0.9/setup.py
--rw-r--r--   0        0        0     4081 1970-01-01 00:00:00.000000 ssb_project_cli-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-23 13:59:00.044906 ssb_project_cli-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2881 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     2635 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/py.typed
+-rw-r--r--   0        0        0      257 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/__init__.py
+-rw-r--r--   0        0        0     4305 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/app.py
+-rw-r--r--   0        0        0       29 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/__init__.py
+-rw-r--r--   0        0        0     3021 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/build.py
+-rw-r--r--   0        0        0     3740 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/environment.py
+-rw-r--r--   0        0        0     4938 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/poetry.py
+-rw-r--r--   0        0        0     1886 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/prompt.py
+-rw-r--r--   0        0        0     1644 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build/temp_template_repo.py
+-rw-r--r--   0        0        0       69 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/build_cmds.md
+-rw-r--r--   0        0        0       29 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/clean/__init__.py
+-rw-r--r--   0        0        0     3008 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/clean/clean.py
+-rw-r--r--   0        0        0       30 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/__init__.py
+-rw-r--r--   0        0        0     6285 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/create.py
+-rw-r--r--   0        0        0     9618 2023-05-23 13:59:00.048905 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/github.py
+-rw-r--r--   0        0        0     6057 2023-05-23 13:59:15.789056 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/local_repo.py
+-rw-r--r--   0        0        0     1631 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/prompt.py
+-rw-r--r--   0        0        0      224 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/repo_privacy.py
+-rw-r--r--   0        0        0     1303 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/temp_git_repo.py
+-rw-r--r--   0        0        0      368 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/settings.py
+-rw-r--r--   0        0        0     3209 2023-05-23 13:59:00.052906 ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/util.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.0/setup.py
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 ssb_project_cli-1.1.0/PKG-INFO
```

### Comparing `ssb_project_cli-1.0.9/LICENSE` & `ssb_project_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.0.9/README.md` & `ssb_project_cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.0.9/pyproject.toml` & `ssb_project_cli-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-project-cli"
-version = "1.0.9"
+version = "1.1.0"
 description = "SSB Project CLI"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-project-cli"
 repository = "https://github.com/statisticsnorway/ssb-project-cli"
 documentation = "https://ssb-project-cli.readthedocs.io"
@@ -15,26 +15,33 @@
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-project-cli/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.10,<3.11"
 click = ">=8.0.1"
 dparse = "^0.6.2"
 typer = "^0.6.1"
 GitPython = "^3.1.27"
 PyGithub = "^1.55"
 cruft = "^2.11.1"
 rich = "^12.5.1"
 urllib3 = "^1.26.12"
 requests = "^2.28.1"
 types-toml = "^0.10.8"
 questionary = "^1.10.0"
+certifi = "^2022.12.7"
+psutil = "^5.9.4"
+types-urllib3 = "^1.26.25.10"
+types-requests = "^2.28.11.17"
+types-psutil = "^5.9.5.12"
+kvakk-git-tools = "^2.2.1"
+
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
@@ -44,15 +51,15 @@
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
-pytest = ">=6.2.5"
+pytest = ">=7.2.0"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
@@ -69,14 +76,17 @@
 build = "^0.8.0"
 Jinja2 = "^3.1.2"
 
 
 [tool.poetry.scripts]
 ssb-project = "ssb_project_cli.__main__:main"
 
+[tool.poetry.group.dev.dependencies]
+nox = "^2022.11.21"
+nox-poetry = "^1.0.2"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/local_repo.py` & `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,130 @@
-"""This module contains functions used to set up a local git repository with ssb-project."""
-import json
-import subprocess  # noqa: S404
-from datetime import datetime
+"""Command-line-interface for project-operations in dapla-jupterlab."""
 from pathlib import Path
-from typing import Optional
 
-from git import Repo  # type: ignore[attr-defined]
-from github import Github
+import typer
+from rich.console import Console
 
-from ssb_project_cli.ssb_project.create import temp_git_repo
-from ssb_project_cli.ssb_project.create.prompt import request_name_email
+from ssb_project_cli.ssb_project.util import set_debug_logging
 
-
-def create_project_from_template(
-    project_name: str,
-    description: str,
-    template_repo_url: str,
-    template_reference: str,
-    working_directory: Path,
-    license_year: Optional[str] = None,
-) -> Path:
-    """Creates a project from CookiCutter template.
-
-    Args:
-        project_name: Name of project
-        description: Project description
-        license_year: Year to be inserted into the LICENSE
-        template_repo_url: URL for the chosen template
-        template_reference: Git reference to the template repository
-        working_directory: Working directory
-
-    Returns:
-        Path: Path of project.
-    """
-    project_dir = working_directory.joinpath(project_name)
-    if project_dir.exists():
-        print(
-            f"A project with name '{project_name}' already exists. Please choose another name."
-        )
-        exit(1)
-
-    name, email = extract_name_email()
-    if not (name and email):
-        name, email = request_name_email()
-
-    template_info = {
-        "project_name": project_name,
-        "description": description,
-        "full_name": name,
-        "email": email,
-        "license_year": license_year or str(datetime.now().year),
-    }
-    quoted = json.dumps(template_info).replace('"', '"')
-
-    argv = [
-        "cruft",
-        "create",
-        template_repo_url,
-        "--no-input",
-        "--checkout",
-        template_reference,
-        "--extra-context",
-        quoted,
-    ]
-
-    subprocess.run(  # noqa: S603 no untrusted input
-        argv, check=True, cwd=working_directory
+from .build.build import build_project
+from .clean.clean import clean_project
+from .create.create import create_project
+from .create.repo_privacy import RepoPrivacy
+from .settings import CURRENT_WORKING_DIRECTORY
+from .settings import GITHUB_ORG_NAME
+from .settings import HOME_PATH
+from .settings import STAT_TEMPLATE_DEFAULT_REFERENCE
+from .settings import STAT_TEMPLATE_REPO_URL
+
+
+# Don't print with color, it's difficult to read when run in Jupyter
+typer.rich_utils.STYLE_OPTION = ""
+typer.rich_utils.STYLE_SWITCH = ""
+typer.rich_utils.STYLE_NEGATIVE_OPTION = ""
+typer.rich_utils.STYLE_NEGATIVE_SWITCH = ""
+typer.rich_utils.STYLE_METAVAR = ""
+typer.rich_utils.STYLE_METAVAR_SEPARATOR = "dim"
+typer.rich_utils.STYLE_USAGE = ""
+typer.rich_utils.STYLE_USAGE_COMMAND = "bold"
+typer.rich_utils.STYLE_DEPRECATED = ""
+typer.rich_utils.STYLE_DEPRECATED_COMMAND = "dim"
+typer.rich_utils.STYLE_HELPTEXT_FIRST_LINE = ""
+typer.rich_utils.STYLE_HELPTEXT = ""
+typer.rich_utils.STYLE_OPTION_HELP = ""
+typer.rich_utils.STYLE_OPTION_DEFAULT = "dim"
+typer.rich_utils.STYLE_OPTION_ENVVAR = "dim"
+typer.rich_utils.STYLE_REQUIRED_SHORT = ""
+typer.rich_utils.STYLE_REQUIRED_LONG = ""
+typer.rich_utils.STYLE_OPTIONS_PANEL_BORDER = "dim"
+console = Console(color_system=None)
+print = console.print
+
+app = typer.Typer(
+    help="Usage instructions: https://manual.dapla.ssb.no/ssbproject.html",
+    rich_markup_mode="rich",
+    pretty_exceptions_show_locals=False,  # Locals can contain sensitive information
+)
+
+
+@app.command()
+def create(  # noqa: C901
+    project_name: str = typer.Argument(..., help="Project name"),  # noqa: B008
+    description: str = typer.Argument(  # noqa: B008
+        "", help="A short description of your project"
+    ),
+    repo_privacy: RepoPrivacy = typer.Argument(  # noqa: B008
+        RepoPrivacy.internal, help="Visibility of the Github repo"
+    ),
+    add_github: bool = typer.Option(  # noqa: B008
+        False,
+        "--github",
+        help="Create the repo on Github as well",
+    ),
+    github_token: str = typer.Option(  # noqa: B008
+        "",
+        help="Your Github Personal Access Token, follow these instructions to create one: https://manual.dapla.ssb.no/git-github.html#personal-access-token-pat",
+    ),
+    verify_config: bool = typer.Option(  # noqa: B008
+        True,
+        "--no-verify",
+        help="Verify git configuration files. Use --no-verify to disable verification (defaults to True).",
+        show_default=True,
+    ),
+) -> None:
+    """:sparkles:  Create a project locally, and optionally on GitHub with the flag --github. The project will follow SSB's best practice for development."""
+    create_project(
+        project_name,
+        description,
+        repo_privacy,
+        add_github,
+        github_token,
+        CURRENT_WORKING_DIRECTORY,
+        HOME_PATH,
+        GITHUB_ORG_NAME,
+        STAT_TEMPLATE_REPO_URL,
+        STAT_TEMPLATE_DEFAULT_REFERENCE,
+        verify_config,
     )
 
-    return project_dir
-
-
-def extract_name_email() -> tuple[str, str]:
-    """Grabs email and name from git config.
-
-    Returns:
-        name: Value of user.name from git config element
-        email: Value of user.email from git config element
-    """
-    name = get_gitconfig_element("user.name")
-    email = get_gitconfig_element("user.email")
-    return name, email
 
-
-def get_gitconfig_element(element: str) -> str:
-    """Grabs a property from git config.
-
-    Args:
-        element: Name of the git config element retrive
-
-    Returns:
-        str: Value of git config element
-    """
-    cmd = ["git", "config", "--get", element]
-    result = subprocess.run(  # noqa: S603 no untrusted input
-        cmd, stdout=subprocess.PIPE, encoding="utf-8"
+@app.command()
+def build(
+    path: Path = typer.Argument(  # noqa: B008
+        "",
+        help="Project path",
+    ),
+    verify_config: bool = typer.Option(  # noqa: B008
+        True,
+        "--no-verify",
+        help="Verify git configuration files. Use --no-verify to disable verification (defaults to True).",
+        show_default=True,
+    ),
+) -> None:
+    """:wrench:  Create a virtual environment and corresponding Jupyter kernel. Runs in the current folder if no arguments are supplied."""
+    build_project(
+        path,
+        CURRENT_WORKING_DIRECTORY,
+        STAT_TEMPLATE_REPO_URL,
+        STAT_TEMPLATE_DEFAULT_REFERENCE,
+        verify_config,
     )
 
-    return result.stdout.strip()
-
 
-def make_and_init_git_repo(repo_dir: Path) -> Repo:
-    """Makes and pushes a GitHub repository.
-
-    Inits a local repository, adds all files and commits.
-
-    Args:
-        repo_dir: Path to local Repository
-
-    Returns:
-        Repo: Repository
-    """
-    repo = Repo.init(repo_dir)
-    repo.git.add("-A")
-    repo.index.commit("Initial commit")
-    repo.git.branch("-M", "main")
-    return repo
-
-
-def make_git_repo_and_push(github_token: str, github_url: str, repo_dir: Path) -> None:
-    """Makes and pushes a GitHub repository.
-
-    Inits a local repository and tries to push it to GitHub,
-     for more information see TempGitRemote.
-
-    Args:
-        github_token: GitHub personal access token
-        github_url: Repository url
-        repo_dir: Path to local Repository
-    """
-    repo = make_and_init_git_repo(repo_dir)
+@app.command()
+def clean(
+    project_name: str = typer.Argument(  # noqa: B008
+        ..., help="The name of the project/kernel you want to delete."
+    )
+) -> None:
+    """:broom:  Delete the kernel for the given project name."""
+    clean_project(project_name)
 
-    github_username = Github(github_token).get_user().login
-    credential_url = mangle_url(github_url, github_token)
-    username_url = mangle_url(github_url, github_username)
 
-    with temp_git_repo.TempGitRemote(repo, credential_url, username_url):
-        repo.git.push("--set-upstream", "origin", "main")
+def main() -> None:
+    """Main function of ssb_project_cli."""
+    set_debug_logging()
+    app(prog_name="ssb-project")  # pragma: no cover
 
 
-def mangle_url(url: str, mangle_name: str) -> str:
-    """Create url mangled with a string: credential or username."""
-    mangle_name = mangle_name + "@"
-    split_index = url.find("//") + 2
-    return url[:split_index] + mangle_name + url[split_index:]
+if __name__ == "__main__":
+    main()  # pragma: no cover
```

### Comparing `ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/prompt.py` & `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/prompt.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.0.9/src/ssb_project_cli/ssb_project/create/temp_git_repo.py` & `ssb_project_cli-1.1.0/src/ssb_project_cli/ssb_project/create/temp_git_repo.py`

 * *Files identical despite different names*

### Comparing `ssb_project_cli-1.0.9/setup.py` & `ssb_project_cli-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,40 +13,46 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['GitPython>=3.1.27,<4.0.0',
  'PyGithub>=1.55,<2.0',
+ 'certifi>=2022.12.7,<2023.0.0',
  'click>=8.0.1',
  'cruft>=2.11.1,<3.0.0',
  'dparse>=0.6.2,<0.7.0',
+ 'kvakk-git-tools>=2.2.1,<3.0.0',
+ 'psutil>=5.9.4,<6.0.0',
  'questionary>=1.10.0,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=12.5.1,<13.0.0',
  'typer>=0.6.1,<0.7.0',
+ 'types-psutil>=5.9.5.12,<6.0.0.0',
+ 'types-requests>=2.28.11.17,<3.0.0.0',
  'types-toml>=0.10.8,<0.11.0',
+ 'types-urllib3>=1.26.25.10,<2.0.0.0',
  'urllib3>=1.26.12,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ssb-project = ssb_project_cli.__main__:main']}
 
 setup_kwargs = {
     'name': 'ssb-project-cli',
-    'version': '1.0.9',
+    'version': '1.1.0',
     'description': 'SSB Project CLI',
     'long_description': '# SSB Project CLI\n\n[![PyPI](https://img.shields.io/pypi/v/ssb-project-cli.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/ssb-project-cli.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/ssb-project-cli)][pypi status]\n[![License](https://img.shields.io/pypi/l/ssb-project-cli)][license]\n\n[![Read the documentation](https://img.shields.io/badge/docs-Github%20Pages-purple)](https://statisticsnorway.github.io/ssb-project-cli/)\n[![Tests](https://github.com/statisticsnorway/ssb-project-cli/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/statisticsnorway/ssb-project-cli/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/ssb-project-cli/\n[read the docs]: https://ssb-project-cli.readthedocs.io/\n[tests]: https://github.com/statisticsnorway/ssb-project-cli/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/statisticsnorway/ssb-project-cli\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n![Help text](docs/assets/cli_help_screenshot.png)\n\n- Create a new project quickly and easily with `ssb-project create`.\n- Your colleagues can quickly get started when you share the project with them with `ssb-project build`.\n- Includes:\n  - Local directory structure\n  - Virtual Environment\n  - Kernel for use on Jupyter\n  - Github repo (if desired)\n- The project will follow the most recent SSB guidelines for security and quality.\n- It will always be possible to update existing projects as guidelines change.\n\n## Installation\n\nYou can install _SSB Project CLI_ via [pip] from [PyPI]:\n\n```console\npip install ssb-project-cli\n```\n\n## Releasing a new version\n\nTo release a new version of the CLI, run the following sequence.\n\n```console\ngit switch --create release main\n```\n\n```console\npoetry version <version>\n```\n\n```console\ngit commit --message="<project> <version>" pyproject.toml\n```\n\n```console\ngit push origin release\n```\n\n## Contributing\n\n### Setup\n\n1. [Install dependencies](https://cookiecutter-hypermodern-python.readthedocs.io/en/latest/guide.html#installation)\n1. [Install pre-commit hooks](https://cookiecutter-hypermodern-python.readthedocs.io/en/latest/guide.html#running-pre-commit-from-git)\n1. Run tests: `nox -r` ([More information here](https://cookiecutter-hypermodern-python.readthedocs.io/en/latest/guide.html#using-nox))\n1. Run the help command: `poetry run ssb-project --help`\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_SSB Project CLI_ is free and open source software.\n\n<!-- github-only -->\n\n[license]: https://github.com/statisticsnorway/ssb-project-cli/blob/main/LICENSE\n',
     'author': 'Statistics Norway',
     'author_email': 'stat-dev@ssb.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/statisticsnorway/ssb-project-cli',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.11',
+    'python_requires': '>=3.10,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ssb_project_cli-1.0.9/PKG-INFO` & `ssb_project_cli-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: ssb-project-cli
-Version: 1.0.9
+Version: 1.1.0
 Summary: SSB Project CLI
 Home-page: https://github.com/statisticsnorway/ssb-project-cli
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: PyGithub (>=1.55,<2.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: cruft (>=2.11.1,<3.0.0)
 Requires-Dist: dparse (>=0.6.2,<0.7.0)
+Requires-Dist: kvakk-git-tools (>=2.2.1,<3.0.0)
+Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: types-psutil (>=5.9.5.12,<6.0.0.0)
+Requires-Dist: types-requests (>=2.28.11.17,<3.0.0.0)
 Requires-Dist: types-toml (>=0.10.8,<0.11.0)
+Requires-Dist: types-urllib3 (>=1.26.25.10,<2.0.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-project-cli/releases
 Project-URL: Documentation, https://ssb-project-cli.readthedocs.io
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-project-cli
 Description-Content-Type: text/markdown
 
 # SSB Project CLI
```


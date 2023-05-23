# Comparing `tmp/tft-cli-0.0.8.tar.gz` & `tmp/tft-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tft-cli-0.0.8.tar", max compression
+gzip compressed data, was "tft-cli-0.0.9.tar", max compression
```

## Comparing `tft-cli-0.0.8.tar` & `tft-cli-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      574 2023-02-21 15:28:41.141348 tft-cli-0.0.8/LICENSE
--rw-r--r--   0        0        0       88 2023-02-21 15:28:41.141348 tft-cli-0.0.8/LICENSE_SPDX
--rw-r--r--   0        0        0      865 2023-02-28 09:30:59.162122 tft-cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       92 2023-02-21 15:28:41.143349 tft-cli-0.0.8/src/tft/cli/__init__.py
--rw-r--r--   0        0        0    12838 2023-03-01 09:24:30.713108 tft-cli-0.0.8/src/tft/cli/commands.py
--rw-r--r--   0        0        0      675 2023-02-21 15:28:41.143349 tft-cli-0.0.8/src/tft/cli/config.py
--rw-r--r--   0        0        0      259 2023-02-21 15:28:41.143349 tft-cli-0.0.8/src/tft/cli/tool.py
--rw-r--r--   0        0        0     4227 2023-02-28 09:13:25.721103 tft-cli-0.0.8/src/tft/cli/utils.py
--rw-r--r--   0        0        0      916 2023-04-03 20:43:30.524015 tft-cli-0.0.8/setup.py
--rw-r--r--   0        0        0      641 2023-04-03 20:43:30.524170 tft-cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      574 2023-02-21 15:28:41.141348 tft-cli-0.0.9/LICENSE
+-rw-r--r--   0        0        0       88 2023-02-21 15:28:41.141348 tft-cli-0.0.9/LICENSE_SPDX
+-rw-r--r--   0        0        0      878 2023-05-23 16:40:15.962486 tft-cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-02-21 15:28:41.143349 tft-cli-0.0.9/src/tft/cli/__init__.py
+-rw-r--r--   0        0        0    18049 2023-05-23 12:33:42.089141 tft-cli-0.0.9/src/tft/cli/commands.py
+-rw-r--r--   0        0        0      745 2023-04-19 08:30:28.905651 tft-cli-0.0.9/src/tft/cli/config.py
+-rw-r--r--   0        0        0      291 2023-05-23 12:33:42.089141 tft-cli-0.0.9/src/tft/cli/tool.py
+-rw-r--r--   0        0        0     4876 2023-05-23 12:33:42.091140 tft-cli-0.0.9/src/tft/cli/utils.py
+-rw-r--r--   0        0        0      896 2023-05-23 16:41:47.220545 tft-cli-0.0.9/setup.py
+-rw-r--r--   0        0        0      607 2023-05-23 16:41:47.220914 tft-cli-0.0.9/PKG-INFO
```

### Comparing `tft-cli-0.0.8/LICENSE` & `tft-cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tft-cli-0.0.8/pyproject.toml` & `tft-cli-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "tft-cli"
-version = "0.0.8"
+version = "0.0.9"
 description = "Testing Farm CLI tool"
 authors = ["Miroslav Vadkerti <mvadkert@redhat.com>"]
 license = "Apache-2.0"
 
 packages = [
   { include = "tft", from = "src" }
 ]
 
 [tool.poetry.scripts]
 testing-farm = "tft.cli.tool:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-typer = "^0.4.0"
+typer = {extras = ["all"], version = "^0.7.0"}
 # click 8.1.0 broke typer 0.4.0
 # https://github.com/tiangolo/typer/pull/375
 click = "~8.0.4"
 dynaconf = "^3.1.7"
 colorama = "^0.4.4"
 requests = "^2.27.1"
-rich = "^13.3.1"
 
 [tool.poetry.dev-dependencies]
 pyre-check = "^0.9.10"
 pytest = "^7.0.0"
 isort = "^5.10.1"
 black = "^22.1.0"
 pre-commit = "^2.17.0"
```

### Comparing `tft-cli-0.0.8/src/tft/cli/commands.py` & `tft-cli-0.0.9/src/tft/cli/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,25 +19,29 @@
 from tft.cli.utils import (
     artifacts,
     blue,
     cmd_output_or_exit,
     exit_error,
     hw_constraints,
     install_http_retries,
+    normalize_multistring_option,
     options_to_dict,
     uuid_valid,
 )
 
 cli_version: str = pkg_resources.get_distribution("tft-cli").version
 
 TestingFarmRequestV1: Dict[str, Any] = {'api_key': None, 'test': {}, 'environments': None}
-Environments: List[Dict[str, Any]] = [{'arch': None, 'os': None, 'pool': None, 'artifacts': None}]
+Environment: Dict[str, Any] = {'arch': None, 'os': None, 'pool': None, 'artifacts': None}
 TestTMT: Dict[str, Any] = {'url': None, 'ref': None, 'name': None}
 TestSTI: Dict[str, Any] = {'url': None, 'ref': None}
 
+REQUEST_PANEL_TMT = "TMT Options"
+REQUEST_PANEL_STI = "STI Options"
+
 
 def watch(
     api_url: str = typer.Option(settings.API_URL, help="Testing Farm API URL."),
     id: str = typer.Option(..., help="Request ID to watch"),
     no_wait: bool = typer.Option(False, help="Skip waiting for request completion."),
 ):
     """Watch request for completion."""
@@ -119,29 +123,57 @@
 
 def version():
     """Print CLI version"""
     typer.echo(f"{cli_version}")
 
 
 def request(
-    api_url: str = typer.Option(settings.API_URL, help="Testing Farm API URL."),
+    api_url: str = typer.Argument(
+        settings.API_URL, envvar="TESTING_FARM_API_URL", metavar='', rich_help_panel='Environment variables'
+    ),
+    api_token: str = typer.Argument(
+        settings.API_TOKEN,
+        envvar="TESTING_FARM_API_TOKEN",
+        show_default=False,
+        metavar='',
+        rich_help_panel='Environment variables',
+    ),
+    timeout: Optional[int] = typer.Option(
+        60 * 12,
+        help="Set the timeout for the request in minutes. If the test takes longer than this, it will be terminated. Testing Farm internal default is 12h.",  # noqa
+    ),
     test_type: str = typer.Option("fmf", help="Test type to use, if not set autodetected."),
     tmt_plan_regex: Optional[str] = typer.Option(
-        None, "--plan", help="Regex for selecting plans, by default all plans are selected."
+        None,
+        "--plan",
+        help="Regex for selecting plans, by default all plans are selected.",
+        rich_help_panel=REQUEST_PANEL_TMT,
+    ),
+    tmt_plan_filter_regex: Optional[str] = typer.Option(
+        None,
+        "--plan-filter",
+        help="Regex for filtering plans, by default only enabled plans are executed.",
+        rich_help_panel=REQUEST_PANEL_TMT,
+    ),
+    tmt_test_filter_regex: Optional[str] = typer.Option(
+        None, "--test-filter", help="Regex for filtering tests.", rich_help_panel=REQUEST_PANEL_TMT
     ),
     sti_playbooks: Optional[List[str]] = typer.Option(
-        None, "--playbook", help="Playbook to run, by default 'tests/tests*.yml', multiple playbooks can be specified."
+        None,
+        "--playbook",
+        help="Playbook to run, by default 'tests/tests*.yml', multiple playbooks can be specified.",
+        rich_help_panel=REQUEST_PANEL_STI,
     ),
     git_url: Optional[str] = typer.Option(
         None, help="URL of the GIT repository to test. If not set autodetected from current git repository."
     ),
     git_ref: str = typer.Option(
         "main", help="GIT ref or branch to test. If not set autodetected from current git repository."
     ),
-    arch: str = typer.Option("x86_64", help="Hardware platfrom of the system to be provisioned."),
+    arches: List[str] = typer.Option(["x86_64"], "--arch", help="Hardware platforms of the system to be provisioned."),
     compose: Optional[str] = typer.Option(
         None,
         help="Compose used to provision system-under-test. If not set tests will expect 'container' provision method specified in tmt plans.",  # noqa
     ),
     hardware: List[str] = typer.Option(
         None,
         help=(
@@ -175,30 +207,28 @@
         None,
         help="Fedora Copr build to install on the test environment, specified using `build-id:chroot-name`, e.g. 1784470:fedora-32-x86_64.",  # noqa
     ),
     repository: List[str] = typer.Option(
         None, help="Repository base url to add to the test environment and install all packages from it."
     ),
     tags: Optional[List[str]] = typer.Option(
-        None, "-t", "--tags", metavar="key=value", help="Context variables to pass to `tmt`."
+        None, "-t", "--tag", metavar="key=value", help="Tag cloud resources with given value."
     ),
     dry_run: bool = typer.Option(False, help="Do not submit request, just print it"),
 ):
     """
     Request testing from Testing Farm.
-
-    Environment variables:
-
-        TESTING_FARM_API_URL            - Testing Farm API URL
-        TESTING_FARM_API_TOKEN          - API token used to authenticate.
     """
+    # Split comma separated arches
+    arches = normalize_multistring_option(arches)
+
     git_available = bool(shutil.which("git"))
 
     # check for token
-    if not settings.API_TOKEN:
+    if not api_token:
         exit_error("No API token found, export `TESTING_FARM_API_TOKEN` environment variable")
 
     # resolve git repository details from the current repository
     if not git_url:
         if not git_available:
             exit_error("no git url defined")
 
@@ -244,81 +274,89 @@
     # STI is not supported against a container
     if test_type == "sti" and compose == "container":
         exit_error("container based testing is not available for 'sti' test type")
 
     typer.echo(f"📦 repository {blue(git_url)} ref {blue(git_ref)} test-type {blue(test_type)}")
 
     pool_info = f"via pool {blue(pool)}" if pool else ""
-    typer.echo(f"💻 {blue(compose or 'container image in plan')} on {blue(arch)} {pool_info}")
+    for arch in arches:
+        typer.echo(f"💻 {blue(compose or 'container image in plan')} on {blue(arch)} {pool_info}")
 
     # test details
     test = TestTMT if test_type == "fmf" else TestSTI
     test["url"] = git_url
     test["ref"] = git_ref
 
     if tmt_plan_regex:
         test["name"] = tmt_plan_regex
 
+    if tmt_plan_filter_regex:
+        test["plan_filter"] = tmt_plan_filter_regex
+
+    if tmt_test_filter_regex:
+        test["test_filter"] = tmt_test_filter_regex
+
     if sti_playbooks:
         test["playbooks"] = sti_playbooks
 
     # environment details
-    environments = Environments
-    environments[0]["arch"] = arch
-    environments[0]["pool"] = pool
-    environments[0]["artifacts"] = []
+    environments = []
+    for arch in arches:
+        environment = Environment.copy()
+        environment["arch"] = arch
+        environment["pool"] = pool
+        environment["artifacts"] = []
 
-    if compose:
-        environments[0]["os"] = {"compose": compose}
+        if compose:
+            environment["os"] = {"compose": compose}
 
-    if secrets:
-        environments[0]["secrets"] = options_to_dict("environment secrets", secrets)
+        if secrets:
+            environment["secrets"] = options_to_dict("environment secrets", secrets)
 
-    if tmt_context:
-        environments[0]["tmt"] = {"context": options_to_dict("tmt context", tmt_context)}
+        if tmt_context:
+            environment["tmt"] = {"context": options_to_dict("tmt context", tmt_context)}
 
-    if variables:
-        environments[0]["variables"] = options_to_dict("environment variables", variables)
+        if variables:
+            environment["variables"] = options_to_dict("environment variables", variables)
 
-    if hardware:
-        environments[0]["hardware"] = hw_constraints(hardware)
+        if hardware:
+            environment["hardware"] = hw_constraints(hardware)
 
-    if redhat_brew_build:
-        environments[0]["artifacts"].extend(artifacts("redhat-brew-build", redhat_brew_build))
+        if redhat_brew_build:
+            environment["artifacts"].extend(artifacts("redhat-brew-build", redhat_brew_build))
 
-    if fedora_koji_build:
-        environments[0]["artifacts"].extend(artifacts("fedora-koji-build", fedora_koji_build))
+        if fedora_koji_build:
+            environment["artifacts"].extend(artifacts("fedora-koji-build", fedora_koji_build))
 
-    if fedora_copr_build:
-        environments[0]["artifacts"].extend(artifacts("fedora-copr-build", fedora_copr_build))
+        if fedora_copr_build:
+            environment["artifacts"].extend(artifacts("fedora-copr-build", fedora_copr_build))
 
-    if repository:
-        environments[0]["artifacts"].extend(artifacts("repository", repository))
+        if repository:
+            environment["artifacts"].extend(artifacts("repository", repository))
 
-    if tags:
-        environments[0]["settings"] = {
-                "provisioning": {
-                    "tags": options_to_dict("tags", tags)
-                }
-        }
+        environments.append(environment)
 
+    if tags:
+        environments[0]["settings"] = {"provisioning": {"tags": options_to_dict("tags", tags)}}
 
     # create final request
     request = TestingFarmRequestV1
-    request["api_key"] = settings.API_TOKEN
+    request["api_key"] = api_token
     if test_type == "fmf":
         request["test"]["fmf"] = test
     else:
         request["test"]["sti"] = test
+
     request["environments"] = environments
+    request["settings"] = {}
+    request["settings"]["pipeline"] = {"timeout": timeout}
 
     # worker image
     if worker_image:
-        request["settings"] = {"worker": {"image": worker_image}}
-
+        request["settings"]["worker"] = {"image": worker_image}
     # submit request to Testing Farm
     post_url = urllib.parse.urljoin(api_url, "v0.1/requests")
 
     # Setting up retries
     session = requests.Session()
     install_http_retries(session)
 
@@ -337,7 +375,118 @@
         exit_error(f"Request is invalid. Please file an issue to {settings.ISSUE_TRACKER}")
 
     if response.status_code != 200:
         exit_error(f"Unexpected error. Please file an issue to {settings.ISSUE_TRACKER}.")
 
     # watch
     watch(api_url, response.json()['id'], no_wait)
+
+
+def restart(
+    request_id: str = typer.Argument(..., help="Testing Farm request ID or an string containing it."),
+    api_url: str = typer.Argument(
+        settings.API_URL, envvar="TESTING_FARM_API_URL", metavar='', rich_help_panel='Environment variables'
+    ),
+    internal_api_url: str = typer.Argument(
+        settings.INTERNAL_API_URL,
+        envvar="TESTING_FARM_INTERNAL_API_URL",
+        metavar='',
+        rich_help_panel='Environment variables',
+    ),
+    api_token: str = typer.Argument(
+        settings.API_TOKEN,
+        envvar="TESTING_FARM_API_TOKEN",
+        show_default=False,
+        metavar='',
+        rich_help_panel='Environment variables',
+    ),
+    compose: Optional[str] = typer.Option(
+        None,
+        help="Change compose used to provision system-under-test. If not set it will use the compose from the original request.",  # noqa
+    ),
+    no_wait: bool = typer.Option(False, help="Skip waiting for request completion."),
+    dry_run: bool = typer.Option(False, help="Do not submit request, just print it"),
+):
+    """
+    Restart a Testing Farm request.
+
+    Just pass a request ID or an URL with a request ID to restart it.
+    """
+
+    # UUID pattern
+    uuid_pattern = re.compile('[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}')
+
+    # Find the UUID in the string
+    uuid_match = uuid_pattern.search(request_id)
+
+    if not uuid_match:
+        exit_error(f"Could not find a valid Testing Farm request id in '{request_id}'.")
+        return
+
+    # Extract the UUID from the match object
+    _request_id = uuid_match.group()
+
+    # Construct URL to the internal API
+    get_url = urllib.parse.urljoin(str(internal_api_url), f"v0.1/requests/{_request_id}?api_key={api_token}")
+
+    # Setting up retries
+    session = requests.Session()
+    install_http_retries(session)
+
+    # Get the request details
+    response = session.get(get_url)
+
+    if response.status_code == 404:
+        exit_error(f"API token is invalid. See {settings.ONBOARDING_DOCS} for more information.")
+
+    if response.status_code != 200:
+        exit_error(f"Unexpected error. Please file an issue to {settings.ISSUE_TRACKER}.")
+
+    request = response.json()
+
+    # Transform to a request
+    request['environments'] = request['environments_requested']
+
+    # Remove all keys except test and environments
+    for key in list(request):
+        if key not in ['test', 'environments']:
+            del request[key]
+
+    # Remove empty test keys
+    for key in list(request['test']):
+        if not request['test'][key]:
+            del request['test'][key]
+
+    # Set compose
+    if compose:
+        typer.echo(f"💻 forcing {blue(compose)}")
+        for environment in request['environments']:
+            if environment.get("os") is None:
+                environment["os"] = {}
+            environment["os"]["compose"] = compose
+
+    # Add API key
+    request['api_key'] = api_token
+
+    # dry run
+    if dry_run:
+        typer.secho("🔍 Dry run, showing POST json only", fg=typer.colors.BRIGHT_YELLOW)
+        print(json.dumps(request, indent=4, separators=(',', ': ')))
+        raise typer.Exit()
+
+    # submit request to Testing Farm
+    post_url = urllib.parse.urljoin(str(api_url), "v0.1/requests")
+
+    # handle errors
+    response = session.post(post_url, json=request)
+    if response.status_code == 404:
+        exit_error(f"API token is invalid. See {settings.ONBOARDING_DOCS} for more information.")
+
+    if response.status_code == 400:
+        print(response.text)
+        exit_error(f"Request is invalid. Please file an issue to {settings.ISSUE_TRACKER}")
+
+    if response.status_code != 200:
+        exit_error(f"Unexpected error. Please file an issue to {settings.ISSUE_TRACKER}.")
+
+    # watch
+    watch(str(api_url), response.json()['id'], no_wait)
```

### Comparing `tft-cli-0.0.8/src/tft/cli/utils.py` & `tft-cli-0.0.9/src/tft/cli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -114,24 +114,37 @@
 
 def install_http_retries(
     session: requests.Session,
     timeout: int = settings.DEFAULT_API_TIMEOUT,
     retries: int = settings.DEFAULT_API_RETRIES,
     retry_backoff_factor: int = settings.DEFAULT_RETRY_BACKOFF_FACTOR,
 ) -> None:
-    retry_strategy = Retry(
-        total=retries,
-        status_forcelist=[
+    # urllib3 1.26.0 deprecated method_whitelist, and 2.0.0 removed it:
+    #  - https://github.com/urllib3/urllib3/commit/382ab32f23795c44faae83b4e8b18a16fb605a0a
+    #  - https://github.com/urllib3/urllib3/commit/c67c0949e9c91c7621ea718a7f297ecac7c3b79e
+    if hasattr(Retry, "DEFAULT_ALLOWED_METHODS"):
+        allowed_retry_parameter = "allowed_methods"
+    else:
+        allowed_retry_parameter = "method_whitelist"
+
+    params = {
+        "total": retries,
+        "status_forcelist": [
             429,  # Too Many Requests
             500,  # Internal Server Error
             502,  # Bad Gateway
             503,  # Service Unavailable
             504,  # Gateway Timeout
         ],
-        method_whitelist=['HEAD', 'GET', 'POST', 'DELETE', 'PUT'],
-        backoff_factor=retry_backoff_factor,
-    )
+        allowed_retry_parameter: ['HEAD', 'GET', 'POST', 'DELETE', 'PUT'],
+        "backoff_factor": retry_backoff_factor,
+    }
+    retry_strategy = Retry(**params)
 
     timeout_adapter = TimeoutHTTPAdapter(timeout=timeout, max_retries=retry_strategy)
 
     session.mount('https://', timeout_adapter)
     session.mount('http://', timeout_adapter)
+
+
+def normalize_multistring_option(options: List[str], separator: str = ',') -> List[str]:
+    return sum([[option.strip() for option in item.split(separator)] for item in options], [])
```

### Comparing `tft-cli-0.0.8/setup.py` & `tft-cli-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 {'': ['*']}
 
 install_requires = \
 ['click>=8.0.4,<8.1.0',
  'colorama>=0.4.4,<0.5.0',
  'dynaconf>=3.1.7,<4.0.0',
  'requests>=2.27.1,<3.0.0',
- 'rich>=13.3.1,<14.0.0',
- 'typer>=0.4.0,<0.5.0']
+ 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['testing-farm = tft.cli.tool:app']}
 
 setup_kwargs = {
     'name': 'tft-cli',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Testing Farm CLI tool',
     'long_description': None,
     'author': 'Miroslav Vadkerti',
     'author_email': 'mvadkert@redhat.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tft-cli-0.0.8/PKG-INFO` & `tft-cli-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tft-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Testing Farm CLI tool
 License: Apache-2.0
 Author: Miroslav Vadkerti
 Author-email: mvadkert@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.0.4,<8.1.0)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: dynaconf (>=3.1.7,<4.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
-Requires-Dist: typer (>=0.4.0,<0.5.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
```


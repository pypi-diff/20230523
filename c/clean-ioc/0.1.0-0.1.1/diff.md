# Comparing `tmp/clean_ioc-0.1.0.tar.gz` & `tmp/clean_ioc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.1.0.tar", max compression
+gzip compressed data, was "clean_ioc-0.1.1.tar", max compression
```

## Comparing `clean_ioc-0.1.0.tar` & `clean_ioc-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-05-17 21:04:51.684575 clean_ioc-0.1.0/LICENSE
--rw-r--r--   0        0        0    14851 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/README.md
--rw-r--r--   0        0        0    27728 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/__init__.py
--rw-r--r--   0        0        0      674 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0     1811 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6537 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1125 2023-05-17 21:04:51.688575 clean_ioc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    16063 1970-01-01 00:00:00.000000 clean_ioc-0.1.0/setup.py
--rw-r--r--   0        0        0    15491 1970-01-01 00:00:00.000000 clean_ioc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/LICENSE
+-rw-r--r--   0        0        0    15650 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/README.md
+-rw-r--r--   0        0        0    31136 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/__init__.py
+-rw-r--r--   0        0        0      674 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0     1811 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6537 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1125 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    16897 1970-01-01 00:00:00.000000 clean_ioc-0.1.1/setup.py
+-rw-r--r--   0        0        0    16290 1970-01-01 00:00:00.000000 clean_ioc-0.1.1/PKG-INFO
```

### Comparing `clean_ioc-0.1.0/LICENSE` & `clean_ioc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.0/README.md` & `clean_ioc-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -616,21 +616,55 @@
         self.module = module
 
 class Client
     def __init__(self, logger: Logger)
         self.logger = logger
 
 def logger_fac(context: DependencyContext):
-    module = context.parent.__module__
+    module = context.parent.implementation.__module__
     return Logger(module)
 
 
 container = Container()
 container.register(Client)
 container.register(Logger, factory=logger_fac)
 
-container.apply_module(client_module)
-
 client = container.resolve(Client)
 
 
 ```
+
+
+## Pre-configurations
+
+Pre configurations run a side-effect for a type before the type gets resolved.
+This is useful if some python modules have some sort of module level functions that need to be called before the object get created
+
+```python
+import logging
+
+class Client
+    def __init__(self, logger: logging.Logger)
+        self.logger = logger
+
+    def do_a_thing(self):
+        self.logger.info('Doing a thing')
+
+def logger_fac(context: DependencyContext):
+    module = context.parent.implementation.__module__
+    return logging.getLogger(module)
+
+def configuring_logging():
+    logging.basicConfig()
+
+
+
+
+container = Container()
+container.register(Client)
+container.register(logging.Logger, factory=logger_fac)
+container.pre_configure(logging.Logger, configuring_logging)
+
+client = container.resolve(Client)
+
+
+```
```

### Comparing `clean_ioc-0.1.0/clean_ioc/__init__.py` & `clean_ioc-0.1.1/clean_ioc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         self.parent = dependency_node.parent
         self.decorated = dependency_node.decorated
 
 
 class DependencyGraph:
     def __init__(self, root_node: DependencyNode, resolved_object: Any):
         self.root_node = root_node
-        self.resolved_object = resolved_object
+        self.resolved_instance = resolved_object
         self.children: list[DependencyGraph] = []
 
     def add_child(self, child_graph: DependencyGraph):
         self.children.append(child_graph)
         self.root_node.add_child(child_graph.root_node)
 
 
@@ -149,15 +149,18 @@
         spaces = " "
 
         root, *rest = self.stack
 
         chain += f"\n{CannotResolveException.print_dependency(root)}\n"
 
         for item in rest:
-            chain += f"{spaces}{vertical_line}\n{spaces}{horizontal_line}{CannotResolveException.print_dependency(item)}\n"
+            printer_item = CannotResolveException.print_dependency(item)
+            chain += (
+                f"{spaces}{vertical_line}\n{spaces}{horizontal_line}{printer_item}\n"
+            )
             spaces += "     "
 
         return chain
 
     def __str__(self):
         return self.message
 
@@ -216,14 +219,18 @@
             name="__ROOT__",
             parent_implementation=RootDependency.__PARENT_ROOT__,
             service_type=service_type,
             settings=settings,
             default_value=_empty,
         )
 
+    def resolve_instance(self, context: ResolvingContext) -> DependencyGraph:
+        graph = self.resolve_dependency_graph(context)
+        return graph.resolved_instance
+
     def resolve_dependency_graph(self, context: ResolvingContext) -> DependencyGraph:
         root_node = DependencyNode(
             RootDependency, self.parent_implementation, lifespan=Lifespan.transient
         )
         resolved_object = self.resolve(context=context, depedency_node=root_node)
         return DependencyGraph(root_node=root_node, resolved_object=resolved_object)
 
@@ -298,14 +305,39 @@
         self.dependencies = {
             name: dep
             for name, dep in self.dependencies.items()
             if name != self.decorated_arg
         }
 
 
+class PreConfiguration:
+    def __init__(
+        self,
+        service_type: type,
+        pre_configuration: Callable[..., None],
+        registration_filter: RegistartionFilter,
+        dependency_config: dict[str, DependencySettings],
+    ):
+        self.service_type = service_type
+        self.pre_configuration = pre_configuration
+        self.filter = registration_filter
+        self.dependency_config = dependency_config
+
+        self.creator = ImplementationCreator(
+            creator_function=self.pre_configuration,
+            dependency_config=self.dependency_config,
+        )
+
+        self.id = str(uuid4())
+
+    def run(self, context: ResolvingContext, dependency_node: DependencyNode):
+        self.creator.create(context=context, dependency_node=dependency_node)
+        context.mark_pre_configuration_as_ran(self.id)
+
+
 class Decorator:
     def __init__(
         self,
         service_type: type,
         decorator_type: type,
         filter: RegistartionFilter,
         decorated_arg: str | None,
@@ -360,14 +392,19 @@
             service_type=self.service_type,
             implementation=self.implementation,
             lifespan=self.lifespan,
         )
 
         dependency_node.add_child(next_node)
 
+        pre_configurations = context.find_pre_configurations_that_apply(self)
+
+        for pre_configuration in pre_configurations:
+            pre_configuration.run(context, dependency_node)
+
         cached_instance = context.get_cached(self._id)
         if not cached_instance == _empty:
             return cached_instance
         built_instance = self.creator.create(context, next_node)
         decorated_node = next_node
         for dec in context.find_decorators_that_apply(self):
             next_dec_node = DependencyNode(
@@ -383,38 +420,57 @@
         return built_instance
 
 
 class Registry:
     def __init__(self):
         self._registrations: dict[type, deque[Registration]] = defaultdict(deque)
         self._decorators: dict[type, deque[Decorator]] = defaultdict(deque)
+        self._pre_configurations: dict[type, deque[PreConfiguration]] = defaultdict(
+            deque
+        )
         self._singletons: dict[str, Any] = {}
+        self._run_preconfigurations: list[str] = []
 
     def add_registration(self, registartion: Registration):
         self._registrations[registartion.service_type].appendleft(registartion)
 
     def add_decorator(self, decorator: Decorator):
         self._decorators[decorator.service_type].appendleft(decorator)
 
+    def add_pre_configuration(self, pre_configuration: PreConfiguration):
+        self._pre_configurations[pre_configuration.service_type].appendleft(
+            pre_configuration
+        )
+
     def add_singleton_instance(self, registartion_id: str, instance: Any):
         self._singletons[registartion_id] = instance
 
+    def mark_pre_configuration_as_run(self, pre_configuration_id):
+        self._run_preconfigurations.append(pre_configuration_id)
+
     def get_registartions(self, service_type: type):
         return self._registrations[service_type]
 
+    def get_pre_configurations(self, service_type: type):
+        return self._pre_configurations[service_type]
+
     def get_decorators(self, service_type: type):
         return self._decorators[service_type]
 
     def get_singleton(self, registartion_id):
         return self._singletons.get(registartion_id)
 
     @property
     def singletons(self):
         return self._singletons
 
+    @property
+    def run_pre_configurations(self):
+        return self._run_preconfigurations
+
 
 class DependencyCache:
     def __init__(self, registry: Registry, scope: Scope):
         self.registry = registry
         self.scope = scope
         self._current_items = {
             **{k: v for k, v in registry.singletons.items()},
@@ -488,20 +544,31 @@
     def find_decorators_that_apply(self, registration: Registration):
         return [
             d
             for d in self.registry.get_decorators(registration.service_type)
             if d.registartion_filter(registration)
         ]
 
+    def find_pre_configurations_that_apply(self, registration: Registration):
+        return [
+            c
+            for c in self.registry.get_pre_configurations(registration.service_type)
+            if c.id not in self.registry.run_pre_configurations
+            and c.filter(registration)
+        ]
+
     def get_cached(self, reg_id: str):
         return self._cache.get(reg_id)
 
     def new_instance_created(self, reg_id: str, instance: Any, lifespan: Lifespan):
         self._cache.put(registration_id=reg_id, instance=instance, lifespan=lifespan)
 
+    def mark_pre_configuration_as_ran(self, preconfiguration_id: str):
+        self.registry.mark_pre_configuration_as_run(preconfiguration_id)
+
 
 class Resolver(abc.ABC):
     @abc.abstractmethod
     def resolve(
         self,
         cls: type,
         filter: RegistartionFilter = _all_registartions,
@@ -660,14 +727,30 @@
 
 class Container(Resolver):
     def __init__(self):
         self.registry = Registry()
         self.register(Container, instance=self)
         self.register(Resolver, instance=self)
 
+    def pre_configure(
+        self,
+        service_type: type,
+        configuration_function: Callable[..., None],
+        registration_filter: RegistartionFilter = _all_registartions,
+        dependency_config: dict[str, DependencySettings] = {},
+    ):
+        self.registry.add_pre_configuration(
+            PreConfiguration(
+                service_type=service_type,
+                pre_configuration=configuration_function,
+                registration_filter=registration_filter,
+                dependency_config=dependency_config,
+            )
+        )
+
     def register(
         self,
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
         lifespan: Lifespan = Lifespan.once_per_graph,
@@ -716,19 +799,21 @@
             )
 
     def register_subclasses(
         self,
         base_type: type,
         lifespan: Lifespan = Lifespan.once_per_graph,
         subclass_type_filter: Callable[[type], bool] = constant(True),
+        get_registration_name: Callable[[type], str | None] = constant(None),
     ):
-        subclasses = get_subclasses(base_type, subclass_type_filter)
-
+        full_type_filter = fn_and(fn_not(is_abstract), subclass_type_filter)
+        subclasses = get_subclasses(base_type, full_type_filter)
         for sc in subclasses:
-            self.register(base_type, sc, lifespan=lifespan)
+            name = get_registration_name(sc)
+            self.register(base_type, sc, lifespan=lifespan, name=name)
             self.register(sc, lifespan=lifespan)
 
     def register_decorator(
         self,
         service_type: type,
         decorator_type: type,
         registration_filter: Callable[[Registration], bool] = _all_registartions,
@@ -758,30 +843,37 @@
             None,
         )
 
     def register_open_generic(
         self,
         generic_service_type: type,
         fallback_type: type | None = None,
+        fallback_name: str | None = None,
         lifespan: Lifespan = Lifespan.once_per_graph,
-        name: str | None = None,
         subclass_type_filter: Callable[[type], bool] = constant(True),
+        get_registration_name: Callable[[type], str | None] = constant(None),
     ):
         full_type_filter = fn_and(fn_not(is_abstract), subclass_type_filter)
         subclasses = get_subclasses(generic_service_type, full_type_filter)
         for subclass in subclasses:
+            name = get_registration_name(subclass)
             target_generic_base = self._get_target_generic_base(
                 generic_service_type, subclass
             )
             if target_generic_base:
-                self.register(target_generic_base, subclass, lifespan=lifespan)
+                self.register(
+                    target_generic_base, subclass, lifespan=lifespan, name=name
+                )
 
         if fallback_type:
             self.register(
-                generic_service_type, fallback_type, lifespan=lifespan, name=name
+                generic_service_type,
+                fallback_type,
+                lifespan=lifespan,
+                name=fallback_name,
             )
 
     def register_open_generic_decorator(
         self,
         generic_service_type: type,
         generic_decorator_type: type,
         subclass_type_filter: Callable[[type], bool] = constant(True),
@@ -825,16 +917,15 @@
         self,
         service_type,
         filter: RegistartionFilter = _all_registartions,
         scope: Scope = EmptyContainerScope(),
     ) -> Any:
         d = RootDependency(service_type, DependencySettings(filter=filter))
         context = ResolvingContext(self.registry, scope)
-        graph = d.resolve_dependency_graph(context)
-        return graph.resolved_object
+        return d.resolve_instance(context)
 
     def new_scope(
         self, ScopeClass: Type[ContainerScope] = ContainerScope, *args, **kwargs
     ) -> Scope:
         return ScopeClass(self, *args, **kwargs)
 
     def expect_to_be_scoped(self, service_type: type, name: str | None = None):
```

### Comparing `clean_ioc-0.1.0/clean_ioc/factories.py` & `clean_ioc-0.1.1/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.0/clean_ioc/functional_utils.py` & `clean_ioc-0.1.1/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.0/clean_ioc/registration_filters.py` & `clean_ioc-0.1.1/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.0/clean_ioc/type_filters.py` & `clean_ioc-0.1.1/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.0/clean_ioc/typing_utils.py` & `clean_ioc-0.1.1/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.0/pyproject.toml` & `clean_ioc-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.1.0"
+version = "0.1.1"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
```

### Comparing `clean_ioc-0.1.0/setup.py` & `clean_ioc-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['clean_ioc']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'clean-ioc',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'An IOC Container for Python 3.10+',
-    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\n\n```\n',
+    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\nclient = container.resolve(Client)\n\n\n```\n\n\n## Pre-configurations\n\nPre configurations run a side-effect for a type before the type gets resolved.\nThis is useful if some python modules have some sort of module level functions that need to be called before the object get created\n\n```python\nimport logging\n\nclass Client\n    def __init__(self, logger: logging.Logger)\n        self.logger = logger\n\n    def do_a_thing(self):\n        self.logger.info(\'Doing a thing\')\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return logging.getLogger(module)\n\ndef configuring_logging():\n    logging.basicConfig()\n\n\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(logging.Logger, factory=logger_fac)\ncontainer.pre_configure(logging.Logger, configuring_logging)\n\nclient = container.resolve(Client)\n\n\n```',
     'author': 'Peter Daly',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/peter-daly/clean_ioc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clean_ioc-0.1.0/PKG-INFO` & `clean_ioc-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.1.0
+Version: 0.1.1
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -633,22 +633,55 @@
         self.module = module
 
 class Client
     def __init__(self, logger: Logger)
         self.logger = logger
 
 def logger_fac(context: DependencyContext):
-    module = context.parent.__module__
+    module = context.parent.implementation.__module__
     return Logger(module)
 
 
 container = Container()
 container.register(Client)
 container.register(Logger, factory=logger_fac)
 
-container.apply_module(client_module)
-
 client = container.resolve(Client)
 
 
 ```
 
+
+## Pre-configurations
+
+Pre configurations run a side-effect for a type before the type gets resolved.
+This is useful if some python modules have some sort of module level functions that need to be called before the object get created
+
+```python
+import logging
+
+class Client
+    def __init__(self, logger: logging.Logger)
+        self.logger = logger
+
+    def do_a_thing(self):
+        self.logger.info('Doing a thing')
+
+def logger_fac(context: DependencyContext):
+    module = context.parent.implementation.__module__
+    return logging.getLogger(module)
+
+def configuring_logging():
+    logging.basicConfig()
+
+
+
+
+container = Container()
+container.register(Client)
+container.register(logging.Logger, factory=logger_fac)
+container.pre_configure(logging.Logger, configuring_logging)
+
+client = container.resolve(Client)
+
+
+```
```


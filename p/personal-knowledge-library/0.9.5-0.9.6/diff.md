# Comparing `tmp/personal_knowledge_library-0.9.5.tar.gz` & `tmp/personal_knowledge_library-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-0.9.5.tar", last modified: Wed Apr 26 14:53:20 2023, max compression
+gzip compressed data, was "personal_knowledge_library-0.9.6.tar", last modified: Tue May 23 09:39:46 2023, max compression
```

## Comparing `personal_knowledge_library-0.9.5.tar` & `personal_knowledge_library-0.9.6.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.522276 personal_knowledge_library-0.9.5/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.522276 personal_knowledge_library-0.9.5/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    55252 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.522276 personal_knowledge_library-0.9.5/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)   312127 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26750 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    51751 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    28407 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:53:20.526276 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 14:53:20.000000 personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 14:53:20.530277 personal_knowledge_library-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-26 14:52:55.000000 personal_knowledge_library-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    39600 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52179 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19967 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29014 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.318938 personal_knowledge_library-0.9.6/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39600 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:39:46.000000 personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 09:39:46.322938 personal_knowledge_library-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-23 09:39:29.000000 personal_knowledge_library-0.9.6/setup.py
```

### Comparing `personal_knowledge_library-0.9.5/LICENSE` & `personal_knowledge_library-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.5/PKG-INFO` & `personal_knowledge_library-0.9.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,811 +1,790 @@
-Metadata-Version: 2.1
-Name: personal_knowledge_library
-Version: 0.9.5
-Summary: Library to access Wacom's Personal Knowledge graph.
-Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
-Author: Markus Weber
-Author-email: markus.weber@wacom.com
-License: Apache 2.0 License
-Description: # Wacom Personal Knowledge Library
-        
-        The library and the cloud services are still under development. 
-        The required access tokens are only available for selected partner companies.
-        
-        > :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
-        
-        ## Introduction
-        
-        In knowledge management there is a distinction between data, information and knowledge.
-        In the domain of digital ink this means:
-        
-        - **Data** - The equivalent would be the ink strokes
-        - **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
-        - **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
-        
-        The following illustration shows the different layers of knowledge:
-        ![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
-        
-        For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
-        
-        This library provide simplified access to Wacom's personal knowledge cloud service.
-        It contains:
-        
-        - Basic datastructures for Ontology object and entities from the knowledge graph
-        - Clients for the REST APIs
-        - Connector for Wikidata public knowledge graph
-        
-        **Ontology service:**
-        
-        - List all Ontology structures
-        - Modify Ontology structures
-        - Delete Ontology structures
-        
-        **Entity service:**
-        
-        - List all entities
-        - Add entities to knowledge graph
-        - Access object properties
-        
-        # Technology stack
-        
-        ## Domain Knowledge
-        
-        The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
-        The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
-        
-        - Foundation for structured data, knowledge representation as concepts and relations among concepts
-        - Being explicit definitions of shared vocabularies for interoperability
-        - Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
-        - Can be used for problem solving
-        
-        An ontology defines (specifies) the concepts, relationships, and other distinctions that are relevant for modelling a domain.
-        
-        ## Knowledge Graph
-        
-        - Knowledge graph is generated from unstructured and structured knowledge sources
-        - Contains all structured knowledge gathered from all sources
-        - Foundation for all semantic algorithms
-        
-        ## Semantic Technology
-        
-        - Extract knowledge from various sources (Connectors)
-        - Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
-        - Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
-        
-        
-        # Functionality
-        
-        ## Access API
-        
-        The personal knowledge graph backend is implement as a multi-tenancy system.
-        Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
-        
-        ![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
-        
-        In general, a tenant with their users, groups, and entities are logically separated.
-        Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
-        
-        The user management is rather limited, each organisation must provide their own authentication service and user management.
-        The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
-        
-        The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
-        While users for each tenant can be created by the owner of the **Tenant API Key**.
-        You will receive this token from the system owner after the creation of the tenant.
-        
-        
-        > :warning: Store the **Tenant API Key** in a secure key store, as attackers can use the key to harm your system.
-        
-        
-        The **Tenant API Key** should be only used by your authentication service to create shadow users and to login your user into the WPK backend.
-        After a successful user login, you will receive a token which can be used by the user to create, update, or delete entities and relations.
-        
-        The following illustration summarizes the flows for creation of tenant and users:
-        
-        ![Tenant and user creation](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-user-creation.png)
-        
-        The organisation itself needs to implement their own authentication service which:
-        
-        - handles the users and their passwords,
-        - controls the personal data of the users,
-        - connects the users with the WPK backend and share with them the user token.
-        
-        The WPK backend only manages the access levels of the entities and the group management for users.
-        The illustration shows how the access token is received from the WPK endpoint:
-        
-        ![Access token request.](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/access-token.png)
-        
-        # Entity API
-        
-        The entities used within the knowledge graph and the relationship among them is defined within an ontology that is manage with Wacom Ontology Management System (WOMS).
-        
-        An entity within the personal knowledge graphs consist of these major parts:
-        
-        - **Icon** - a visual representation of the entity, for instance a portrait of a person.
-        - **URI** - a unique resource identifier of an entity in the graph.
-        - **Type** - the type links to the defined concept class in the ontology.
-        - **Labels** - labels are the word(s) use in a language for the concept.
-        - **Description** - a short abstract that describes the entity.
-        - **Literals** - literals are properties of an entity, such as first name of a person. The ontology defines all literals of the concept class as well as its data type.
-        - **Relations** - the relationship among different entities is described using relations.
-        
-        The following illustration provides an example for an entity:
-        
-        ![Entity description](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/entity-description.png)
-        
-        ## Entity content
-        
-        Entities in general are language-independent as across nationalities or cultures we only use different scripts and words for a shared instance of a concept.
-        
-        Let's take Leonardo da Vinci as an example.
-        The ontology defines the concept of a Person, a human being.
-        Now, in English its label would be _Leonardo da Vinci_, while in Japanese _レオナルド・ダ・ヴィンチ_.
-        Moreover, he is also known as _Leonardo di ser Piero da Vinci_ or _ダ・ビンチ_.
-        
-        ### Labels
-        
-        Now, in the given example all words that a assigned to the concept are labels.
-        The label _Leonardo da Vinci_ is stored in the backend with an additional language code, e.g. _en_.
-        
-        There is always a main label, which refers to the most common or official name of entity.
-        Another example would be Wacom, where _Wacom Co., Ltd._ is the official name while _Wacom_ is commonly used and be considered as an alias.
-        
-        >  :pushpin: For the language code the **ISO 639-1:2002**, codes for the representation of names of languages—Part 1: Alpha-2 code. Read more, [here](https://www.iso.org/standard/22109.html)
-        
-        ## Samples
-        
-        ### Entity handling
-        
-        This samples shows how to work with graph service.
-        
-        ```python
-        import argparse
-        from typing import Optional, List, Dict
-        
-        from knowledge.base.entity import LanguageCode, Description, Label
-        from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
-        from knowledge.services.graph import WacomKnowledgeService
-        
-        # ------------------------------- Knowledge entities -------------------------------------------------------------------
-        LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
-        SELF_PORTRAIT_STYLE: str = 'self-portrait'
-        ICON: str = "https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29."\
-                    "JPG/1024px-Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29.JPG"
-        # ------------------------------- Ontology class names -----------------------------------------------------------------
-        THING_OBJECT: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Thing')
-        """
-        The Ontology will contain a Thing class where is the root class in the hierarchy. 
-        """
-        ARTWORK_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'creative', 'VisualArtwork')
-        PERSON_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Person')
-        ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
-        IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
-        HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
-        CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
-        HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
-        
-        
-        def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
-            """
-            Printing entity details.
-        
-            Parameters
-            ----------
-            entity: ThingObject
-                Entity with properties
-            list_idx: int
-                Index with a list
-            auth_key: str
-                Authorization key
-            client: WacomKnowledgeService
-                Knowledge graph client
-            short: bool
-                Short summary
-            """
-            print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
-            if len(entity.label) > 0:
-                print('    | [Labels]')
-                for la in entity.label:
-                    print(f'    |     |- "{la.content}"@{la.language_code}')
-                print('    |')
-            if not short:
-                if len(entity.alias) > 0:
-                    print('    | [Alias]')
-                    for la in entity.alias:
-                        print(f'    |     |- "{la.content}"@{la.language_code}')
-                    print('    |')
-                if len(entity.data_properties) > 0:
-                    print('    | [Attributes]')
-                    for data_property, labels in entity.data_properties.items():
-                        print(f'    |    |- {data_property.iri}:')
-                        for li in labels:
-                            print(f'    |    |-- "{li.value}"@{li.language_code}')
-                    print('    |')
-        
-                relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
-                                                                                                  uri=entity.uri)
-                if len(relations_obj) > 0:
-                    print('    | [Relations]')
-                    for re in relations_obj.values():
-                        print(f'    |--- {re.relation.iri}: ')
-                        print(f'           |- [Incoming]: {re.incoming_relations} ')
-                        print(f'           |- [Outgoing]: {re.outgoing_relations}')
-                print()
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
-                                help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom personal knowledge REST API Client
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
-                                                                            service_url=args.instance)
-            # Use special tenant for testing:  Unit-test tenant
-            user_token, refresh_token, expiration_time = knowledge_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            page_id: Optional[str] = None
-            page_number: int = 1
-            entity_count: int = 0
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' First step: Find Leonardo da Vinci in the knowledge graph.')
-            print('-----------------------------------------------------------------------------------------------------------')
-            res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
-                                                                            language_code=LanguageCode('en_US'), limit=1000)
-            leo: Optional[ThingObject] = None
-            s_idx: int = 1
-            for entity in res_entities:
-                #  Entity must be a person and the label match with full string
-                if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
-                    leo = entity
-                    break
-        
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' What artwork exists in the knowledge graph.')
-            print('-----------------------------------------------------------------------------------------------------------')
-            relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
-                                                                                                         uri=leo.uri)
-            print(f' Artwork of {leo.label}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            idx: int = 1
-            if CREATED in relations_dict:
-                for e in relations_dict[CREATED].outgoing_relations:
-                    print(f' [{idx}] {e.uri}: {e.label}')
-                    idx += 1
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' Let us create a new piece of artwork.')
-            print('-----------------------------------------------------------------------------------------------------------')
-        
-            # Main labels for entity
-            artwork_labels: List[Label] = [
-                Label('Ginevra Gherardini', LanguageCode('en_US')),
-                Label('Ginevra Gherardini', LanguageCode('de_DE'))
-            ]
-            # Alias labels for entity
-            artwork_alias: List[Label] = [
-                Label("Ginevra", LanguageCode('en_US')),
-                Label("Ginevra", LanguageCode('de_DE'))
-            ]
-            # Topic description
-            artwork_description: List[Description] = [
-                Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
-                Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
-            ]
-            # Topic
-            artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
-                                                      description=artwork_description,
-                                                      icon=ICON)
-            artwork_object.alias = artwork_alias
-            print(f' Create: {artwork_object}')
-            # Create artwork
-            artwork_entity_uri: str = knowledge_client.create_entity(user_token, artwork_object)
-            print(f' Entity URI: {artwork_entity_uri}')
-            # Create relation between Leonardo da Vinci and artwork
-            knowledge_client.create_relation(auth_key=user_token, source=leo.uri, relation=IS_CREATOR,
-                                             target=artwork_entity_uri)
-        
-            relations_dict = knowledge_client.relations(auth_key=user_token, uri=artwork_entity_uri)
-            for ontology_property, object_property in relations_dict.items():
-                print(f'  {object_property}')
-            # You will see that wacom:core#isCreatedBy is automatically inferred as relation as it is the inverse property of
-            # wacom:core#created.
-        
-            # Now, more search options
-            res_entities, next_search_page = knowledge_client.search_description(user_token, 'Michelangelo\'s Sistine Chapel',
-                                                                                 LanguageCode('en_US'), limit=1000)
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' Search results.  Description: "Michelangelo\'s Sistine Chapel"')
-            print('-----------------------------------------------------------------------------------------------------------')
-            s_idx: int = 1
-            for e in res_entities:
-                print_entity(e, s_idx, user_token, knowledge_client)
-        
-            # Now, let's search all artwork that has the art style self-portrait
-            res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token,
-                                                                            search_term=SELF_PORTRAIT_STYLE,
-                                                                            language_code=LanguageCode('en_US'), limit=1000)
-            art_style: Optional[ThingObject] = None
-            s_idx: int = 1
-            for entity in res_entities:
-                #  Entity must be a person and the label match with full string
-                if entity.concept_type == ART_STYLE_CLASS and SELF_PORTRAIT_STYLE in [l.content for l in entity.label]:
-                    art_style = entity
-                    break
-            res_entities, next_search_page = knowledge_client.search_relation(auth_key=user_token,
-                                                                              subject_uri=None,
-                                                                              relation=HAS_ART_STYLE,
-                                                                              object_uri=art_style.uri,
-                                                                              language_code=LanguageCode('en_US'))
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' Search results.  Relation: relation:=has_topic  object_uri:= unknown')
-            print('-----------------------------------------------------------------------------------------------------------')
-            s_idx: int = 1
-            for e in res_entities:
-                print_entity(e, s_idx, user_token, knowledge_client, short=True)
-                s_idx += 1
-        
-            # Finally, the activation function retrieving the related identities to a pre-defined depth.
-            entities, relations = knowledge_client.activations(auth_key=user_token,
-                                                               uris=[leo.uri],
-                                                               depth=1)
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(f'Activation.  URI: {leo.uri}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            s_idx: int = 1
-            for e in res_entities:
-                print_entity(e, s_idx, user_token, knowledge_client)
-                s_idx += 1
-            # All relations
-            print('-----------------------------------------------------------------------------------------------------------')
-            for r in relations:
-                print(f'Subject: {r[0]} Predicate: {r[1]} Object: {r[2]}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            page_id = None
-        
-            # Listing all entities which have the type
-            idx: int = 1
-            while True:
-                # pull
-                entities, total_number, next_page_id = knowledge_client.listing(user_token, ART_STYLE_CLASS, page_id=page_id,
-                                                                                limit=100)
-                pulled_entities: int = len(entities)
-                entity_count += pulled_entities
-                print('-------------------------------------------------------------------------------------------------------')
-                print(f' Page: {page_number} Number of entities: {len(entities)}  ({entity_count}/{total_number}) '
-                      f'Next page id: {next_page_id}')
-                print('-------------------------------------------------------------------------------------------------------')
-                for e in entities:
-                    print_entity(e, idx, user_token, knowledge_client)
-                    idx += 1
-                if pulled_entities == 0:
-                    break
-                page_number += 1
-                page_id = next_page_id
-            print()
-            # Delete all personal entities for this user
-            while True:
-                # pull
-                entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
-                                                                                limit=100)
-                pulled_entities: int = len(entities)
-                if pulled_entities == 0:
-                    break
-                delete_uris: List[str] = [e.uri for e in entities]
-                print(f'Cleanup. Delete entities: {delete_uris}')
-                knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
-                page_number += 1
-                page_id = next_page_id
-            print('-----------------------------------------------------------------------------------------------------------')
-        ```
-        
-        ### Named Entity Linking 
-        
-        Performing Named Entity Linking (NEL) on text and Universal Ink Model.
-        
-        ```python
-        import argparse
-        from typing import List, Dict
-        
-        from knowledge.base.entity import LanguageCode
-        from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
-        from knowledge.nel.base import KnowledgeGraphEntity
-        from knowledge.nel.engine import WacomEntityLinkingEngine
-        from knowledge.services.graph import WacomKnowledgeService
-        
-        LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
-        TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
-        
-        
-        def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
-            """
-            Printing entity details.
-        
-            Parameters
-            ----------
-            entity: KnowledgeGraphEntity
-                Named entity
-            list_idx: int
-                Index with a list
-            auth_key: str
-                Authorization key
-            client: WacomKnowledgeService
-                Knowledge graph client
-            """
-            thing: ThingObject = knowledge_client.entity(auth_key=user_token, uri=entity.entity_source.uri)
-            print(f'[{list_idx}] - {e.ref_text} [{e.start_idx}-{e.end_idx}] : {thing.uri} <{thing.concept_type.iri}>')
-            if len(thing.label) > 0:
-                print('    | [Labels]')
-                for la in thing.label:
-                    print(f'    |     |- "{la.content}"@{la.language_code}')
-                print('    |')
-            if len(thing.label) > 0:
-                print('    | [Alias]')
-                for la in thing.alias:
-                    print(f'    |     |- "{la.content}"@{la.language_code}')
-                print('    |')
-            relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
-            if len(thing.data_properties) > 0:
-                print('    | [Attributes]')
-                for data_property, labels in thing.data_properties.items():
-                    print(f'    |    |- {data_property.iri}:')
-                    for li in labels:
-                        print(f'    |    |-- "{li.value}"@{li.language_code}')
-                print('    |')
-            if len(relations) > 0:
-                print('    | [Relations]')
-                for re in relations.values():
-                    print(f'    |--- {re.relation.iri}: ')
-                    print(f'           |- [Incoming]: {re.incoming_relations} ')
-                    print(f'           |- [Outgoing]: {re.outgoing_relations}')
-            print()
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom personal knowledge REST API Client
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
-                application_name="Named Entity Linking Knowledge access",
-                service_url=args.instance)
-            #  Wacom Named Entity Linking
-            nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
-                service_url=args.instance,
-                service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
-            )
-            # Use special tenant for testing:  Unit-test tenant
-            user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            entities: List[KnowledgeGraphEntity] = nel_client.\
-                link_personal_entities(auth_key=user_token, text=TEXT,
-                                       language_code=LANGUAGE_CODE)
-            idx: int = 1
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            for e in entities:
-                print_entity(e, idx, user_token, knowledge_client)
-                idx += 1
-        
-        ```
-        
-        ### Access Management
-        
-        The sample shows, how access to entities can be shared with a group of users or the tenant.
-        
-        ```python
-        import argparse
-        from typing import List
-        from knowledge.base.entity import LanguageCode, Label, Description
-        from knowledge.base.ontology import OntologyClassReference, ThingObject
-        from knowledge.services.base import WacomServiceException
-        from knowledge.services.graph import WacomKnowledgeService
-        from knowledge.services.group import GroupManagementServiceAPI, Group
-        from knowledge.services.users import UserManagementServiceAPI
-        
-        # ------------------------------- User credential ----------------------------------------------------------------------
-        TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
-        
-        
-        def create_entity() -> ThingObject:
-            # Main labels for entity
-            topic_labels: List[Label] = [
-                Label('Hidden', LanguageCode('en_US')),
-                Label('Versteckt', LanguageCode('de_DE')),
-                Label('隠れた', LanguageCode('ja_JP'))
-            ]
-        
-            # Topic description
-            topic_description: List[Description] = [
-                Description('Hidden entity to explain access management.', LanguageCode('en_US')),
-                Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
-            ]
-            # Topic
-            topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
-            return topic_object
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
-                                help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom personal knowledge REST API Client
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
-                                                                            service_url=args.instance)
-            # User Management
-            user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
-            # Group Management
-            group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
-            admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            # Now, we create a users
-            u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
-            u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
-            u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
-        
-            # Now, let's create an entity
-            thing: ThingObject = create_entity()
-            entity_uri: str = knowledge_client.create_entity(u1_token, thing)
-            # Only user 1 can access the entity from cloud storage
-            my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
-            print(f'User is the owner of {my_thing.owner}')
-            # Now only user 1 has access to the personal entity
-            knowledge_client.entity(u1_token, entity_uri)
-            # Try to access the entity
-            try:
-                knowledge_client.entity(u2_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
-            # Try to access the entity
-            try:
-                knowledge_client.entity(u3_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 3 has no access to the personal entity of user 1. Exception: {we}")
-            # Now, user 1 creates a group
-            g: Group = group_management.create_group(u1_token, "test-group")
-            # Shares the join key with user 2 and user 2 joins
-            group_management.join_group(u2_token, g.id, g.join_key)
-            # Share entity with group
-            group_management.add_entity_to_group(u1_token, g.id, entity_uri)
-            # Now, user 2 should have access
-            other_thing: ThingObject = knowledge_client.entity(u2_token, entity_uri)
-            print(f'User 2 is the owner of the thing: {other_thing.owner}')
-            # Try to access the entity
-            try:
-                knowledge_client.entity(u3_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 3 still has no access to the personal entity of user 1. Exception: {we}")
-            # Un-share the entity
-            group_management.remove_entity_to_group(u1_token, g.id, entity_uri)
-            # Now, again no access
-            try:
-                knowledge_client.entity(u2_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
-            group_management.leave_group(u2_token, group_id=g.id)
-            # Now, share the entity with the whole tenant
-            my_thing.tenant_access_right.read = True
-            knowledge_client.update_entity(u1_token, my_thing)
-            # Now, all users can access the entity
-            knowledge_client.entity(u2_token, entity_uri)
-            knowledge_client.entity(u3_token, entity_uri)
-            # Finally, clean up
-            knowledge_client.delete_entity(u1_token, entity_uri, force=True)
-            # Remove users
-            user_management.delete_user(TENANT_KEY, u1.external_user_id, u1.id)
-            user_management.delete_user(TENANT_KEY, u2.external_user_id, u2.id)
-            user_management.delete_user(TENANT_KEY, u3.external_user_id, u3.id)
-        
-        ```
-        
-        ### Ontology Creation
-        
-        The samples show how the ontology can be extended and new entities can be added using the added classes.
-        
-        ```python
-        import argparse
-        from typing import List, Optional
-        
-        from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
-        from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
-            DataProperty
-        from knowledge.services.graph import WacomKnowledgeService
-        from knowledge.services.ontology import OntologyService
-        
-        # ------------------------------- Constants ----------------------------------------------------------------------------
-        LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
-        CONTEXT_NAME: str = 'core'
-        # Wacom Base Ontology Types
-        PERSON_TYPE: OntologyClassReference = OntologyClassReference.parse("wacom:core#Person")
-        # Demo Class
-        ARTIST_TYPE: OntologyClassReference = OntologyClassReference.parse("demo:creative#Artist")
-        # Demo Object property
-        IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
-        # Demo Data property
-        STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
-        
-        
-        def create_artist() -> ThingObject:
-            # Main labels for entity
-            topic_labels: List[Label] = [
-                Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
-            ]
-        
-            # Topic description
-            topic_description: List[Description] = [
-                Description('Hidden entity to explain access management.', LanguageCode('en_US')),
-                Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
-            ]
-        
-            data_property: DataProperty = DataProperty(content='Salaj',
-                                                       property_ref=STAGE_NAME,
-                                                       language_code=LanguageCode('en_US'))
-            # Topic
-            artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
-            artist.add_data_property(data_property)
-            return artist
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom Ontology REST API Client
-            ontology_client: OntologyService = OntologyService(service_url=args.instance)
-            admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
-                application_name="Ontology Creation Demo",
-                service_url=args.instance)
-            contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
-            if len(contexts) == 0:
-                # First, create a context for the ontology
-                ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
-                context_name: str = CONTEXT_NAME
-            else:
-                context_name: str = contexts[0].context
-            # Creating a class which is a subclass of a person
-            ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
-        
-            # Object properties
-            ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                                   reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
-                                                   ranges_cls=[PERSON_TYPE],
-                                                   inverse_of=None, subproperty_of=None)
-            # Data properties
-            ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                                 reference=STAGE_NAME,
-                                                 domains_cls=[ARTIST_TYPE],
-                                                 ranges_cls=[DataPropertyType.STRING],
-                                                 subproperty_of=None)
-        
-            # Commit the changes of the ontology. This is very important to confirm changes.
-            ontology_client.commit(admin_token, CONTEXT_NAME)
-            # Trigger graph service. After the update the ontology is available and the new entities can be created
-            knowledge_client.ontology_update(admin_token)
-        
-            res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
-                                                                            language_code=LanguageCode('en_US'), limit=1000)
-            leo: Optional[ThingObject] = None
-            for entity in res_entities:
-                #  Entity must be a person and the label match with full string
-                if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
-                    leo = entity
-                    break
-        
-            artist_student: ThingObject = create_artist()
-            artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
-            knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
-        ```
-        
-        ## Tools
-        
-        The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
-        
-        ### Listing script
-        
-        Listing the entities for tenant. 
-        
-        ```bash
-        >> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-r, --relations (optional)_ -  Requesting the relations for each entity
-        
-        ### Export entities script
-        
-        Dump all entities of a user to a ndjson file. 
-        
-        ```bash
-        >> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
-                                knowledge.wacom.com)
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-r, --relations (optional)_ -  Requesting the relations for each entity
-        - _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
-        - _-p, --images (optional)_ - Include the images in the dump.
-        - _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
-         
-        ### Push entities script
-        
-        Pushing entities to knowledge graph.
-        
-        ```bash
-        >> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
-          
-        ### Reset
-        
-        Resets a tenant by removing entities, groups, and users. 
-        
-        ```bash
-        >> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
-          
-        # Documentation
-        
-        You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
-        API documentation is available [here](./docs/).
-        
-        ## Contributing
-        Contribution guidelines are still work in progress.
-        
-        ## License
-        [Apache License 2.0](LICENSE)
-        
-Keywords: semantic-knowledge;knowledge-graph
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown
+# Wacom Personal Knowledge Library
+
+The library and the cloud services are still under development. 
+The required access tokens are only available for selected partner companies.
+
+> :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
+
+## Introduction
+
+In knowledge management there is a distinction between data, information and knowledge.
+In the domain of digital ink this means:
+
+- **Data** - The equivalent would be the ink strokes
+- **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
+- **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
+
+The following illustration shows the different layers of knowledge:
+![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
+
+For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
+
+This library provide simplified access to Wacom's personal knowledge cloud service.
+It contains:
+
+- Basic datastructures for Ontology object and entities from the knowledge graph
+- Clients for the REST APIs
+- Connector for Wikidata public knowledge graph
+
+**Ontology service:**
+
+- List all Ontology structures
+- Modify Ontology structures
+- Delete Ontology structures
+
+**Entity service:**
+
+- List all entities
+- Add entities to knowledge graph
+- Access object properties
+
+# Technology stack
+
+## Domain Knowledge
+
+The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
+The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
+
+- Foundation for structured data, knowledge representation as concepts and relations among concepts
+- Being explicit definitions of shared vocabularies for interoperability
+- Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
+- Can be used for problem solving
+
+An ontology defines (specifies) the concepts, relationships, and other distinctions that are relevant for modelling a domain.
+
+## Knowledge Graph
+
+- Knowledge graph is generated from unstructured and structured knowledge sources
+- Contains all structured knowledge gathered from all sources
+- Foundation for all semantic algorithms
+
+## Semantic Technology
+
+- Extract knowledge from various sources (Connectors)
+- Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
+- Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
+
+
+# Functionality
+
+## Access API
+
+The personal knowledge graph backend is implement as a multi-tenancy system.
+Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
+
+![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
+
+In general, a tenant with their users, groups, and entities are logically separated.
+Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
+
+The user management is rather limited, each organisation must provide their own authentication service and user management.
+The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
+
+The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
+While users for each tenant can be created by the owner of the **Tenant API Key**.
+You will receive this token from the system owner after the creation of the tenant.
+
+
+> :warning: Store the **Tenant API Key** in a secure key store, as attackers can use the key to harm your system.
+
+
+The **Tenant API Key** should be only used by your authentication service to create shadow users and to login your user into the WPK backend.
+After a successful user login, you will receive a token which can be used by the user to create, update, or delete entities and relations.
+
+The following illustration summarizes the flows for creation of tenant and users:
+
+![Tenant and user creation](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-user-creation.png)
+
+The organisation itself needs to implement their own authentication service which:
+
+- handles the users and their passwords,
+- controls the personal data of the users,
+- connects the users with the WPK backend and share with them the user token.
+
+The WPK backend only manages the access levels of the entities and the group management for users.
+The illustration shows how the access token is received from the WPK endpoint:
+
+![Access token request.](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/access-token.png)
+
+# Entity API
+
+The entities used within the knowledge graph and the relationship among them is defined within an ontology that is manage with Wacom Ontology Management System (WOMS).
+
+An entity within the personal knowledge graphs consist of these major parts:
+
+- **Icon** - a visual representation of the entity, for instance a portrait of a person.
+- **URI** - a unique resource identifier of an entity in the graph.
+- **Type** - the type links to the defined concept class in the ontology.
+- **Labels** - labels are the word(s) use in a language for the concept.
+- **Description** - a short abstract that describes the entity.
+- **Literals** - literals are properties of an entity, such as first name of a person. The ontology defines all literals of the concept class as well as its data type.
+- **Relations** - the relationship among different entities is described using relations.
+
+The following illustration provides an example for an entity:
+
+![Entity description](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/entity-description.png)
+
+## Entity content
+
+Entities in general are language-independent as across nationalities or cultures we only use different scripts and words for a shared instance of a concept.
+
+Let's take Leonardo da Vinci as an example.
+The ontology defines the concept of a Person, a human being.
+Now, in English its label would be _Leonardo da Vinci_, while in Japanese _レオナルド・ダ・ヴィンチ_.
+Moreover, he is also known as _Leonardo di ser Piero da Vinci_ or _ダ・ビンチ_.
+
+### Labels
+
+Now, in the given example all words that a assigned to the concept are labels.
+The label _Leonardo da Vinci_ is stored in the backend with an additional language code, e.g. _en_.
+
+There is always a main label, which refers to the most common or official name of entity.
+Another example would be Wacom, where _Wacom Co., Ltd._ is the official name while _Wacom_ is commonly used and be considered as an alias.
+
+>  :pushpin: For the language code the **ISO 639-1:2002**, codes for the representation of names of languages—Part 1: Alpha-2 code. Read more, [here](https://www.iso.org/standard/22109.html)
+
+## Samples
+
+### Entity handling
+
+This samples shows how to work with graph service.
+
+```python
+import argparse
+from typing import Optional, List, Dict
+
+from knowledge.base.entity import LanguageCode, Description, Label
+from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
+from knowledge.services.graph import WacomKnowledgeService
+
+# ------------------------------- Knowledge entities -------------------------------------------------------------------
+LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
+SELF_PORTRAIT_STYLE: str = 'self-portrait'
+ICON: str = "https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29."\
+            "JPG/1024px-Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29.JPG"
+# ------------------------------- Ontology class names -----------------------------------------------------------------
+THING_OBJECT: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Thing')
+"""
+The Ontology will contain a Thing class where is the root class in the hierarchy. 
+"""
+ARTWORK_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'creative', 'VisualArtwork')
+PERSON_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Person')
+ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
+IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
+HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
+CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
+HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
+
+
+def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
+    """
+    Printing entity details.
+
+    Parameters
+    ----------
+    entity: ThingObject
+        Entity with properties
+    list_idx: int
+        Index with a list
+    auth_key: str
+        Authorization key
+    client: WacomKnowledgeService
+        Knowledge graph client
+    short: bool
+        Short summary
+    """
+    print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
+    if len(entity.label) > 0:
+        print('    | [Labels]')
+        for la in entity.label:
+            print(f'    |     |- "{la.content}"@{la.language_code}')
+        print('    |')
+    if not short:
+        if len(entity.alias) > 0:
+            print('    | [Alias]')
+            for la in entity.alias:
+                print(f'    |     |- "{la.content}"@{la.language_code}')
+            print('    |')
+        if len(entity.data_properties) > 0:
+            print('    | [Attributes]')
+            for data_property, labels in entity.data_properties.items():
+                print(f'    |    |- {data_property.iri}:')
+                for li in labels:
+                    print(f'    |    |-- "{li.value}"@{li.language_code}')
+            print('    |')
+
+        relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
+                                                                                          uri=entity.uri)
+        if len(relations_obj) > 0:
+            print('    | [Relations]')
+            for re in relations_obj.values():
+                print(f'    |--- {re.relation.iri}: ')
+                print(f'           |- [Incoming]: {re.incoming_relations} ')
+                print(f'           |- [Outgoing]: {re.outgoing_relations}')
+        print()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+                        help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom personal knowledge REST API Client
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
+                                                                    service_url=args.instance)
+    # Use special tenant for testing:  Unit-test tenant
+    user_token, refresh_token, expiration_time = knowledge_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    page_id: Optional[str] = None
+    page_number: int = 1
+    entity_count: int = 0
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' First step: Find Leonardo da Vinci in the knowledge graph.')
+    print('-----------------------------------------------------------------------------------------------------------')
+    res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
+                                                                    language_code=LanguageCode('en_US'), limit=1000)
+    leo: Optional[ThingObject] = None
+    s_idx: int = 1
+    for entity in res_entities:
+        #  Entity must be a person and the label match with full string
+        if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
+            leo = entity
+            break
+
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' What artwork exists in the knowledge graph.')
+    print('-----------------------------------------------------------------------------------------------------------')
+    relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
+                                                                                                 uri=leo.uri)
+    print(f' Artwork of {leo.label}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    idx: int = 1
+    if CREATED in relations_dict:
+        for e in relations_dict[CREATED].outgoing_relations:
+            print(f' [{idx}] {e.uri}: {e.label}')
+            idx += 1
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' Let us create a new piece of artwork.')
+    print('-----------------------------------------------------------------------------------------------------------')
+
+    # Main labels for entity
+    artwork_labels: List[Label] = [
+        Label('Ginevra Gherardini', LanguageCode('en_US')),
+        Label('Ginevra Gherardini', LanguageCode('de_DE'))
+    ]
+    # Alias labels for entity
+    artwork_alias: List[Label] = [
+        Label("Ginevra", LanguageCode('en_US')),
+        Label("Ginevra", LanguageCode('de_DE'))
+    ]
+    # Topic description
+    artwork_description: List[Description] = [
+        Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
+        Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
+    ]
+    # Topic
+    artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
+                                              description=artwork_description,
+                                              icon=ICON)
+    artwork_object.alias = artwork_alias
+    print(f' Create: {artwork_object}')
+    # Create artwork
+    artwork_entity_uri: str = knowledge_client.create_entity(user_token, artwork_object)
+    print(f' Entity URI: {artwork_entity_uri}')
+    # Create relation between Leonardo da Vinci and artwork
+    knowledge_client.create_relation(auth_key=user_token, source=leo.uri, relation=IS_CREATOR,
+                                     target=artwork_entity_uri)
+
+    relations_dict = knowledge_client.relations(auth_key=user_token, uri=artwork_entity_uri)
+    for ontology_property, object_property in relations_dict.items():
+        print(f'  {object_property}')
+    # You will see that wacom:core#isCreatedBy is automatically inferred as relation as it is the inverse property of
+    # wacom:core#created.
+
+    # Now, more search options
+    res_entities, next_search_page = knowledge_client.search_description(user_token, 'Michelangelo\'s Sistine Chapel',
+                                                                         LanguageCode('en_US'), limit=1000)
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' Search results.  Description: "Michelangelo\'s Sistine Chapel"')
+    print('-----------------------------------------------------------------------------------------------------------')
+    s_idx: int = 1
+    for e in res_entities:
+        print_entity(e, s_idx, user_token, knowledge_client)
+
+    # Now, let's search all artwork that has the art style self-portrait
+    res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token,
+                                                                    search_term=SELF_PORTRAIT_STYLE,
+                                                                    language_code=LanguageCode('en_US'), limit=1000)
+    art_style: Optional[ThingObject] = None
+    s_idx: int = 1
+    for entity in res_entities:
+        #  Entity must be a person and the label match with full string
+        if entity.concept_type == ART_STYLE_CLASS and SELF_PORTRAIT_STYLE in [l.content for l in entity.label]:
+            art_style = entity
+            break
+    res_entities, next_search_page = knowledge_client.search_relation(auth_key=user_token,
+                                                                      subject_uri=None,
+                                                                      relation=HAS_ART_STYLE,
+                                                                      object_uri=art_style.uri,
+                                                                      language_code=LanguageCode('en_US'))
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' Search results.  Relation: relation:=has_topic  object_uri:= unknown')
+    print('-----------------------------------------------------------------------------------------------------------')
+    s_idx: int = 1
+    for e in res_entities:
+        print_entity(e, s_idx, user_token, knowledge_client, short=True)
+        s_idx += 1
+
+    # Finally, the activation function retrieving the related identities to a pre-defined depth.
+    entities, relations = knowledge_client.activations(auth_key=user_token,
+                                                       uris=[leo.uri],
+                                                       depth=1)
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(f'Activation.  URI: {leo.uri}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    s_idx: int = 1
+    for e in res_entities:
+        print_entity(e, s_idx, user_token, knowledge_client)
+        s_idx += 1
+    # All relations
+    print('-----------------------------------------------------------------------------------------------------------')
+    for r in relations:
+        print(f'Subject: {r[0]} Predicate: {r[1]} Object: {r[2]}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    page_id = None
+
+    # Listing all entities which have the type
+    idx: int = 1
+    while True:
+        # pull
+        entities, total_number, next_page_id = knowledge_client.listing(user_token, ART_STYLE_CLASS, page_id=page_id,
+                                                                        limit=100)
+        pulled_entities: int = len(entities)
+        entity_count += pulled_entities
+        print('-------------------------------------------------------------------------------------------------------')
+        print(f' Page: {page_number} Number of entities: {len(entities)}  ({entity_count}/{total_number}) '
+              f'Next page id: {next_page_id}')
+        print('-------------------------------------------------------------------------------------------------------')
+        for e in entities:
+            print_entity(e, idx, user_token, knowledge_client)
+            idx += 1
+        if pulled_entities == 0:
+            break
+        page_number += 1
+        page_id = next_page_id
+    print()
+    # Delete all personal entities for this user
+    while True:
+        # pull
+        entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
+                                                                        limit=100)
+        pulled_entities: int = len(entities)
+        if pulled_entities == 0:
+            break
+        delete_uris: List[str] = [e.uri for e in entities]
+        print(f'Cleanup. Delete entities: {delete_uris}')
+        knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
+        page_number += 1
+        page_id = next_page_id
+    print('-----------------------------------------------------------------------------------------------------------')
+```
+
+### Named Entity Linking 
+
+Performing Named Entity Linking (NEL) on text and Universal Ink Model.
+
+```python
+import argparse
+from typing import List, Dict
+
+from knowledge.base.entity import LanguageCode
+from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
+from knowledge.nel.base import KnowledgeGraphEntity
+from knowledge.nel.engine import WacomEntityLinkingEngine
+from knowledge.services.graph import WacomKnowledgeService
+
+LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
+TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
+
+
+def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
+    """
+    Printing entity details.
+
+    Parameters
+    ----------
+    entity: KnowledgeGraphEntity
+        Named entity
+    list_idx: int
+        Index with a list
+    auth_key: str
+        Authorization key
+    client: WacomKnowledgeService
+        Knowledge graph client
+    """
+    thing: ThingObject = knowledge_client.entity(auth_key=user_token, uri=entity.entity_source.uri)
+    print(f'[{list_idx}] - {e.ref_text} [{e.start_idx}-{e.end_idx}] : {thing.uri} <{thing.concept_type.iri}>')
+    if len(thing.label) > 0:
+        print('    | [Labels]')
+        for la in thing.label:
+            print(f'    |     |- "{la.content}"@{la.language_code}')
+        print('    |')
+    if len(thing.label) > 0:
+        print('    | [Alias]')
+        for la in thing.alias:
+            print(f'    |     |- "{la.content}"@{la.language_code}')
+        print('    |')
+    relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
+    if len(thing.data_properties) > 0:
+        print('    | [Attributes]')
+        for data_property, labels in thing.data_properties.items():
+            print(f'    |    |- {data_property.iri}:')
+            for li in labels:
+                print(f'    |    |-- "{li.value}"@{li.language_code}')
+        print('    |')
+    if len(relations) > 0:
+        print('    | [Relations]')
+        for re in relations.values():
+            print(f'    |--- {re.relation.iri}: ')
+            print(f'           |- [Incoming]: {re.incoming_relations} ')
+            print(f'           |- [Outgoing]: {re.outgoing_relations}')
+    print()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom personal knowledge REST API Client
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
+        application_name="Named Entity Linking Knowledge access",
+        service_url=args.instance)
+    #  Wacom Named Entity Linking
+    nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
+        service_url=args.instance,
+        service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
+    )
+    # Use special tenant for testing:  Unit-test tenant
+    user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    entities: List[KnowledgeGraphEntity] = nel_client.\
+        link_personal_entities(auth_key=user_token, text=TEXT,
+                               language_code=LANGUAGE_CODE)
+    idx: int = 1
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    for e in entities:
+        print_entity(e, idx, user_token, knowledge_client)
+        idx += 1
+
+```
+
+### Access Management
+
+The sample shows, how access to entities can be shared with a group of users or the tenant.
+
+```python
+import argparse
+from typing import List
+from knowledge.base.entity import LanguageCode, Label, Description
+from knowledge.base.ontology import OntologyClassReference, ThingObject
+from knowledge.services.base import WacomServiceException
+from knowledge.services.graph import WacomKnowledgeService
+from knowledge.services.group import GroupManagementServiceAPI, Group
+from knowledge.services.users import UserManagementServiceAPI
+
+# ------------------------------- User credential ----------------------------------------------------------------------
+TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
+
+
+def create_entity() -> ThingObject:
+    # Main labels for entity
+    topic_labels: List[Label] = [
+        Label('Hidden', LanguageCode('en_US')),
+        Label('Versteckt', LanguageCode('de_DE')),
+        Label('隠れた', LanguageCode('ja_JP'))
+    ]
+
+    # Topic description
+    topic_description: List[Description] = [
+        Description('Hidden entity to explain access management.', LanguageCode('en_US')),
+        Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
+    ]
+    # Topic
+    topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
+    return topic_object
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+                        help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom personal knowledge REST API Client
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
+                                                                    service_url=args.instance)
+    # User Management
+    user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
+    # Group Management
+    group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
+    admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    # Now, we create a users
+    u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
+    u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
+    u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
+
+    # Now, let's create an entity
+    thing: ThingObject = create_entity()
+    entity_uri: str = knowledge_client.create_entity(u1_token, thing)
+    # Only user 1 can access the entity from cloud storage
+    my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
+    print(f'User is the owner of {my_thing.owner}')
+    # Now only user 1 has access to the personal entity
+    knowledge_client.entity(u1_token, entity_uri)
+    # Try to access the entity
+    try:
+        knowledge_client.entity(u2_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
+    # Try to access the entity
+    try:
+        knowledge_client.entity(u3_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 3 has no access to the personal entity of user 1. Exception: {we}")
+    # Now, user 1 creates a group
+    g: Group = group_management.create_group(u1_token, "test-group")
+    # Shares the join key with user 2 and user 2 joins
+    group_management.join_group(u2_token, g.id, g.join_key)
+    # Share entity with group
+    group_management.add_entity_to_group(u1_token, g.id, entity_uri)
+    # Now, user 2 should have access
+    other_thing: ThingObject = knowledge_client.entity(u2_token, entity_uri)
+    print(f'User 2 is the owner of the thing: {other_thing.owner}')
+    # Try to access the entity
+    try:
+        knowledge_client.entity(u3_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 3 still has no access to the personal entity of user 1. Exception: {we}")
+    # Un-share the entity
+    group_management.remove_entity_to_group(u1_token, g.id, entity_uri)
+    # Now, again no access
+    try:
+        knowledge_client.entity(u2_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
+    group_management.leave_group(u2_token, group_id=g.id)
+    # Now, share the entity with the whole tenant
+    my_thing.tenant_access_right.read = True
+    knowledge_client.update_entity(u1_token, my_thing)
+    # Now, all users can access the entity
+    knowledge_client.entity(u2_token, entity_uri)
+    knowledge_client.entity(u3_token, entity_uri)
+    # Finally, clean up
+    knowledge_client.delete_entity(u1_token, entity_uri, force=True)
+    # Remove users
+    user_management.delete_user(TENANT_KEY, u1.external_user_id, u1.id)
+    user_management.delete_user(TENANT_KEY, u2.external_user_id, u2.id)
+    user_management.delete_user(TENANT_KEY, u3.external_user_id, u3.id)
+
+```
+
+### Ontology Creation
+
+The samples show how the ontology can be extended and new entities can be added using the added classes.
+
+```python
+import argparse
+from typing import List, Optional
+
+from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
+from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
+    DataProperty
+from knowledge.services.graph import WacomKnowledgeService
+from knowledge.services.ontology import OntologyService
+
+# ------------------------------- Constants ----------------------------------------------------------------------------
+LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
+CONTEXT_NAME: str = 'core'
+# Wacom Base Ontology Types
+PERSON_TYPE: OntologyClassReference = OntologyClassReference.parse("wacom:core#Person")
+# Demo Class
+ARTIST_TYPE: OntologyClassReference = OntologyClassReference.parse("demo:creative#Artist")
+# Demo Object property
+IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
+# Demo Data property
+STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
+
+
+def create_artist() -> ThingObject:
+    # Main labels for entity
+    topic_labels: List[Label] = [
+        Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
+    ]
+
+    # Topic description
+    topic_description: List[Description] = [
+        Description('Hidden entity to explain access management.', LanguageCode('en_US')),
+        Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
+    ]
+
+    data_property: DataProperty = DataProperty(content='Salaj',
+                                               property_ref=STAGE_NAME,
+                                               language_code=LanguageCode('en_US'))
+    # Topic
+    artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
+    artist.add_data_property(data_property)
+    return artist
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom Ontology REST API Client
+    ontology_client: OntologyService = OntologyService(service_url=args.instance)
+    admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
+        application_name="Ontology Creation Demo",
+        service_url=args.instance)
+    contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
+    if len(contexts) == 0:
+        # First, create a context for the ontology
+        ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
+        context_name: str = CONTEXT_NAME
+    else:
+        context_name: str = contexts[0].context
+    # Creating a class which is a subclass of a person
+    ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
+
+    # Object properties
+    ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
+                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
+                                           ranges_cls=[PERSON_TYPE],
+                                           inverse_of=None, subproperty_of=None)
+    # Data properties
+    ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
+                                         reference=STAGE_NAME,
+                                         domains_cls=[ARTIST_TYPE],
+                                         ranges_cls=[DataPropertyType.STRING],
+                                         subproperty_of=None)
+
+    # Commit the changes of the ontology. This is very important to confirm changes.
+    ontology_client.commit(admin_token, CONTEXT_NAME)
+    # Trigger graph service. After the update the ontology is available and the new entities can be created
+    knowledge_client.ontology_update(admin_token)
+
+    res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
+                                                                    language_code=LanguageCode('en_US'), limit=1000)
+    leo: Optional[ThingObject] = None
+    for entity in res_entities:
+        #  Entity must be a person and the label match with full string
+        if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
+            leo = entity
+            break
+
+    artist_student: ThingObject = create_artist()
+    artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
+    knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
+```
+
+## Tools
+
+The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
+
+### Listing script
+
+Listing the entities for tenant. 
+
+```bash
+>> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-r, --relations (optional)_ -  Requesting the relations for each entity
+
+### Export entities script
+
+Dump all entities of a user to a ndjson file. 
+
+```bash
+>> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
+                        knowledge.wacom.com)
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-r, --relations (optional)_ -  Requesting the relations for each entity
+- _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
+- _-p, --images (optional)_ - Include the images in the dump.
+- _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
+ 
+### Push entities script
+
+Pushing entities to knowledge graph.
+
+```bash
+>> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
+  
+### Reset
+
+Resets a tenant by removing entities, groups, and users. 
+
+```bash
+>> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
+  
+# Documentation
+
+You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
+API documentation is available [here](./docs/).
+
+## Contributing
+Contribution guidelines are still work in progress.
+
+## License
+[Apache License 2.0](LICENSE)
```

### Comparing `personal_knowledge_library-0.9.5/README.md` & `personal_knowledge_library-0.9.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: personal_knowledge_library
+Version: 0.9.6
+Summary: Library to access Wacom's Personal Knowledge graph.
+Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
+Author: Markus Weber
+Author-email: markus.weber@wacom.com
+License: Apache 2.0 License
+Keywords: semantic-knowledge;knowledge-graph
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Wacom Personal Knowledge Library
 
 The library and the cloud services are still under development. 
 The required access tokens are only available for selected partner companies.
 
 > :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
 
@@ -784,7 +806,9 @@
 API documentation is available [here](./docs/).
 
 ## Contributing
 Contribution guidelines are still work in progress.
 
 ## License
 [Apache License 2.0](LICENSE)
+
+
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/__init__.py` & `personal_knowledge_library-0.9.6/knowledge/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
-""""Personal knowledge Library"""
+""""
+Personal knowledge Library
+--------------------------
+This library provides a set of tools to manage Wacom private knowledge graph API.
+All services are wrapped in a pythonic way to make it easy to use.
+"""
 import logging
 from typing import Optional
 
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 # Create the Logger
 logger: Optional[logging.Logger] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/base/__init__.py` & `personal_knowledge_library-0.9.6/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.5/knowledge/base/access.py` & `personal_knowledge_library-0.9.6/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.5/knowledge/base/entity.py` & `personal_knowledge_library-0.9.6/knowledge/base/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,30 @@
     def main(self) -> bool:
         """Flag if the content is the  main content or an alias."""
         return self.__main
 
     @staticmethod
     def create_from_dict(dict_label: Dict[str, Any], tag_name: str = CONTENT_TAG, locale_name: str = LOCALE_TAG) \
             -> 'Label':
+        """
+        Create a label from a dictionary.
+        Parameters
+        ----------
+        dict_label: Dict[str, Any]
+            Dictionary containing the label information.
+        tag_name: str
+            Tag name of the content.
+        locale_name: str
+            Tag name of the language code.
+
+        Returns
+        -------
+        instance: Label
+            Label instance.
+        """
         if tag_name not in dict_label:
             raise ValueError("Dict is does not contain a localized label.")
         if locale_name not in dict_label:
             raise ValueError("Dict is does not contain a language code")
         if IS_MAIN_TAG in dict_label:
             return Label(dict_label[tag_name], dict_label[locale_name], dict_label[IS_MAIN_TAG])
         else:
@@ -465,24 +481,52 @@
         self.__orphaned: bool = orphaned
         self.__concepts: List[str] = concepts
         self.__properties: List[str] = properties
         super().__init__(tenant_id, name, icon, labels, comments, context)
 
     @property
     def id(self) -> str:
+        """Context id."""
         return self.__id
 
     @property
     def base_uri(self) -> str:
+        """Base URI."""
         return self.__base_uri
 
     @property
     def orphaned(self) -> bool:
+        """Orphaned."""
         return self.__orphaned
 
+    @property
+    def version(self) -> int:
+        """Version."""
+        return self.__version
+
+    @property
+    def date_added(self) -> datetime:
+        """Date added."""
+        return self.__date_added
+
+    @property
+    def date_modified(self) -> datetime:
+        """Date modified."""
+        return self.__date_modified
+
+    @property
+    def concepts(self) -> List[str]:
+        """List of concepts."""
+        return self.__concepts
+
+    @property
+    def properties(self) -> List[str]:
+        """List of properties."""
+        return self.__properties
+
     @classmethod
     def from_dict(cls, context_dict: Dict[str, Any]):
         context_data: Dict[str, Any] = context_dict['context']
         labels: List[OntologyLabel] = [] if context_data['labels'] is None else \
             [Label(content=la[VALUE_TAG], language_code=la[LANGUAGE_TAG]) for la in context_data['labels']]
         comments: List[Comment] = [] if context_data['comments'] is None else \
             [Comment(text=la[VALUE_TAG], language_code=la[LANGUAGE_TAG]) for la in context_data['comments']]
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/base/ontology.py` & `personal_knowledge_library-0.9.6/knowledge/base/ontology.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 SUB_CLASS_OF_TAG: str = 'subClassOf'
 TENANT_ID: str = 'tenantId'
 NAME_TAG: str = "name"
 SUPPORTED_LOCALES: List[str] = ['ja_JP', 'en_US', 'de_DE', 'bg_BG', 'fr_FR', 'it_IT', 'es_ES', 'zh_CN']
 SUPPORTED_LANGUAGES: List[str] = ['ja', 'en', 'de', 'bg', 'fr', 'it', 'es', 'zh']
 LANGUAGE_LOCALE_MAPPING: Dict[str, str] = dict([(lang, locale)
                                                 for lang, locale in zip(SUPPORTED_LANGUAGES, SUPPORTED_LOCALES)])
+LOCALE_LANGUAGE_MAPPING: Dict[str, str] = dict([(locale, lang)
+                                                for locale, lang in zip(SUPPORTED_LOCALES, SUPPORTED_LANGUAGES)])
 
+
+# ---------------------------------------------------- Ontology --------------------------------------------------------
 class PropertyType(enum.Enum):
     """
     PropertyType
     -----------
     Within the ontology two different property types are defined. A data- and an object property.
     """
     OBJECT_PROPERTY = "Relation"
@@ -578,18 +582,37 @@
             if isinstance(outgoing_relation, dict):
                 outgoing.append(ThingObject.from_dict(outgoing_relation))
             elif isinstance(outgoing_relation, str):
                 outgoing.append(outgoing_relation)
         return relation_type, ObjectProperty(relation_type, incoming, outgoing)
 
     def __dict__(self):
+        outgoing_relations: List[str] = []
+        incoming_relations: List[str] = []
+        for e in self.incoming_relations:
+
+            if isinstance(e, ThingObject):
+                if e.uri is not None:
+                    incoming_relations.append(e.uri)
+                else:
+                    incoming_relations.append(e.reference_id)
+            else:
+                incoming_relations.append(e)
+        for e in self.outgoing_relations:
+            if isinstance(e, ThingObject):
+                if e.uri is not None:
+                    outgoing_relations.append(e.uri)
+                else:
+                    outgoing_relations.append(e.reference_id)
+            else:
+                outgoing_relations.append(e)
         return {
             RELATION_TAG: self.relation.iri,
-            INCOMING_TAG: [e.uri if isinstance(e, ThingObject) else e for e in self.incoming_relations],
-            OUTGOING_TAG: [e.uri if isinstance(e, ThingObject) else e for e in self.outgoing_relations]
+            INCOMING_TAG: incoming_relations,
+            OUTGOING_TAG: outgoing_relations
         }
 
     def __repr__(self):
         return f'{self.relation.iri}, in:={self.incoming_relations}, out:={self.outgoing_relations}'
 
     @staticmethod
     def create_from_list(param: List[dict]) -> Dict[OntologyPropertyReference, 'ObjectProperty']:
@@ -1000,14 +1023,66 @@
         if SYSTEM_SOURCE_REFERENCE_ID not in self.__data_properties:
             self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID] = []
         for idx in range(0, len(self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID])):
             if self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID][idx].language_code == value.language_code:
                 del self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID][idx]
         self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID].append(value)
 
+    @property
+    def reference_id(self) -> Optional[str]:
+        """Default reference id for the entity."""
+        if SYSTEM_SOURCE_REFERENCE_ID in self.__data_properties:
+            # The en_US is the default language for the source reference id
+            for sr in self.data_properties[SYSTEM_SOURCE_REFERENCE_ID]:
+                if sr.language_code == LanguageCode('en_US'):
+                    return sr.value
+            if len(self.data_properties[SYSTEM_SOURCE_REFERENCE_ID]) > 0:
+                return self.data_properties[SYSTEM_SOURCE_REFERENCE_ID][0].value
+        return None
+
+    @reference_id.setter
+    def reference_id(self, value: str):
+        """
+        Setting the default reference id for the entity.
+
+        Parameters
+        ----------
+        value: str
+            Reference id to be set
+        """
+        if SYSTEM_SOURCE_REFERENCE_ID not in self.__data_properties:
+            self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID] = []
+        self.__data_properties[SYSTEM_SOURCE_REFERENCE_ID].append(DataProperty(value, SYSTEM_SOURCE_REFERENCE_ID))
+
+    @property
+    def source_system(self) -> Optional[str]:
+        """Default reference system for the entity."""
+        if SYSTEM_SOURCE_REFERENCE_ID in self.__data_properties:
+            # The en_US is the default language for the source reference system
+            for sr in self.data_properties[SYSTEM_SOURCE_SYSTEM]:
+                if sr.language_code == LanguageCode('en_US'):
+                    return sr.value
+            if len(self.data_properties[SYSTEM_SOURCE_SYSTEM]) > 0:
+                return self.data_properties[SYSTEM_SOURCE_SYSTEM][0].value
+        return None
+
+    @source_system.setter
+    def source_system(self, value: str):
+        """
+        Setting the default reference system for the entity.
+
+        Parameters
+        ----------
+        value: str
+            Reference id to be set
+        """
+        if SYSTEM_SOURCE_SYSTEM not in self.__data_properties:
+            self.__data_properties[SYSTEM_SOURCE_SYSTEM] = []
+        self.__data_properties[SYSTEM_SOURCE_SYSTEM].append(DataProperty(value, SYSTEM_SOURCE_SYSTEM))
+
     def default_source_reference_id(self, language_code: LanguageCode = LanguageCode('en_US')) -> Optional[str]:
         """
         Getting the source reference id for a certain language code.
 
         Parameters
         ----------
         language_code: LanguageCode
@@ -1156,31 +1231,41 @@
         """Relations of the concept."""
         return self.__object_properties
 
     @object_properties.setter
     def object_properties(self, relations: Dict[OntologyPropertyReference, ObjectProperty]):
         self.__object_properties = relations
 
-    def data_property_lang(self, property: OntologyPropertyReference, language_code: LanguageCode) \
+    def data_property_lang(self, data_property: OntologyPropertyReference, language_code: LanguageCode) \
             -> List[DataProperty]:
         """
         Get data property for language_code code.
 
         Parameters
         ----------
-        property: OntologyPropertyReference
+        data_property: OntologyPropertyReference
             Data property.
         language_code: LanguageCode
             Requested language_code code
         Returns
         -------
         data_properties: List[DataProperty]
             Returns a list of data properties for a specific language code
         """
-        return [d for d in self.data_properties.get(property, []) if d.language_code == language_code]
+        return [d for d in self.data_properties.get(data_property, []) if d.language_code == language_code]
+
+    def remove_data_property(self, data_property: OntologyPropertyReference):
+        """Remove data property.
+
+        Parameters
+        ----------
+        data_property: OntologyPropertyReference
+            Data property to be removed.
+        """
+        self.__data_properties.pop(data_property, None)
 
     @property
     def alias(self) -> List[Label]:
         """Alternative labels of the concept."""
         return self.__alias
 
     @alias.setter
@@ -1289,14 +1374,37 @@
         }
         for literal_type, items in self.data_properties.items():
             dict_object[DATA_PROPERTIES_TAG][literal_type.iri] = [i.__dict__() for i in items]
         for relation_type, item in self.object_properties.items():
             dict_object[OBJECT_PROPERTIES_TAG][relation_type.iri] = item.__dict__()
         return dict_object
 
+    def __import_format_dict__(self, group_ids: List[Dict[str, str]] = None):
+        labels: List[Dict[str, Any]] = []
+        labels.extend([la.__dict__() for la in self.label])
+        labels.extend([la.__dict__() for la in self.alias])
+        dict_object: Dict[str, Any] = {
+            SOURCE_REFERENCE_ID_TAG: self.reference_id,
+            SOURCE_SYSTEM_TAG: self.source_system,
+            IMAGE_TAG: self.image,
+            LABELS_TAG: labels,
+            DESCRIPTIONS_TAG: [desc.__dict__() for desc in self.description],
+            TYPE_TAG: self.concept_type.iri,
+            DATA_PROPERTIES_TAG: [],
+            OBJECT_PROPERTIES_TAG: [],
+            TENANT_RIGHTS_TAG: self.tenant_access_right.to_list(),
+            GROUP_IDS: group_ids if group_ids else [],
+            SEND_TO_NEL_TAG: self.use_for_nel
+        }
+        for literal_type, items in self.data_properties.items():
+            dict_object[DATA_PROPERTIES_TAG].extend([i.__dict__() for i in items])
+        for relation_type, item in self.object_properties.items():
+            dict_object[OBJECT_PROPERTIES_TAG].append(item.__dict__())
+        return dict_object
+
     @staticmethod
     def from_dict(entity: Dict[str, Any]) -> 'ThingObject':
         labels: List[Label] = []
         alias: List[Label] = []
         descriptions: List[Description] = []
 
         for label in entity[LABELS_TAG]:
@@ -1367,19 +1475,19 @@
                     self.__alias.append(Label.create_from_dict(label))
 
         for desc in state[DESCRIPTIONS_TAG]:
             self.__description.append(Description.create_from_dict(desc))
 
         use_nel: bool = state.get(USE_NEL_TAG, True)
         visibility: Optional[str] = state.get(VISIBILITY_TAG)
-        self.__icon=state[IMAGE_TAG]
-        self.__uri=state[URI_TAG]
-        self.__concept_type=OntologyClassReference.parse(state[TYPE_TAG])
-        self.__owner=state.get(OWNER_TAG, True)
-        self.__use_for_nel=use_nel
+        self.__icon = state[IMAGE_TAG]
+        self.__uri = state[URI_TAG]
+        self.__concept_type = OntologyClassReference.parse(state[TYPE_TAG])
+        self.__owner = state.get(OWNER_TAG, True)
+        self.__use_for_nel = use_nel
         self.__visibility = visibility
         self.__owner_id = state.get(OWNER_ID_TAG)
         self.__group_ids = state.get(GROUP_IDS)
         if DATA_PROPERTIES_TAG in state:
             if isinstance(state[DATA_PROPERTIES_TAG], dict):
                 for data_property_type_str, data_properties in state[DATA_PROPERTIES_TAG].items():
                     data_property_type: OntologyPropertyReference = \
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/nel/base.py` & `personal_knowledge_library-0.9.6/knowledge/nel/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         List of supported languages
     verify_calls: bool (default:=False)
         Verifies all HTTPS calls and the associated certificate.
     """
 
     def __init__(self, service_url: str = str, supported_languages: List[str] = None, verify_calls: bool = True):
         super().__init__(application_name="Personal entity linking", service_url=service_url,
-                         service_endpoint="graph", verify_calls=verify_calls)
+                         service_endpoint='graph/v1', verify_calls=verify_calls)
         self.__supported_languages: List[str] = supported_languages if supported_languages else []
 
     @abc.abstractmethod
     def link_personal_entities(self, auth_key: str, text: str, language_code: LanguageCode = 'en_US') \
             -> List[KnowledgeGraphEntity]:
         """
         Performs Named Entity Linking on a text. It only finds entities which are accessible by the user identified by
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/nel/engine.py` & `personal_knowledge_library-0.9.6/knowledge/nel/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,30 @@
         LanguageCode('ja_JP')
     ]
 
     def __init__(self, service_url: str = SERVICE_URL, service_endpoint: str = SERVICE_ENDPOINT):
         self.__service_endpoint: str = service_endpoint
         super().__init__(supported_languages=WacomEntityLinkingEngine.LANGUAGES, service_url=service_url)
 
-    def link_personal_entities(self, auth_key: str, text: str, locale: str = 'en_US') \
+    def link_personal_entities(self, auth_key: str, text: str, locale: str = 'en_US', max_retries: int = 5) \
             -> List[KnowledgeGraphEntity]:
         """
         Performs Named Entity Linking on a text. It only finds entities which are accessible by the user identified by
         the auth key.
 
         Parameters
         ----------
         auth_key: str
             Auth key identifying a user within the Wacom personal knowledge service.
         text: str
             Text where the entities shall be tagged in.
         locale: LanguageCode
             ISO-3166 Country Codes and ISO-639 Language Codes in the format '<language_code>_<country>', e.g., en_US.
+        max_retries: int
+            Maximum number of retries, if the service is not available.
 
         Returns
         -------
         entities: List[KnowledgeGraphEntity]
             List of knowledge graph entities.
 
         Raises
@@ -70,16 +72,16 @@
         }
         payload: Dict[str, str] = {
             LOCALE_TAG: locale,
             TEXT_TAG: text
         }
         # Define the retry policy
         retry_policy: Retry = Retry(
-            total=10,  # maximum number of retries
-            backoff_factor=1.5,  # factor by which to multiply the delay between retries
+            total=max_retries,  # maximum number of retries
+            backoff_factor=0.5,  # factor by which to multiply the delay between retries
             status_forcelist=[429, 500, 502, 503, 504],  # HTTP status codes to retry on
             method_whitelist=["POST"],  # HTTP methods to retry on
             respect_retry_after_header=True  # respect the Retry-After header
         )
 
         # Create a session and mount the retry adapter
         with requests.Session() as session:
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/services/base.py` & `personal_knowledge_library-0.9.6/knowledge/services/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 CONTENT_TYPE_HEADER_FLAG: str = 'Content-Type'
 TENANT_API_KEY: str = 'x-tenant-api-key'
 REFRESH_TOKEN_TAG: str = 'refreshToken'
 
 
 class WacomServiceException(Exception):
     """Exception thrown if Wacom service fails."""
+    def __init__(self, message: str, status_code: int = 500):
+        super().__init__(message)
+        self.__status_code: int = status_code
+
+    @property
+    def status_code(self) -> int:
+        """Status code of the exception."""
+        return self.__status_code
 
 
 class RESTAPIClient(ABC):
     """
     Abstract REST API client
     ------------------------
     REST API client handling the service url.
@@ -128,15 +136,16 @@
                     date_object: datetime = datetime.now()
                 return response_token['accessToken'], response_token['refreshToken'], date_object
             except Exception as e:
                 raise WacomServiceException(f'Login failed'
                                             f'Response code:={response.status_code}, response text:= {response.text}, '
                                             f'exception:= {e} ')
         raise WacomServiceException(f'User login failed.'
-                                    f'Response code:={response.status_code}, exception:= {response.text}')
+                                    f'Response code:={response.status_code}, exception:= {response.text}',
+                                    status_code=response.status_code)
 
     def refresh_token(self, refresh_token: str) -> Tuple[str, str, datetime]:
         """
         Refreshing a token.
 
         Parameters
         ----------
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/services/graph.py` & `personal_knowledge_library-0.9.6/knowledge/services/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,14 @@
     LOCALE_TAG, EntityStatus, Label, Description, URIS_TAG, FORCE_TAG
 from knowledge.base.ontology import DataProperty, OntologyPropertyReference, ThingObject, OntologyClassReference, \
     ObjectProperty
 from knowledge.services import USER_AGENT_STR
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException, AUTHORIZATION_HEADER_FLAG, \
     USER_AGENT_HEADER_FLAG, CONTENT_TYPE_HEADER_FLAG
 
-
-
 # ------------------------------------------------- Constants ----------------------------------------------------------
 ACTIVATION_TAG: str = 'activation'
 SEARCH_TERM: str = 'searchTerm'
 LANGUAGE_PARAMETER: str = 'language'
 TYPES_PARAMETER: str = 'types'
 LIMIT_PARAMETER: str = 'limit'
 LITERAL_PARAMETER: str = 'Literal'
@@ -273,15 +271,14 @@
             session.mount(mount_point, HTTPAdapter(max_retries=retries))
             response: Response = session.delete(url, headers=headers, params={FORCE_TAG: force},
                                                 verify=self.verify_calls)
             if not response.ok:
                 raise WacomServiceException(f'Deletion of entity (URI:={uri}) failed.'
                                             f'Response code:={response.status_code}, exception:= {response.content}')
 
-
     def exists(self, auth_key: str, uri: str) -> bool:
         """
         Check if entity exists in knowledge graph.
 
         Parameters
         ----------
         auth_key: str -
@@ -335,15 +332,15 @@
             if label is not None and len(label.content) > 0 and label.content != " ":
                 labels.append({
                     VALUE_TAG: label.content,
                     LOCALE_TAG: label.language_code,
                     IS_MAIN_TAG: False
                 })
         # Labels are tagged as main label
-        for literal_property, list_literals in entity.data_properties.items():
+        for _, list_literals in entity.data_properties.items():
             for li in list_literals:
                 if li.data_property_type:
                     literals.append({
                         VALUE_TAG: li.value,
                         LOCALE_TAG: li.language_code
                         if li.language_code and li.language_code in SUPPORTED_LANGUAGES else "en_US",
                         DATA_PROPERTY_TAG: li.data_property_type.iri
@@ -417,14 +414,16 @@
         entity: ThingObject
             Entity object that needs to be created
         max_retries: int
             Maximum number of retries
         backoff_factor: float
             A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a
             second try without a delay)
+        ignore_image: bool
+            Ignore image.
 
         Returns
         -------
         uri: str
             URI of entity
 
 
@@ -573,18 +572,24 @@
             If the graph service returns an error code
         """
         url: str = f'{self.service_base_url}{WacomKnowledgeService.ENTITY_ENDPOINT}/{urllib.parse.quote(uri)}/relations'
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.get(url, headers=headers, verify=self.verify_calls)
-        if response.ok:
-            rel: list = response.json().get(RELATIONS_TAG)
-            return ObjectProperty.create_from_list(rel)
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.get(url, headers=headers, verify=self.verify_calls)
+            if response.ok:
+                rel: list = response.json().get(RELATIONS_TAG)
+                return ObjectProperty.create_from_list(rel)
         raise WacomServiceException(f'Failed to pull relations. '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
     def labels(self, auth_key: str, uri: str, locale: str = 'en_US') -> List[Label]:
         """
         Extract list labels of entity.
 
@@ -688,24 +693,24 @@
         }
         params: dict = {
             RELATION_TAG: relation.iri,
             TARGET: target
         }
         mount_point: str = \
             'https://' if self.service_url.startswith('https') else 'http://'
-        session: requests.Session = requests.Session()
-        retries: Retry = Retry(backoff_factor=0.1,
-                               status_forcelist=[500, 502, 503, 504])
-        session.mount(mount_point, HTTPAdapter(max_retries=retries))
-        response: Response = session.post(url, params=params, headers=headers, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Create relations failed. '
-                                        f'Response code:={response.status_code}, exception:= {response.content}. '
-                                        f'URL: {url}'
-                                        f'Parameters: \n{json.dumps(params, indent=4)}')
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.post(url, params=params, headers=headers, verify=self.verify_calls)
+            if not response.ok:
+                raise WacomServiceException(f'Create relations failed. '
+                                            f'Response code:={response.status_code}, exception:= {response.content}. '
+                                            f'URL: {url}'
+                                            f'Parameters: \n{json.dumps(params, indent=4)}')
 
     def remove_relation(self, auth_key: str, source: str, relation: OntologyPropertyReference, target: str):
         """
         Removes a relation.
 
         Parameters
         ----------
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/services/group.py` & `personal_knowledge_library-0.9.6/knowledge/services/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021-23 Wacom. All rights reserved.
 import urllib.parse
 from typing import Dict, List, Any, Optional
 
 import requests
 from requests import Response
+from requests.adapters import HTTPAdapter
+from urllib3 import Retry
 
 from knowledge.base.access import GroupAccessRight
 from knowledge.base.ontology import NAME_TAG
 from knowledge.services.base import WacomServiceAPIClient, WacomServiceException
 from knowledge.services.graph import AUTHORIZATION_HEADER_FLAG, CONTENT_TYPE_HEADER_FLAG
 
 # -------------------------------------- Constant flags ----------------------------------------------------------------
 from knowledge.services.users import User
 
 GROUP_USER_RIGHTS_TAG: str = "groupUserRights"
 JOIN_KEY_PARAM: str = "joinKey"
 USER_TO_ADD_PARAM: str = "userToAddId"
 USER_TO_REMOVE_PARAM: str = "userToRemoveId"
+FORCE_PARAM: str = "force"
+DEFAULT_TIMEOUT: int = 30
 
 
 class Group(object):
     """
     Group
     -----
     In Personal Knowledge backend users can be logically grouped.
@@ -186,19 +190,26 @@
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}',
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
         payload: Dict[str, str] = {
             NAME_TAG: name,
             GROUP_USER_RIGHTS_TAG: rights.to_list()
         }
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
-        if response.ok:
-            return Group.parse(response.json())
-        raise WacomServiceException(f'Creation of group failed.'
-                                    f'Response code:={response.status_code}, exception:= {response.text}')
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.post(url, headers=headers, json=payload, verify=self.verify_calls,
+                                              timeout=DEFAULT_TIMEOUT)
+            if response.ok:
+                return Group.parse(response.json())
+            raise WacomServiceException(f'Creation of group failed.'
+                                        f'Response code:={response.status_code}, exception:= {response.text}')
 
     def update_group(self, auth_key: str, group_id: str, name: str, rights: GroupAccessRight = GroupAccessRight):
         """
         Updates a group.
 
         Parameters
         ----------
@@ -221,18 +232,25 @@
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}',
             CONTENT_TYPE_HEADER_FLAG: 'application/json'
         }
         payload: Dict[str, str] = {
             NAME_TAG: name,
             GROUP_USER_RIGHTS_TAG: rights.to_list()
         }
-        response: Response = requests.patch(url, headers=headers, json=payload, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Update of group failed.'
-                                        f'Response code:={response.status_code}, exception:= {response.text}')
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.patch(url, headers=headers, json=payload, verify=self.verify_calls,
+                                               timeout=DEFAULT_TIMEOUT)
+            if not response.ok:
+                raise WacomServiceException(f'Update of group failed.'
+                                            f'Response code:={response.status_code}, exception:= {response.text}')
 
     def delete_group(self, auth_key: str, group_id: str):
         """
          Delete a group.
 
          Parameters
          ----------
@@ -246,18 +264,24 @@
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Deletion of group failed.'
-                                        f'Response code:={response.status_code}, exception:= {response.text}')
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
+            if not response.ok:
+                raise WacomServiceException(f'Deletion of group failed.'
+                                            f'Response code:={response.status_code}, exception:= {response.text}')
 
     def listing_groups(self, auth_key: str, admin: bool = False) -> List[Group]:
         """
         Listing all groups configured for this instance.
 
         Parameters
         ----------
@@ -275,18 +299,24 @@
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}'
         if admin:
             url += '/admin'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.get(url, headers=headers, verify=self.verify_calls)
-        if response.ok:
-            groups: List[Dict[str, Any]] = response.json()
-            return [Group.parse(g) for g in groups]
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
+            if response.ok:
+                groups: List[Dict[str, Any]] = response.json()
+                return [Group.parse(g) for g in groups]
         raise WacomServiceException(f'Listing of group failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def group(self, auth_key: str, group_id: str) -> GroupInfo:
         """Get a group.
 
         Parameters
@@ -306,15 +336,15 @@
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.get(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
             group: Dict[str, Any] = response.json()
             return GroupInfo.parse(group)
         raise WacomServiceException(f'Getting of group information failed.'
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def join_group(self, auth_key: str, group_id: str, join_key: str):
@@ -337,15 +367,16 @@
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/join'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         params: Dict[str, str] = {
             JOIN_KEY_PARAM: join_key,
         }
-        response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Joining the group failed.'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def leave_group(self, auth_key: str, group_id: str):
         """User leaving a group with his auth token.
 
@@ -362,15 +393,15 @@
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/leave'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
 
-        response: Response = requests.post(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Leaving group failed.'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def add_user_to_group(self, auth_key: str, group_id: str, user_id: str):
         """Adding a user to group.
 
@@ -391,44 +422,49 @@
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/user/add'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         params: Dict[str, str] = {
             USER_TO_ADD_PARAM: user_id,
         }
-        response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Adding of user to group failed.'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
-    def remove_user_to_group(self, auth_key: str, group_id: str, user_id: str):
-        """Remove a user to group.
+    def remove_user_from_group(self, auth_key: str, group_id: str, user_id: str, force: bool = False):
+        """Remove a user from group.
 
         Parameters
         ----------
         auth_key: str
             API key for user.
         group_id: str
             Id of group
         user_id: str
             User who is remove from the group
+        force: bool
+            If true remove user and entities owned by the user if any
 
         Raises
         ------
         WacomServiceException
             If the tenant service returns an error code.
         """
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/user/remove'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         params: Dict[str, str] = {
             USER_TO_REMOVE_PARAM: user_id,
+            FORCE_PARAM: force
         }
-        response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, params=params, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Removing of user from group failed. URL: {url}'
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def add_entity_to_group(self, auth_key: str, group_id: str, entity_uri: str):
         """Adding a entity to group.
 
@@ -447,19 +483,24 @@
             If the tenant service returns an error code.
         """
         uri: str = urllib.parse.quote(entity_uri)
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/entity/{uri}/add'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-
-        response: Response = requests.post(url, headers=headers, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Adding of entity to group failed.'
-                                        f'Response code:={response.status_code}, exception:= {response.text}')
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.post(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
+            if not response.ok:
+                raise WacomServiceException(f'Adding of entity to group failed.'
+                                            f'Response code:={response.status_code}, exception:= {response.text}')
 
     def remove_entity_to_group(self, auth_key: str, group_id: str, entity_uri: str):
         """Remove a entity from group.
 
         Parameters
         ----------
         auth_key: str
@@ -475,12 +516,17 @@
             If the tenant service returns an error code.
         """
         uri: str = urllib.parse.quote(entity_uri)
         url: str = f'{self.service_base_url}{GroupManagementServiceAPI.GROUP_ENDPOINT}/{group_id}/entity/{uri}/remove'
         headers: Dict[str, str] = {
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-
-        response: Response = requests.post(url, headers=headers, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Removing of entity to group failed.'
-                                        f'Response code:={response.status_code}, exception:= {response.text}')
+        mount_point: str = \
+            'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(backoff_factor=0.1,
+                                   status_forcelist=[500, 502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.post(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
+            if not response.ok:
+                raise WacomServiceException(f'Removing of entity to group failed.'
+                                            f'Response code:={response.status_code}, exception:= {response.text}')
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/services/ontology.py` & `personal_knowledge_library-0.9.6/knowledge/services/ontology.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 LABELS_TAG: str = "labels"
 LANGUAGE_CODE: str = 'lang'
 NAME_TAG: str = "name"
 RANGE_TAG: str = "ranges"
 SUB_CLASS_OF_TAG: str = "subClassOf"
 SUB_PROPERTY_OF_TAG: str = "subPropertyOf"
 TEXT_TAG: str = 'value'
+DEFAULT_TIMEOUT: int = 30
 
 
 class OntologyService(WacomServiceAPIClient):
     """
     Ontology API Client
     -------------------
     Client to access the ontology service. Offers the following functionality:
@@ -127,15 +128,15 @@
         """
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context}/' \
                    f'{OntologyService.CONCEPTS_ENDPOINT}'
-        response: Response = requests.get(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
             response_list: List[Tuple[OntologyClassReference, OntologyClassReference]] = []
             result = response.json()
             for struct in result:
                 response_list.append((OntologyClassReference.parse(struct[NAME_TAG]),
                                       None if struct[SUB_CLASS_OF_TAG] is None else
                                       OntologyClassReference.parse(struct[SUB_CLASS_OF_TAG])))
@@ -205,15 +206,15 @@
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         concept_url: str = urllib.parse.quote_plus(concept_name)
         response: Response = requests.get(f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context_url}'
                                           f'/{OntologyService.CONCEPTS_ENDPOINT}/{concept_url}',
-                                          headers=headers, verify=self.verify_calls)
+                                          headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
             result: Dict[str, Any] = response.json()
             return OntologyClass.from_dict(result)
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def property(self, auth_key: str, context: str, property_name: str) -> OntologyProperty:
         """Retrieve a property instance.
@@ -238,15 +239,16 @@
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         concept_url: str = urllib.parse.quote_plus(property_name)
         param: str = f"context/{context_url}/properties/{concept_url}"
-        response: Response = requests.get(f'{self.service_base_url}{param}', headers=headers, verify=self.verify_calls)
+        response: Response = requests.get(f'{self.service_base_url}{param}', headers=headers, verify=self.verify_calls,
+                                          timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return OntologyProperty.from_dict(response.json())
         raise WacomServiceException(f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_concept(self, auth_key: str, context: str, reference: OntologyClassReference,
                        subclass_of: OntologyClassReference = THING_CLASS,
                        icon: Optional[str] = None, labels: Optional[List[OntologyLabel]] = None,
@@ -295,15 +297,16 @@
         }
         for label in labels if labels is not None else []:
             payload[LABELS_TAG].append({TEXT_TAG: label.content, LANGUAGE_CODE: label.language_code})
         for comment in comments if comments is not None else []:
             payload[COMMENTS_TAG].append({TEXT_TAG: comment.content, LANGUAGE_CODE: comment.language_code})
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context}/' \
                    f'{OntologyService.CONCEPTS_ENDPOINT}'
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if response.ok:
             result_dict: Dict[str, str] = response.json()
             return result_dict
         raise WacomServiceException(f'Creation of concept failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def update_concept(self, auth_key: str, context: str, name: str, subclass_of: Optional[str],
@@ -354,15 +357,16 @@
         }
         for label in labels if labels is not None else []:
             payload[LABELS_TAG].append({TEXT_TAG: label.content, LANGUAGE_CODE: label.language_code})
         for comment in comments if comments is not None else []:
             payload[COMMENTS_TAG].append({TEXT_TAG: comment.content, LANGUAGE_CODE: comment.language_code})
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context}/' \
                    f'{OntologyService.CONCEPTS_ENDPOINT}'
-        response: Response = requests.put(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.put(url, headers=headers, json=payload, verify=self.verify_calls,
+                                          timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Update of concept failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def delete_concept(self, auth_key: str, context: str, reference: OntologyClassReference):
         """Delete concept class.
@@ -387,15 +391,15 @@
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         concept_url: str = urllib.parse.quote_plus(reference.iri)
         url: str = f'{self.service_base_url}context/{context_url}/concepts/{concept_url}'
-        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Deletion of concept failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_object_property(self, auth_key: str, context: str,
                                reference: OntologyPropertyReference,
                                domains_cls: List[OntologyClassReference], ranges_cls: List[OntologyClassReference],
@@ -460,15 +464,16 @@
         context_url: str = urllib.parse.quote_plus(context)
         for label in labels if labels is not None else []:
             payload[LABELS_TAG].append({TEXT_TAG: label.content, LANGUAGE_CODE: label.language_code})
         for comment in comments if comments is not None else []:
             payload[COMMENTS_TAG].append({TEXT_TAG: comment.content, LANGUAGE_CODE: comment.language_code})
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context_url}/' \
                    f'{OntologyService.PROPERTIES_ENDPOINT}'
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Creation of object property failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_data_property(self, auth_key: str, context: str,
                              reference: OntologyPropertyReference,
@@ -530,15 +535,16 @@
         context_url: str = urllib.parse.quote_plus(context)
         for label in labels if labels is not None else []:
             payload[LABELS_TAG].append({TEXT_TAG: label.content, LANGUAGE_CODE: label.language_code})
         for comment in comments if comments is not None else []:
             payload[COMMENTS_TAG].append({TEXT_TAG: comment.content, LANGUAGE_CODE: comment.language_code})
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{context_url}/' \
                    f'{OntologyService.PROPERTIES_ENDPOINT}'
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Creation of data property failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def delete_property(self, auth_key: str, context: str, reference: OntologyPropertyReference):
         """Delete property.
@@ -563,15 +569,15 @@
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         property_url: str = urllib.parse.quote_plus(reference.iri)
         url: str = f'{self.service_base_url}context/{context_url}/properties/{property_url}'
-        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Deletion of property: {reference.iri} failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def create_context(self, auth_key: str, name: str, base_uri: Optional[str] = None, icon: Optional[str] = None,
                        labels: List[OntologyLabel] = None, comments: List[Comment] = None) -> Dict[str, str]:
         """Create context.
@@ -616,27 +622,28 @@
             ICON_TAG: icon
         }
         for label in labels if labels is not None else []:
             payload[LABELS_TAG].append({TEXT_TAG: label.content, LANGUAGE_CODE: label.language_code})
         for comment in comments if comments is not None else []:
             payload[COMMENTS_TAG].append({TEXT_TAG: comment.content, LANGUAGE_CODE: comment.language_code})
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}'
-        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls)
+        response: Response = requests.post(url, headers=headers, json=payload, verify=self.verify_calls,
+                                           timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return response.json()
         raise WacomServiceException(f'Creation of concept failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
 
     def remove_context(self, auth_key: str, name: str, force: bool = False):
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         url: str = f'{self.service_base_url}{OntologyService.CONTEXT_ENDPOINT}/{name}{"/force" if force else ""}'
-        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.delete(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
 
             raise WacomServiceException(f'Removing the context failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def commit(self, auth_key: str, context: str):
         """
@@ -651,15 +658,15 @@
         """
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         url: str = f'{self.service_base_url}context/{context_url}/commit'
-        response: Response = requests.put(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.put(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if not response.ok:
             raise WacomServiceException(f'Commit of ontology failed. '
                                         f'Response code:={response.status_code}, exception:= {response.text}')
 
     def rdf_export(self, auth_key: str, context: str) -> str:
         """
         Export RDF.
@@ -678,12 +685,12 @@
         """
         headers: Dict[str, str] = {
             USER_AGENT_TAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
         context_url: str = urllib.parse.quote_plus(context)
         url: str = f'{self.service_base_url}context/{context_url}/versions/rdf'
-        response: Response = requests.get(url, headers=headers, verify=self.verify_calls)
+        response: Response = requests.get(url, headers=headers, verify=self.verify_calls, timeout=DEFAULT_TIMEOUT)
         if response.ok:
             return response.text
         raise WacomServiceException(f'RDF export failed. '
                                     f'Response code:={response.status_code}, exception:= {response.text}')
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/services/tenant.py` & `personal_knowledge_library-0.9.6/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.5/knowledge/services/users.py` & `personal_knowledge_library-0.9.6/knowledge/services/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # -------------------------------------- Constant flags ----------------------------------------------------------------
 TENANT_ID: str = 'tenantId'
 USER_ID_TAG: str = 'userId'
 LIMIT_TAG: str = 'limit'
 OFFSET_TAG: str = 'offset'
 ROLES_TAG: str = 'roles'
-META_DATA_TAG: str = 'metaData'
+META_DATA_TAG: str = 'metadata'
 INTERNAL_USER_ID_TAG: str = 'internalUserId'
 EXTERNAL_USER_ID_TAG: str = 'externalUserId'
 FORCE_TAG: str = 'force'
 CONTENT_TYPE_FLAG: str = 'Content-Type'
 TENANT_API_KEY_FLAG: str = 'x-tenant-api-key'
 USER_AGENT_TAG: str = "User-Agent"
 
@@ -97,18 +97,35 @@
     @property
     def user_roles(self) -> List[UserRole]:
         """List of user roles"""
         return self.__user_roles
 
     @classmethod
     def parse(cls, param: Dict[str, Any]) -> 'User':
+        """
+        Parse user from dictionary.
+        Parameters
+        ----------
+        param: Dict[str, Any]
+            Dictionary containing user information.
+
+        Returns
+        -------
+        user: User
+            Instance of user.
+        """
         user_id: str = param['id']
         tenant_id: str = param[TENANT_ID]
         external_user_id: str = param['externalUserId']
-        meta_data: Dict[str, Any] = param['metaData']
+        meta_data: Dict[str, Any] = {}
+        if META_DATA_TAG in param:
+            meta_data = param[META_DATA_TAG]
+        # Support the old version of the user management service
+        elif 'metaData' in param:
+            meta_data = param['metaData']
         user_roles: List[UserRole] = [USER_ROLE_MAPPING[r] for r in param['roles']]
         return User(tenant_id=tenant_id, user_id=user_id, external_user_id=external_user_id, meta_data=meta_data,
                     user_roles=user_roles)
 
     def __repr__(self):
         return f'<User: id:={self.id}, external user id:={self.external_user_id}, user roles:= {self.user_roles}]>'
```

### Comparing `personal_knowledge_library-0.9.5/knowledge/utils/rdf.py` & `personal_knowledge_library-0.9.6/knowledge/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,811 +1,814 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 0.9.5
+Version: 0.9.6
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
-Description: # Wacom Personal Knowledge Library
-        
-        The library and the cloud services are still under development. 
-        The required access tokens are only available for selected partner companies.
-        
-        > :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
-        
-        ## Introduction
-        
-        In knowledge management there is a distinction between data, information and knowledge.
-        In the domain of digital ink this means:
-        
-        - **Data** - The equivalent would be the ink strokes
-        - **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
-        - **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
-        
-        The following illustration shows the different layers of knowledge:
-        ![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
-        
-        For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
-        
-        This library provide simplified access to Wacom's personal knowledge cloud service.
-        It contains:
-        
-        - Basic datastructures for Ontology object and entities from the knowledge graph
-        - Clients for the REST APIs
-        - Connector for Wikidata public knowledge graph
-        
-        **Ontology service:**
-        
-        - List all Ontology structures
-        - Modify Ontology structures
-        - Delete Ontology structures
-        
-        **Entity service:**
-        
-        - List all entities
-        - Add entities to knowledge graph
-        - Access object properties
-        
-        # Technology stack
-        
-        ## Domain Knowledge
-        
-        The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
-        The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
-        
-        - Foundation for structured data, knowledge representation as concepts and relations among concepts
-        - Being explicit definitions of shared vocabularies for interoperability
-        - Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
-        - Can be used for problem solving
-        
-        An ontology defines (specifies) the concepts, relationships, and other distinctions that are relevant for modelling a domain.
-        
-        ## Knowledge Graph
-        
-        - Knowledge graph is generated from unstructured and structured knowledge sources
-        - Contains all structured knowledge gathered from all sources
-        - Foundation for all semantic algorithms
-        
-        ## Semantic Technology
-        
-        - Extract knowledge from various sources (Connectors)
-        - Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
-        - Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
-        
-        
-        # Functionality
-        
-        ## Access API
-        
-        The personal knowledge graph backend is implement as a multi-tenancy system.
-        Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
-        
-        ![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
-        
-        In general, a tenant with their users, groups, and entities are logically separated.
-        Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
-        
-        The user management is rather limited, each organisation must provide their own authentication service and user management.
-        The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
-        
-        The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
-        While users for each tenant can be created by the owner of the **Tenant API Key**.
-        You will receive this token from the system owner after the creation of the tenant.
-        
-        
-        > :warning: Store the **Tenant API Key** in a secure key store, as attackers can use the key to harm your system.
-        
-        
-        The **Tenant API Key** should be only used by your authentication service to create shadow users and to login your user into the WPK backend.
-        After a successful user login, you will receive a token which can be used by the user to create, update, or delete entities and relations.
-        
-        The following illustration summarizes the flows for creation of tenant and users:
-        
-        ![Tenant and user creation](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-user-creation.png)
-        
-        The organisation itself needs to implement their own authentication service which:
-        
-        - handles the users and their passwords,
-        - controls the personal data of the users,
-        - connects the users with the WPK backend and share with them the user token.
-        
-        The WPK backend only manages the access levels of the entities and the group management for users.
-        The illustration shows how the access token is received from the WPK endpoint:
-        
-        ![Access token request.](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/access-token.png)
-        
-        # Entity API
-        
-        The entities used within the knowledge graph and the relationship among them is defined within an ontology that is manage with Wacom Ontology Management System (WOMS).
-        
-        An entity within the personal knowledge graphs consist of these major parts:
-        
-        - **Icon** - a visual representation of the entity, for instance a portrait of a person.
-        - **URI** - a unique resource identifier of an entity in the graph.
-        - **Type** - the type links to the defined concept class in the ontology.
-        - **Labels** - labels are the word(s) use in a language for the concept.
-        - **Description** - a short abstract that describes the entity.
-        - **Literals** - literals are properties of an entity, such as first name of a person. The ontology defines all literals of the concept class as well as its data type.
-        - **Relations** - the relationship among different entities is described using relations.
-        
-        The following illustration provides an example for an entity:
-        
-        ![Entity description](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/entity-description.png)
-        
-        ## Entity content
-        
-        Entities in general are language-independent as across nationalities or cultures we only use different scripts and words for a shared instance of a concept.
-        
-        Let's take Leonardo da Vinci as an example.
-        The ontology defines the concept of a Person, a human being.
-        Now, in English its label would be _Leonardo da Vinci_, while in Japanese _レオナルド・ダ・ヴィンチ_.
-        Moreover, he is also known as _Leonardo di ser Piero da Vinci_ or _ダ・ビンチ_.
-        
-        ### Labels
-        
-        Now, in the given example all words that a assigned to the concept are labels.
-        The label _Leonardo da Vinci_ is stored in the backend with an additional language code, e.g. _en_.
-        
-        There is always a main label, which refers to the most common or official name of entity.
-        Another example would be Wacom, where _Wacom Co., Ltd._ is the official name while _Wacom_ is commonly used and be considered as an alias.
-        
-        >  :pushpin: For the language code the **ISO 639-1:2002**, codes for the representation of names of languages—Part 1: Alpha-2 code. Read more, [here](https://www.iso.org/standard/22109.html)
-        
-        ## Samples
-        
-        ### Entity handling
-        
-        This samples shows how to work with graph service.
-        
-        ```python
-        import argparse
-        from typing import Optional, List, Dict
-        
-        from knowledge.base.entity import LanguageCode, Description, Label
-        from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
-        from knowledge.services.graph import WacomKnowledgeService
-        
-        # ------------------------------- Knowledge entities -------------------------------------------------------------------
-        LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
-        SELF_PORTRAIT_STYLE: str = 'self-portrait'
-        ICON: str = "https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29."\
-                    "JPG/1024px-Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29.JPG"
-        # ------------------------------- Ontology class names -----------------------------------------------------------------
-        THING_OBJECT: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Thing')
-        """
-        The Ontology will contain a Thing class where is the root class in the hierarchy. 
-        """
-        ARTWORK_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'creative', 'VisualArtwork')
-        PERSON_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Person')
-        ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
-        IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
-        HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
-        CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
-        HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
-        
-        
-        def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
-            """
-            Printing entity details.
-        
-            Parameters
-            ----------
-            entity: ThingObject
-                Entity with properties
-            list_idx: int
-                Index with a list
-            auth_key: str
-                Authorization key
-            client: WacomKnowledgeService
-                Knowledge graph client
-            short: bool
-                Short summary
-            """
-            print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
-            if len(entity.label) > 0:
-                print('    | [Labels]')
-                for la in entity.label:
-                    print(f'    |     |- "{la.content}"@{la.language_code}')
-                print('    |')
-            if not short:
-                if len(entity.alias) > 0:
-                    print('    | [Alias]')
-                    for la in entity.alias:
-                        print(f'    |     |- "{la.content}"@{la.language_code}')
-                    print('    |')
-                if len(entity.data_properties) > 0:
-                    print('    | [Attributes]')
-                    for data_property, labels in entity.data_properties.items():
-                        print(f'    |    |- {data_property.iri}:')
-                        for li in labels:
-                            print(f'    |    |-- "{li.value}"@{li.language_code}')
-                    print('    |')
-        
-                relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
-                                                                                                  uri=entity.uri)
-                if len(relations_obj) > 0:
-                    print('    | [Relations]')
-                    for re in relations_obj.values():
-                        print(f'    |--- {re.relation.iri}: ')
-                        print(f'           |- [Incoming]: {re.incoming_relations} ')
-                        print(f'           |- [Outgoing]: {re.outgoing_relations}')
-                print()
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
-                                help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom personal knowledge REST API Client
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
-                                                                            service_url=args.instance)
-            # Use special tenant for testing:  Unit-test tenant
-            user_token, refresh_token, expiration_time = knowledge_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            page_id: Optional[str] = None
-            page_number: int = 1
-            entity_count: int = 0
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' First step: Find Leonardo da Vinci in the knowledge graph.')
-            print('-----------------------------------------------------------------------------------------------------------')
-            res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
-                                                                            language_code=LanguageCode('en_US'), limit=1000)
-            leo: Optional[ThingObject] = None
-            s_idx: int = 1
-            for entity in res_entities:
-                #  Entity must be a person and the label match with full string
-                if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
-                    leo = entity
-                    break
-        
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' What artwork exists in the knowledge graph.')
-            print('-----------------------------------------------------------------------------------------------------------')
-            relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
-                                                                                                         uri=leo.uri)
-            print(f' Artwork of {leo.label}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            idx: int = 1
-            if CREATED in relations_dict:
-                for e in relations_dict[CREATED].outgoing_relations:
-                    print(f' [{idx}] {e.uri}: {e.label}')
-                    idx += 1
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' Let us create a new piece of artwork.')
-            print('-----------------------------------------------------------------------------------------------------------')
-        
-            # Main labels for entity
-            artwork_labels: List[Label] = [
-                Label('Ginevra Gherardini', LanguageCode('en_US')),
-                Label('Ginevra Gherardini', LanguageCode('de_DE'))
-            ]
-            # Alias labels for entity
-            artwork_alias: List[Label] = [
-                Label("Ginevra", LanguageCode('en_US')),
-                Label("Ginevra", LanguageCode('de_DE'))
-            ]
-            # Topic description
-            artwork_description: List[Description] = [
-                Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
-                Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
-            ]
-            # Topic
-            artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
-                                                      description=artwork_description,
-                                                      icon=ICON)
-            artwork_object.alias = artwork_alias
-            print(f' Create: {artwork_object}')
-            # Create artwork
-            artwork_entity_uri: str = knowledge_client.create_entity(user_token, artwork_object)
-            print(f' Entity URI: {artwork_entity_uri}')
-            # Create relation between Leonardo da Vinci and artwork
-            knowledge_client.create_relation(auth_key=user_token, source=leo.uri, relation=IS_CREATOR,
-                                             target=artwork_entity_uri)
-        
-            relations_dict = knowledge_client.relations(auth_key=user_token, uri=artwork_entity_uri)
-            for ontology_property, object_property in relations_dict.items():
-                print(f'  {object_property}')
-            # You will see that wacom:core#isCreatedBy is automatically inferred as relation as it is the inverse property of
-            # wacom:core#created.
-        
-            # Now, more search options
-            res_entities, next_search_page = knowledge_client.search_description(user_token, 'Michelangelo\'s Sistine Chapel',
-                                                                                 LanguageCode('en_US'), limit=1000)
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' Search results.  Description: "Michelangelo\'s Sistine Chapel"')
-            print('-----------------------------------------------------------------------------------------------------------')
-            s_idx: int = 1
-            for e in res_entities:
-                print_entity(e, s_idx, user_token, knowledge_client)
-        
-            # Now, let's search all artwork that has the art style self-portrait
-            res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token,
-                                                                            search_term=SELF_PORTRAIT_STYLE,
-                                                                            language_code=LanguageCode('en_US'), limit=1000)
-            art_style: Optional[ThingObject] = None
-            s_idx: int = 1
-            for entity in res_entities:
-                #  Entity must be a person and the label match with full string
-                if entity.concept_type == ART_STYLE_CLASS and SELF_PORTRAIT_STYLE in [l.content for l in entity.label]:
-                    art_style = entity
-                    break
-            res_entities, next_search_page = knowledge_client.search_relation(auth_key=user_token,
-                                                                              subject_uri=None,
-                                                                              relation=HAS_ART_STYLE,
-                                                                              object_uri=art_style.uri,
-                                                                              language_code=LanguageCode('en_US'))
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(' Search results.  Relation: relation:=has_topic  object_uri:= unknown')
-            print('-----------------------------------------------------------------------------------------------------------')
-            s_idx: int = 1
-            for e in res_entities:
-                print_entity(e, s_idx, user_token, knowledge_client, short=True)
-                s_idx += 1
-        
-            # Finally, the activation function retrieving the related identities to a pre-defined depth.
-            entities, relations = knowledge_client.activations(auth_key=user_token,
-                                                               uris=[leo.uri],
-                                                               depth=1)
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(f'Activation.  URI: {leo.uri}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            s_idx: int = 1
-            for e in res_entities:
-                print_entity(e, s_idx, user_token, knowledge_client)
-                s_idx += 1
-            # All relations
-            print('-----------------------------------------------------------------------------------------------------------')
-            for r in relations:
-                print(f'Subject: {r[0]} Predicate: {r[1]} Object: {r[2]}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            page_id = None
-        
-            # Listing all entities which have the type
-            idx: int = 1
-            while True:
-                # pull
-                entities, total_number, next_page_id = knowledge_client.listing(user_token, ART_STYLE_CLASS, page_id=page_id,
-                                                                                limit=100)
-                pulled_entities: int = len(entities)
-                entity_count += pulled_entities
-                print('-------------------------------------------------------------------------------------------------------')
-                print(f' Page: {page_number} Number of entities: {len(entities)}  ({entity_count}/{total_number}) '
-                      f'Next page id: {next_page_id}')
-                print('-------------------------------------------------------------------------------------------------------')
-                for e in entities:
-                    print_entity(e, idx, user_token, knowledge_client)
-                    idx += 1
-                if pulled_entities == 0:
-                    break
-                page_number += 1
-                page_id = next_page_id
-            print()
-            # Delete all personal entities for this user
-            while True:
-                # pull
-                entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
-                                                                                limit=100)
-                pulled_entities: int = len(entities)
-                if pulled_entities == 0:
-                    break
-                delete_uris: List[str] = [e.uri for e in entities]
-                print(f'Cleanup. Delete entities: {delete_uris}')
-                knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
-                page_number += 1
-                page_id = next_page_id
-            print('-----------------------------------------------------------------------------------------------------------')
-        ```
-        
-        ### Named Entity Linking 
-        
-        Performing Named Entity Linking (NEL) on text and Universal Ink Model.
-        
-        ```python
-        import argparse
-        from typing import List, Dict
-        
-        from knowledge.base.entity import LanguageCode
-        from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
-        from knowledge.nel.base import KnowledgeGraphEntity
-        from knowledge.nel.engine import WacomEntityLinkingEngine
-        from knowledge.services.graph import WacomKnowledgeService
-        
-        LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
-        TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
-        
-        
-        def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
-            """
-            Printing entity details.
-        
-            Parameters
-            ----------
-            entity: KnowledgeGraphEntity
-                Named entity
-            list_idx: int
-                Index with a list
-            auth_key: str
-                Authorization key
-            client: WacomKnowledgeService
-                Knowledge graph client
-            """
-            thing: ThingObject = knowledge_client.entity(auth_key=user_token, uri=entity.entity_source.uri)
-            print(f'[{list_idx}] - {e.ref_text} [{e.start_idx}-{e.end_idx}] : {thing.uri} <{thing.concept_type.iri}>')
-            if len(thing.label) > 0:
-                print('    | [Labels]')
-                for la in thing.label:
-                    print(f'    |     |- "{la.content}"@{la.language_code}')
-                print('    |')
-            if len(thing.label) > 0:
-                print('    | [Alias]')
-                for la in thing.alias:
-                    print(f'    |     |- "{la.content}"@{la.language_code}')
-                print('    |')
-            relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
-            if len(thing.data_properties) > 0:
-                print('    | [Attributes]')
-                for data_property, labels in thing.data_properties.items():
-                    print(f'    |    |- {data_property.iri}:')
-                    for li in labels:
-                        print(f'    |    |-- "{li.value}"@{li.language_code}')
-                print('    |')
-            if len(relations) > 0:
-                print('    | [Relations]')
-                for re in relations.values():
-                    print(f'    |--- {re.relation.iri}: ')
-                    print(f'           |- [Incoming]: {re.incoming_relations} ')
-                    print(f'           |- [Outgoing]: {re.outgoing_relations}')
-            print()
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom personal knowledge REST API Client
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
-                application_name="Named Entity Linking Knowledge access",
-                service_url=args.instance)
-            #  Wacom Named Entity Linking
-            nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
-                service_url=args.instance,
-                service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
-            )
-            # Use special tenant for testing:  Unit-test tenant
-            user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            entities: List[KnowledgeGraphEntity] = nel_client.\
-                link_personal_entities(auth_key=user_token, text=TEXT,
-                                       language_code=LANGUAGE_CODE)
-            idx: int = 1
-            print('-----------------------------------------------------------------------------------------------------------')
-            print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
-            print('-----------------------------------------------------------------------------------------------------------')
-            for e in entities:
-                print_entity(e, idx, user_token, knowledge_client)
-                idx += 1
-        
-        ```
-        
-        ### Access Management
-        
-        The sample shows, how access to entities can be shared with a group of users or the tenant.
-        
-        ```python
-        import argparse
-        from typing import List
-        from knowledge.base.entity import LanguageCode, Label, Description
-        from knowledge.base.ontology import OntologyClassReference, ThingObject
-        from knowledge.services.base import WacomServiceException
-        from knowledge.services.graph import WacomKnowledgeService
-        from knowledge.services.group import GroupManagementServiceAPI, Group
-        from knowledge.services.users import UserManagementServiceAPI
-        
-        # ------------------------------- User credential ----------------------------------------------------------------------
-        TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
-        
-        
-        def create_entity() -> ThingObject:
-            # Main labels for entity
-            topic_labels: List[Label] = [
-                Label('Hidden', LanguageCode('en_US')),
-                Label('Versteckt', LanguageCode('de_DE')),
-                Label('隠れた', LanguageCode('ja_JP'))
-            ]
-        
-            # Topic description
-            topic_description: List[Description] = [
-                Description('Hidden entity to explain access management.', LanguageCode('en_US')),
-                Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
-            ]
-            # Topic
-            topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
-            return topic_object
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
-                                help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom personal knowledge REST API Client
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
-                                                                            service_url=args.instance)
-            # User Management
-            user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
-            # Group Management
-            group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
-            admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            # Now, we create a users
-            u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
-            u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
-            u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
-        
-            # Now, let's create an entity
-            thing: ThingObject = create_entity()
-            entity_uri: str = knowledge_client.create_entity(u1_token, thing)
-            # Only user 1 can access the entity from cloud storage
-            my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
-            print(f'User is the owner of {my_thing.owner}')
-            # Now only user 1 has access to the personal entity
-            knowledge_client.entity(u1_token, entity_uri)
-            # Try to access the entity
-            try:
-                knowledge_client.entity(u2_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
-            # Try to access the entity
-            try:
-                knowledge_client.entity(u3_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 3 has no access to the personal entity of user 1. Exception: {we}")
-            # Now, user 1 creates a group
-            g: Group = group_management.create_group(u1_token, "test-group")
-            # Shares the join key with user 2 and user 2 joins
-            group_management.join_group(u2_token, g.id, g.join_key)
-            # Share entity with group
-            group_management.add_entity_to_group(u1_token, g.id, entity_uri)
-            # Now, user 2 should have access
-            other_thing: ThingObject = knowledge_client.entity(u2_token, entity_uri)
-            print(f'User 2 is the owner of the thing: {other_thing.owner}')
-            # Try to access the entity
-            try:
-                knowledge_client.entity(u3_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 3 still has no access to the personal entity of user 1. Exception: {we}")
-            # Un-share the entity
-            group_management.remove_entity_to_group(u1_token, g.id, entity_uri)
-            # Now, again no access
-            try:
-                knowledge_client.entity(u2_token, entity_uri)
-            except WacomServiceException as we:
-                print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
-            group_management.leave_group(u2_token, group_id=g.id)
-            # Now, share the entity with the whole tenant
-            my_thing.tenant_access_right.read = True
-            knowledge_client.update_entity(u1_token, my_thing)
-            # Now, all users can access the entity
-            knowledge_client.entity(u2_token, entity_uri)
-            knowledge_client.entity(u3_token, entity_uri)
-            # Finally, clean up
-            knowledge_client.delete_entity(u1_token, entity_uri, force=True)
-            # Remove users
-            user_management.delete_user(TENANT_KEY, u1.external_user_id, u1.id)
-            user_management.delete_user(TENANT_KEY, u2.external_user_id, u2.id)
-            user_management.delete_user(TENANT_KEY, u3.external_user_id, u3.id)
-        
-        ```
-        
-        ### Ontology Creation
-        
-        The samples show how the ontology can be extended and new entities can be added using the added classes.
-        
-        ```python
-        import argparse
-        from typing import List, Optional
-        
-        from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
-        from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
-            DataProperty
-        from knowledge.services.graph import WacomKnowledgeService
-        from knowledge.services.ontology import OntologyService
-        
-        # ------------------------------- Constants ----------------------------------------------------------------------------
-        LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
-        CONTEXT_NAME: str = 'core'
-        # Wacom Base Ontology Types
-        PERSON_TYPE: OntologyClassReference = OntologyClassReference.parse("wacom:core#Person")
-        # Demo Class
-        ARTIST_TYPE: OntologyClassReference = OntologyClassReference.parse("demo:creative#Artist")
-        # Demo Object property
-        IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
-        # Demo Data property
-        STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
-        
-        
-        def create_artist() -> ThingObject:
-            # Main labels for entity
-            topic_labels: List[Label] = [
-                Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
-            ]
-        
-            # Topic description
-            topic_description: List[Description] = [
-                Description('Hidden entity to explain access management.', LanguageCode('en_US')),
-                Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
-            ]
-        
-            data_property: DataProperty = DataProperty(content='Salaj',
-                                                       property_ref=STAGE_NAME,
-                                                       language_code=LanguageCode('en_US'))
-            # Topic
-            artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
-            artist.add_data_property(data_property)
-            return artist
-        
-        
-        if __name__ == '__main__':
-            parser = argparse.ArgumentParser()
-            parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
-                                required=True)
-            parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
-            args = parser.parse_args()
-            TENANT_KEY: str = args.tenant
-            EXTERNAL_USER_ID: str = args.user
-            # Wacom Ontology REST API Client
-            ontology_client: OntologyService = OntologyService(service_url=args.instance)
-            admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
-            knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
-                application_name="Ontology Creation Demo",
-                service_url=args.instance)
-            contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
-            if len(contexts) == 0:
-                # First, create a context for the ontology
-                ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
-                context_name: str = CONTEXT_NAME
-            else:
-                context_name: str = contexts[0].context
-            # Creating a class which is a subclass of a person
-            ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
-        
-            # Object properties
-            ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                                   reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
-                                                   ranges_cls=[PERSON_TYPE],
-                                                   inverse_of=None, subproperty_of=None)
-            # Data properties
-            ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
-                                                 reference=STAGE_NAME,
-                                                 domains_cls=[ARTIST_TYPE],
-                                                 ranges_cls=[DataPropertyType.STRING],
-                                                 subproperty_of=None)
-        
-            # Commit the changes of the ontology. This is very important to confirm changes.
-            ontology_client.commit(admin_token, CONTEXT_NAME)
-            # Trigger graph service. After the update the ontology is available and the new entities can be created
-            knowledge_client.ontology_update(admin_token)
-        
-            res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
-                                                                            language_code=LanguageCode('en_US'), limit=1000)
-            leo: Optional[ThingObject] = None
-            for entity in res_entities:
-                #  Entity must be a person and the label match with full string
-                if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
-                    leo = entity
-                    break
-        
-            artist_student: ThingObject = create_artist()
-            artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
-            knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
-        ```
-        
-        ## Tools
-        
-        The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
-        
-        ### Listing script
-        
-        Listing the entities for tenant. 
-        
-        ```bash
-        >> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-r, --relations (optional)_ -  Requesting the relations for each entity
-        
-        ### Export entities script
-        
-        Dump all entities of a user to a ndjson file. 
-        
-        ```bash
-        >> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
-                                knowledge.wacom.com)
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-r, --relations (optional)_ -  Requesting the relations for each entity
-        - _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
-        - _-p, --images (optional)_ - Include the images in the dump.
-        - _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
-         
-        ### Push entities script
-        
-        Pushing entities to knowledge graph.
-        
-        ```bash
-        >> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
-          
-        ### Reset
-        
-        Resets a tenant by removing entities, groups, and users. 
-        
-        ```bash
-        >> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
-        ```
-        
-        **Parameters:**
-        
-        - _-i INSTANCE, --instance INSTANCE_ - URL of instance
-        - _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
-        - _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
-        - _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
-          
-        # Documentation
-        
-        You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
-        API documentation is available [here](./docs/).
-        
-        ## Contributing
-        Contribution guidelines are still work in progress.
-        
-        ## License
-        [Apache License 2.0](LICENSE)
-        
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Wacom Personal Knowledge Library
+
+The library and the cloud services are still under development. 
+The required access tokens are only available for selected partner companies.
+
+> :warning:  Its is still under development, so **we do not recommend using it yet for production environments**. Moreover, it is not following any formal QA and release process, yet. :fire:
+
+## Introduction
+
+In knowledge management there is a distinction between data, information and knowledge.
+In the domain of digital ink this means:
+
+- **Data** - The equivalent would be the ink strokes
+- **Information** - After using handwriting-, shape-, math-, or other recognition processes ink strokes are converted into machine readable content, such as text, shapes, math representations, other other digital content
+- **Knowledge / Semantics** -  Beyond recognition content needs to be semantically analysed to become semantically understood based on a shared common knowledge.
+
+The following illustration shows the different layers of knowledge:
+![Levels of ink knowledge layers](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/knowledge-levels.png)
+
+For handling semantics, Wacom introduced the Wacom Personal Knowledge (WPK) cloud service to manage personal ontologies and its associated personal knowledge graph.
+
+This library provide simplified access to Wacom's personal knowledge cloud service.
+It contains:
+
+- Basic datastructures for Ontology object and entities from the knowledge graph
+- Clients for the REST APIs
+- Connector for Wikidata public knowledge graph
+
+**Ontology service:**
+
+- List all Ontology structures
+- Modify Ontology structures
+- Delete Ontology structures
+
+**Entity service:**
+
+- List all entities
+- Add entities to knowledge graph
+- Access object properties
+
+# Technology stack
+
+## Domain Knowledge
+
+The tasks of the ontology within Wacom's personal knowledge system is to formalised the domain the technology is used in, such as education-, smart home-, or creative domein.
+The domain model will be the foundation for the entities collected within the knowledge graph, describing real world concepts in a formal language understood by artificial intelligence system:
+
+- Foundation for structured data, knowledge representation as concepts and relations among concepts
+- Being explicit definitions of shared vocabularies for interoperability
+- Being actionable fragments of explicit knowledge that engines can use for inferencing (Reasoning)
+- Can be used for problem solving
+
+An ontology defines (specifies) the concepts, relationships, and other distinctions that are relevant for modelling a domain.
+
+## Knowledge Graph
+
+- Knowledge graph is generated from unstructured and structured knowledge sources
+- Contains all structured knowledge gathered from all sources
+- Foundation for all semantic algorithms
+
+## Semantic Technology
+
+- Extract knowledge from various sources (Connectors)
+- Linking words to knowledge entities from graph in a given text (Ontology-based Named Entity Linking)
+- Enables a smart search functionality which understands the context and finds related documents (Semantic Search)
+
+
+# Functionality
+
+## Access API
+
+The personal knowledge graph backend is implement as a multi-tenancy system.
+Thus, several tenants can be logically separated from each other and different organisations can build their one knowledge graph.
+
+![Tenant concept](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-concept.png)
+
+In general, a tenant with their users, groups, and entities are logically separated.
+Physically the entities are store in the same instance of the Wacom Personal Knowledge (WPK) backend database system.
+
+The user management is rather limited, each organisation must provide their own authentication service and user management.
+The backend only has a reference of the user (*“shadow user”*) by an **external user id**.
+
+The management of tenants is limited to the system owner - Wacom -, as it requires a **tenant management API** key.
+While users for each tenant can be created by the owner of the **Tenant API Key**.
+You will receive this token from the system owner after the creation of the tenant.
+
+
+> :warning: Store the **Tenant API Key** in a secure key store, as attackers can use the key to harm your system.
+
+
+The **Tenant API Key** should be only used by your authentication service to create shadow users and to login your user into the WPK backend.
+After a successful user login, you will receive a token which can be used by the user to create, update, or delete entities and relations.
+
+The following illustration summarizes the flows for creation of tenant and users:
+
+![Tenant and user creation](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/tenant-user-creation.png)
+
+The organisation itself needs to implement their own authentication service which:
+
+- handles the users and their passwords,
+- controls the personal data of the users,
+- connects the users with the WPK backend and share with them the user token.
+
+The WPK backend only manages the access levels of the entities and the group management for users.
+The illustration shows how the access token is received from the WPK endpoint:
+
+![Access token request.](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/access-token.png)
+
+# Entity API
+
+The entities used within the knowledge graph and the relationship among them is defined within an ontology that is manage with Wacom Ontology Management System (WOMS).
+
+An entity within the personal knowledge graphs consist of these major parts:
+
+- **Icon** - a visual representation of the entity, for instance a portrait of a person.
+- **URI** - a unique resource identifier of an entity in the graph.
+- **Type** - the type links to the defined concept class in the ontology.
+- **Labels** - labels are the word(s) use in a language for the concept.
+- **Description** - a short abstract that describes the entity.
+- **Literals** - literals are properties of an entity, such as first name of a person. The ontology defines all literals of the concept class as well as its data type.
+- **Relations** - the relationship among different entities is described using relations.
+
+The following illustration provides an example for an entity:
+
+![Entity description](https://github.com/Wacom-Developer/personal-knowledge-library/blob/main/assets/entity-description.png)
+
+## Entity content
+
+Entities in general are language-independent as across nationalities or cultures we only use different scripts and words for a shared instance of a concept.
+
+Let's take Leonardo da Vinci as an example.
+The ontology defines the concept of a Person, a human being.
+Now, in English its label would be _Leonardo da Vinci_, while in Japanese _レオナルド・ダ・ヴィンチ_.
+Moreover, he is also known as _Leonardo di ser Piero da Vinci_ or _ダ・ビンチ_.
+
+### Labels
+
+Now, in the given example all words that a assigned to the concept are labels.
+The label _Leonardo da Vinci_ is stored in the backend with an additional language code, e.g. _en_.
+
+There is always a main label, which refers to the most common or official name of entity.
+Another example would be Wacom, where _Wacom Co., Ltd._ is the official name while _Wacom_ is commonly used and be considered as an alias.
+
+>  :pushpin: For the language code the **ISO 639-1:2002**, codes for the representation of names of languages—Part 1: Alpha-2 code. Read more, [here](https://www.iso.org/standard/22109.html)
+
+## Samples
+
+### Entity handling
+
+This samples shows how to work with graph service.
+
+```python
+import argparse
+from typing import Optional, List, Dict
+
+from knowledge.base.entity import LanguageCode, Description, Label
+from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, ThingObject, ObjectProperty
+from knowledge.services.graph import WacomKnowledgeService
+
+# ------------------------------- Knowledge entities -------------------------------------------------------------------
+LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
+SELF_PORTRAIT_STYLE: str = 'self-portrait'
+ICON: str = "https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29."\
+            "JPG/1024px-Mona_Lisa_%28copy%2C_Thalwil%2C_Switzerland%29.JPG"
+# ------------------------------- Ontology class names -----------------------------------------------------------------
+THING_OBJECT: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Thing')
+"""
+The Ontology will contain a Thing class where is the root class in the hierarchy. 
+"""
+ARTWORK_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'creative', 'VisualArtwork')
+PERSON_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Person')
+ART_STYLE_CLASS: OntologyClassReference = OntologyClassReference.parse('wacom:creative#ArtStyle')
+IS_CREATOR: OntologyPropertyReference = OntologyPropertyReference('wacom', 'core', 'created')
+HAS_TOPIC: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#hasTopic')
+CREATED: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:core#created')
+HAS_ART_STYLE: OntologyPropertyReference = OntologyPropertyReference.parse('wacom:creative#hasArtstyle')
+
+
+def print_entity(entity: ThingObject, list_idx: int, auth_key: str, client: WacomKnowledgeService, short: bool = False):
+    """
+    Printing entity details.
+
+    Parameters
+    ----------
+    entity: ThingObject
+        Entity with properties
+    list_idx: int
+        Index with a list
+    auth_key: str
+        Authorization key
+    client: WacomKnowledgeService
+        Knowledge graph client
+    short: bool
+        Short summary
+    """
+    print(f'[{list_idx}] : {entity.uri} <{entity.concept_type.iri}>')
+    if len(entity.label) > 0:
+        print('    | [Labels]')
+        for la in entity.label:
+            print(f'    |     |- "{la.content}"@{la.language_code}')
+        print('    |')
+    if not short:
+        if len(entity.alias) > 0:
+            print('    | [Alias]')
+            for la in entity.alias:
+                print(f'    |     |- "{la.content}"@{la.language_code}')
+            print('    |')
+        if len(entity.data_properties) > 0:
+            print('    | [Attributes]')
+            for data_property, labels in entity.data_properties.items():
+                print(f'    |    |- {data_property.iri}:')
+                for li in labels:
+                    print(f'    |    |-- "{li.value}"@{li.language_code}')
+            print('    |')
+
+        relations_obj: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key,
+                                                                                          uri=entity.uri)
+        if len(relations_obj) > 0:
+            print('    | [Relations]')
+            for re in relations_obj.values():
+                print(f'    |--- {re.relation.iri}: ')
+                print(f'           |- [Incoming]: {re.incoming_relations} ')
+                print(f'           |- [Outgoing]: {re.outgoing_relations}')
+        print()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+                        help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom personal knowledge REST API Client
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
+                                                                    service_url=args.instance)
+    # Use special tenant for testing:  Unit-test tenant
+    user_token, refresh_token, expiration_time = knowledge_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    page_id: Optional[str] = None
+    page_number: int = 1
+    entity_count: int = 0
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' First step: Find Leonardo da Vinci in the knowledge graph.')
+    print('-----------------------------------------------------------------------------------------------------------')
+    res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token, search_term=LEONARDO_DA_VINCI,
+                                                                    language_code=LanguageCode('en_US'), limit=1000)
+    leo: Optional[ThingObject] = None
+    s_idx: int = 1
+    for entity in res_entities:
+        #  Entity must be a person and the label match with full string
+        if entity.concept_type == PERSON_CLASS and LEONARDO_DA_VINCI in [l.content for l in entity.label]:
+            leo = entity
+            break
+
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' What artwork exists in the knowledge graph.')
+    print('-----------------------------------------------------------------------------------------------------------')
+    relations_dict: Dict[OntologyPropertyReference, ObjectProperty] = knowledge_client.relations(auth_key=user_token,
+                                                                                                 uri=leo.uri)
+    print(f' Artwork of {leo.label}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    idx: int = 1
+    if CREATED in relations_dict:
+        for e in relations_dict[CREATED].outgoing_relations:
+            print(f' [{idx}] {e.uri}: {e.label}')
+            idx += 1
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' Let us create a new piece of artwork.')
+    print('-----------------------------------------------------------------------------------------------------------')
+
+    # Main labels for entity
+    artwork_labels: List[Label] = [
+        Label('Ginevra Gherardini', LanguageCode('en_US')),
+        Label('Ginevra Gherardini', LanguageCode('de_DE'))
+    ]
+    # Alias labels for entity
+    artwork_alias: List[Label] = [
+        Label("Ginevra", LanguageCode('en_US')),
+        Label("Ginevra", LanguageCode('de_DE'))
+    ]
+    # Topic description
+    artwork_description: List[Description] = [
+        Description('Oil painting of Mona Lisa\' sister', LanguageCode('en_US')),
+        Description('Ölgemälde von Mona Lisa\' Schwester', LanguageCode('de_DE'))
+    ]
+    # Topic
+    artwork_object: ThingObject = ThingObject(label=artwork_labels, concept_type=ARTWORK_CLASS,
+                                              description=artwork_description,
+                                              icon=ICON)
+    artwork_object.alias = artwork_alias
+    print(f' Create: {artwork_object}')
+    # Create artwork
+    artwork_entity_uri: str = knowledge_client.create_entity(user_token, artwork_object)
+    print(f' Entity URI: {artwork_entity_uri}')
+    # Create relation between Leonardo da Vinci and artwork
+    knowledge_client.create_relation(auth_key=user_token, source=leo.uri, relation=IS_CREATOR,
+                                     target=artwork_entity_uri)
+
+    relations_dict = knowledge_client.relations(auth_key=user_token, uri=artwork_entity_uri)
+    for ontology_property, object_property in relations_dict.items():
+        print(f'  {object_property}')
+    # You will see that wacom:core#isCreatedBy is automatically inferred as relation as it is the inverse property of
+    # wacom:core#created.
+
+    # Now, more search options
+    res_entities, next_search_page = knowledge_client.search_description(user_token, 'Michelangelo\'s Sistine Chapel',
+                                                                         LanguageCode('en_US'), limit=1000)
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' Search results.  Description: "Michelangelo\'s Sistine Chapel"')
+    print('-----------------------------------------------------------------------------------------------------------')
+    s_idx: int = 1
+    for e in res_entities:
+        print_entity(e, s_idx, user_token, knowledge_client)
+
+    # Now, let's search all artwork that has the art style self-portrait
+    res_entities, next_search_page = knowledge_client.search_labels(auth_key=user_token,
+                                                                    search_term=SELF_PORTRAIT_STYLE,
+                                                                    language_code=LanguageCode('en_US'), limit=1000)
+    art_style: Optional[ThingObject] = None
+    s_idx: int = 1
+    for entity in res_entities:
+        #  Entity must be a person and the label match with full string
+        if entity.concept_type == ART_STYLE_CLASS and SELF_PORTRAIT_STYLE in [l.content for l in entity.label]:
+            art_style = entity
+            break
+    res_entities, next_search_page = knowledge_client.search_relation(auth_key=user_token,
+                                                                      subject_uri=None,
+                                                                      relation=HAS_ART_STYLE,
+                                                                      object_uri=art_style.uri,
+                                                                      language_code=LanguageCode('en_US'))
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(' Search results.  Relation: relation:=has_topic  object_uri:= unknown')
+    print('-----------------------------------------------------------------------------------------------------------')
+    s_idx: int = 1
+    for e in res_entities:
+        print_entity(e, s_idx, user_token, knowledge_client, short=True)
+        s_idx += 1
+
+    # Finally, the activation function retrieving the related identities to a pre-defined depth.
+    entities, relations = knowledge_client.activations(auth_key=user_token,
+                                                       uris=[leo.uri],
+                                                       depth=1)
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(f'Activation.  URI: {leo.uri}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    s_idx: int = 1
+    for e in res_entities:
+        print_entity(e, s_idx, user_token, knowledge_client)
+        s_idx += 1
+    # All relations
+    print('-----------------------------------------------------------------------------------------------------------')
+    for r in relations:
+        print(f'Subject: {r[0]} Predicate: {r[1]} Object: {r[2]}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    page_id = None
+
+    # Listing all entities which have the type
+    idx: int = 1
+    while True:
+        # pull
+        entities, total_number, next_page_id = knowledge_client.listing(user_token, ART_STYLE_CLASS, page_id=page_id,
+                                                                        limit=100)
+        pulled_entities: int = len(entities)
+        entity_count += pulled_entities
+        print('-------------------------------------------------------------------------------------------------------')
+        print(f' Page: {page_number} Number of entities: {len(entities)}  ({entity_count}/{total_number}) '
+              f'Next page id: {next_page_id}')
+        print('-------------------------------------------------------------------------------------------------------')
+        for e in entities:
+            print_entity(e, idx, user_token, knowledge_client)
+            idx += 1
+        if pulled_entities == 0:
+            break
+        page_number += 1
+        page_id = next_page_id
+    print()
+    # Delete all personal entities for this user
+    while True:
+        # pull
+        entities, total_number, next_page_id = knowledge_client.listing(user_token, THING_OBJECT, page_id=page_id,
+                                                                        limit=100)
+        pulled_entities: int = len(entities)
+        if pulled_entities == 0:
+            break
+        delete_uris: List[str] = [e.uri for e in entities]
+        print(f'Cleanup. Delete entities: {delete_uris}')
+        knowledge_client.delete_entities(auth_key=user_token, uris=delete_uris, force=True)
+        page_number += 1
+        page_id = next_page_id
+    print('-----------------------------------------------------------------------------------------------------------')
+```
+
+### Named Entity Linking 
+
+Performing Named Entity Linking (NEL) on text and Universal Ink Model.
+
+```python
+import argparse
+from typing import List, Dict
+
+from knowledge.base.entity import LanguageCode
+from knowledge.base.ontology import OntologyPropertyReference, ThingObject, ObjectProperty
+from knowledge.nel.base import KnowledgeGraphEntity
+from knowledge.nel.engine import WacomEntityLinkingEngine
+from knowledge.services.graph import WacomKnowledgeService
+
+LANGUAGE_CODE: LanguageCode = LanguageCode("en_US")
+TEXT: str = "Leonardo da Vinci painted the Mona Lisa."
+
+
+def print_entity(entity: KnowledgeGraphEntity, list_idx: int, auth_key: str, client: WacomKnowledgeService):
+    """
+    Printing entity details.
+
+    Parameters
+    ----------
+    entity: KnowledgeGraphEntity
+        Named entity
+    list_idx: int
+        Index with a list
+    auth_key: str
+        Authorization key
+    client: WacomKnowledgeService
+        Knowledge graph client
+    """
+    thing: ThingObject = knowledge_client.entity(auth_key=user_token, uri=entity.entity_source.uri)
+    print(f'[{list_idx}] - {e.ref_text} [{e.start_idx}-{e.end_idx}] : {thing.uri} <{thing.concept_type.iri}>')
+    if len(thing.label) > 0:
+        print('    | [Labels]')
+        for la in thing.label:
+            print(f'    |     |- "{la.content}"@{la.language_code}')
+        print('    |')
+    if len(thing.label) > 0:
+        print('    | [Alias]')
+        for la in thing.alias:
+            print(f'    |     |- "{la.content}"@{la.language_code}')
+        print('    |')
+    relations: Dict[OntologyPropertyReference, ObjectProperty] = client.relations(auth_key=auth_key, uri=thing.uri)
+    if len(thing.data_properties) > 0:
+        print('    | [Attributes]')
+        for data_property, labels in thing.data_properties.items():
+            print(f'    |    |- {data_property.iri}:')
+            for li in labels:
+                print(f'    |    |-- "{li.value}"@{li.language_code}')
+        print('    |')
+    if len(relations) > 0:
+        print('    | [Relations]')
+        for re in relations.values():
+            print(f'    |--- {re.relation.iri}: ')
+            print(f'           |- [Incoming]: {re.incoming_relations} ')
+            print(f'           |- [Outgoing]: {re.outgoing_relations}')
+    print()
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom personal knowledge REST API Client
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
+        application_name="Named Entity Linking Knowledge access",
+        service_url=args.instance)
+    #  Wacom Named Entity Linking
+    nel_client: WacomEntityLinkingEngine = WacomEntityLinkingEngine(
+        service_url=args.instance,
+        service_endpoint=WacomEntityLinkingEngine.SERVICE_ENDPOINT
+    )
+    # Use special tenant for testing:  Unit-test tenant
+    user_token, refresh_token, expiration_time = nel_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    entities: List[KnowledgeGraphEntity] = nel_client.\
+        link_personal_entities(auth_key=user_token, text=TEXT,
+                               language_code=LANGUAGE_CODE)
+    idx: int = 1
+    print('-----------------------------------------------------------------------------------------------------------')
+    print(f'Text: "{TEXT}"@{LANGUAGE_CODE}')
+    print('-----------------------------------------------------------------------------------------------------------')
+    for e in entities:
+        print_entity(e, idx, user_token, knowledge_client)
+        idx += 1
+
+```
+
+### Access Management
+
+The sample shows, how access to entities can be shared with a group of users or the tenant.
+
+```python
+import argparse
+from typing import List
+from knowledge.base.entity import LanguageCode, Label, Description
+from knowledge.base.ontology import OntologyClassReference, ThingObject
+from knowledge.services.base import WacomServiceException
+from knowledge.services.graph import WacomKnowledgeService
+from knowledge.services.group import GroupManagementServiceAPI, Group
+from knowledge.services.users import UserManagementServiceAPI
+
+# ------------------------------- User credential ----------------------------------------------------------------------
+TOPIC_CLASS: OntologyClassReference = OntologyClassReference('wacom', 'core', 'Topic')
+
+
+def create_entity() -> ThingObject:
+    # Main labels for entity
+    topic_labels: List[Label] = [
+        Label('Hidden', LanguageCode('en_US')),
+        Label('Versteckt', LanguageCode('de_DE')),
+        Label('隠れた', LanguageCode('ja_JP'))
+    ]
+
+    # Topic description
+    topic_description: List[Description] = [
+        Description('Hidden entity to explain access management.', LanguageCode('en_US')),
+        Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
+    ]
+    # Topic
+    topic_object: ThingObject = ThingObject(label=topic_labels, concept_type=TOPIC_CLASS, description=topic_description)
+    return topic_object
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default='https://stage-private-knowledge.wacom.com',
+                        help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom personal knowledge REST API Client
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(application_name="Wacom Knowledge Listing",
+                                                                    service_url=args.instance)
+    # User Management
+    user_management: UserManagementServiceAPI = UserManagementServiceAPI(service_url=args.instance)
+    # Group Management
+    group_management: GroupManagementServiceAPI = GroupManagementServiceAPI(service_url=args.instance)
+    admin_token, refresh_token, expiration_time  = user_management.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    # Now, we create a users
+    u1, u1_token = user_management.create_user(TENANT_KEY, "u1")
+    u2, u2_token = user_management.create_user(TENANT_KEY, "u2")
+    u3, u3_token = user_management.create_user(TENANT_KEY, "u3")
+
+    # Now, let's create an entity
+    thing: ThingObject = create_entity()
+    entity_uri: str = knowledge_client.create_entity(u1_token, thing)
+    # Only user 1 can access the entity from cloud storage
+    my_thing: ThingObject = knowledge_client.entity(u1_token, entity_uri)
+    print(f'User is the owner of {my_thing.owner}')
+    # Now only user 1 has access to the personal entity
+    knowledge_client.entity(u1_token, entity_uri)
+    # Try to access the entity
+    try:
+        knowledge_client.entity(u2_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
+    # Try to access the entity
+    try:
+        knowledge_client.entity(u3_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 3 has no access to the personal entity of user 1. Exception: {we}")
+    # Now, user 1 creates a group
+    g: Group = group_management.create_group(u1_token, "test-group")
+    # Shares the join key with user 2 and user 2 joins
+    group_management.join_group(u2_token, g.id, g.join_key)
+    # Share entity with group
+    group_management.add_entity_to_group(u1_token, g.id, entity_uri)
+    # Now, user 2 should have access
+    other_thing: ThingObject = knowledge_client.entity(u2_token, entity_uri)
+    print(f'User 2 is the owner of the thing: {other_thing.owner}')
+    # Try to access the entity
+    try:
+        knowledge_client.entity(u3_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 3 still has no access to the personal entity of user 1. Exception: {we}")
+    # Un-share the entity
+    group_management.remove_entity_to_group(u1_token, g.id, entity_uri)
+    # Now, again no access
+    try:
+        knowledge_client.entity(u2_token, entity_uri)
+    except WacomServiceException as we:
+        print(f"Expected exception as user 2 has no access to the personal entity of user 1. Exception: {we}")
+    group_management.leave_group(u2_token, group_id=g.id)
+    # Now, share the entity with the whole tenant
+    my_thing.tenant_access_right.read = True
+    knowledge_client.update_entity(u1_token, my_thing)
+    # Now, all users can access the entity
+    knowledge_client.entity(u2_token, entity_uri)
+    knowledge_client.entity(u3_token, entity_uri)
+    # Finally, clean up
+    knowledge_client.delete_entity(u1_token, entity_uri, force=True)
+    # Remove users
+    user_management.delete_user(TENANT_KEY, u1.external_user_id, u1.id)
+    user_management.delete_user(TENANT_KEY, u2.external_user_id, u2.id)
+    user_management.delete_user(TENANT_KEY, u3.external_user_id, u3.id)
+
+```
+
+### Ontology Creation
+
+The samples show how the ontology can be extended and new entities can be added using the added classes.
+
+```python
+import argparse
+from typing import List, Optional
+
+from knowledge.base.entity import OntologyContext, Label, LanguageCode, Description
+from knowledge.base.ontology import DataPropertyType, OntologyClassReference, OntologyPropertyReference, ThingObject, \
+    DataProperty
+from knowledge.services.graph import WacomKnowledgeService
+from knowledge.services.ontology import OntologyService
+
+# ------------------------------- Constants ----------------------------------------------------------------------------
+LEONARDO_DA_VINCI: str = 'Leonardo da Vinci'
+CONTEXT_NAME: str = 'core'
+# Wacom Base Ontology Types
+PERSON_TYPE: OntologyClassReference = OntologyClassReference.parse("wacom:core#Person")
+# Demo Class
+ARTIST_TYPE: OntologyClassReference = OntologyClassReference.parse("demo:creative#Artist")
+# Demo Object property
+IS_INSPIRED_BY: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#isInspiredBy")
+# Demo Data property
+STAGE_NAME: OntologyPropertyReference = OntologyPropertyReference.parse("demo:creative#stageName")
+
+
+def create_artist() -> ThingObject:
+    # Main labels for entity
+    topic_labels: List[Label] = [
+        Label('Gian Giacomo Caprotti', LanguageCode('en_US'))
+    ]
+
+    # Topic description
+    topic_description: List[Description] = [
+        Description('Hidden entity to explain access management.', LanguageCode('en_US')),
+        Description('Verstecke Entität, um die Zugriffsteuerung zu erlären.', LanguageCode('de_DE'))
+    ]
+
+    data_property: DataProperty = DataProperty(content='Salaj',
+                                               property_ref=STAGE_NAME,
+                                               language_code=LanguageCode('en_US'))
+    # Topic
+    artist: ThingObject = ThingObject(label=topic_labels, concept_type=ARTIST_TYPE, description=topic_description)
+    artist.add_data_property(data_property)
+    return artist
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-u", "--user", help="External Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-t", "--tenant", help="Tenant Id of the shadow user within the Wacom Personal Knowledge.",
+                        required=True)
+    parser.add_argument("-i", "--instance", default="https://stage-private-knowledge.wacom.com", help="URL of instance")
+    args = parser.parse_args()
+    TENANT_KEY: str = args.tenant
+    EXTERNAL_USER_ID: str = args.user
+    # Wacom Ontology REST API Client
+    ontology_client: OntologyService = OntologyService(service_url=args.instance)
+    admin_token, refresh_token, expiration_time  = ontology_client.request_user_token(TENANT_KEY, EXTERNAL_USER_ID)
+    knowledge_client: WacomKnowledgeService = WacomKnowledgeService(
+        application_name="Ontology Creation Demo",
+        service_url=args.instance)
+    contexts: List[OntologyContext] = ontology_client.contexts(admin_token)
+    if len(contexts) == 0:
+        # First, create a context for the ontology
+        ontology_client.create_context(admin_token, name=CONTEXT_NAME, base_uri=f'demo:{CONTEXT_NAME}')
+        context_name: str = CONTEXT_NAME
+    else:
+        context_name: str = contexts[0].context
+    # Creating a class which is a subclass of a person
+    ontology_client.create_concept(admin_token, CONTEXT_NAME, reference=ARTIST_TYPE, subclass_of=PERSON_TYPE)
+
+    # Object properties
+    ontology_client.create_object_property(auth_key=admin_token, context=CONTEXT_NAME,
+                                           reference=IS_INSPIRED_BY, domains_cls=[ARTIST_TYPE], 
+                                           ranges_cls=[PERSON_TYPE],
+                                           inverse_of=None, subproperty_of=None)
+    # Data properties
+    ontology_client.create_data_property(auth_key=admin_token, context=CONTEXT_NAME,
+                                         reference=STAGE_NAME,
+                                         domains_cls=[ARTIST_TYPE],
+                                         ranges_cls=[DataPropertyType.STRING],
+                                         subproperty_of=None)
+
+    # Commit the changes of the ontology. This is very important to confirm changes.
+    ontology_client.commit(admin_token, CONTEXT_NAME)
+    # Trigger graph service. After the update the ontology is available and the new entities can be created
+    knowledge_client.ontology_update(admin_token)
+
+    res_entities, next_search_page = knowledge_client.search_labels(auth_key=admin_token, search_term=LEONARDO_DA_VINCI,
+                                                                    language_code=LanguageCode('en_US'), limit=1000)
+    leo: Optional[ThingObject] = None
+    for entity in res_entities:
+        #  Entity must be a person and the label match with full string
+        if entity.concept_type == PERSON_TYPE and LEONARDO_DA_VINCI in [la.content for la in entity.label]:
+            leo = entity
+            break
+
+    artist_student: ThingObject = create_artist()
+    artist_student_uri: str = knowledge_client.create_entity(admin_token, artist_student)
+    knowledge_client.create_relation(admin_token, artist_student_uri, IS_INSPIRED_BY, leo.uri)
+```
+
+## Tools
+
+The following samples show how to utilize the library to work with Wacom's Personal Knowledge.
+
+### Listing script
+
+Listing the entities for tenant. 
+
+```bash
+>> python listing.py [-h] -u USER -t TENANT [-r] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-r, --relations (optional)_ -  Requesting the relations for each entity
+
+### Export entities script
+
+Dump all entities of a user to a ndjson file. 
+
+```bash
+>> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
+                        knowledge.wacom.com)
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-r, --relations (optional)_ -  Requesting the relations for each entity
+- _-a, --all (optional)_ - All entities the user as access to, otherwise only his own entities are dumped.
+- _-p, --images (optional)_ - Include the images in the dump.
+- _-d DUMP, --dump DUMP_ -  Defines the location of the dump path.
+ 
+### Push entities script
+
+Pushing entities to knowledge graph.
+
+```bash
+>> python push_entities.py [-h] [-u USER] [-t TENANT] [-r] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.
+  
+### Reset
+
+Resets a tenant by removing entities, groups, and users. 
+
+```bash
+>> python reset.py [-h] [-u USER] [-t TENANT] [-i INSTANCE]
+```
+
+**Parameters:**
+
+- _-i INSTANCE, --instance INSTANCE_ - URL of instance
+- _-u USER, --user USER_ - External ID to identify user of the Wacom Personal Knowledge 
+- _-t TENANT, --tenant TENANT_ - Tenant key to identify tenant
+- _-i CACHE, --cache CACHE_ - Path to entities that must be imported.  
+  
+# Documentation
+
+You can find more detailed technical documentation, [here](https://developer-docs.wacom.com/preview/semantic-ink/).
+API documentation is available [here](./docs/).
+
+## Contributing
+Contribution guidelines are still work in progress.
+
+## License
+[Apache License 2.0](LICENSE)
+
+
```

### Comparing `personal_knowledge_library-0.9.5/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-0.9.6/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 knowledge/base/__init__.py
 knowledge/base/access.py
 knowledge/base/entity.py
 knowledge/base/ontology.py
 knowledge/nel/__init__.py
 knowledge/nel/base.py
 knowledge/nel/engine.py
+knowledge/ontomapping/__init__.py
+knowledge/ontomapping/manager.py
 knowledge/public/__init__.py
+knowledge/public/helper.py
+knowledge/public/relations.py
 knowledge/public/wikidata.py
 knowledge/services/__init__.py
 knowledge/services/base.py
 knowledge/services/graph.py
 knowledge/services/group.py
 knowledge/services/ontology.py
 knowledge/services/tenant.py
```

### Comparing `personal_knowledge_library-0.9.5/setup.py` & `personal_knowledge_library-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """.format(*(REQUIRED_PYTHON + CURRENT_PYTHON)))
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
@@ -43,21 +43,19 @@
     author_email='markus.weber@wacom.com',
     license='Apache 2.0 License',
     keywords='semantic-knowledge;knowledge-graph',
     packages=find_packages(exclude=('docs', 'tests', 'env')),
     include_package_data=True,
     install_requires=[
         "requests>=2.25.1",
-        "qwikidata>=0.4.2",
         "python-dateutil>=2.8.2",
-        "PyJWT==2.6.0",
+        "PyJWT>=2.6.0",
         "tqdm>=4.62.0",
         "ndjson>=0.3.1",
-        "rdflib>=6.3.1",
-        "iso639-lang"
+        "rdflib>=6.3.2"
     ],
     extras_require={
     },
     tests_require=(
         'pytest',
         'pytest-cov'
     ),
```


# Comparing `tmp/openassetio_mediacreation-1.0.0a4-py3-none-any.whl.zip` & `tmp/openassetio_mediacreation-1.0.0a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13687 bytes, number of entries: 12
--rw-r--r--  2.0 unx      188 b- defN 23-May-04 14:06 openassetio_mediacreation/__init__.py
--rw-r--r--  2.0 unx     6511 b- defN 23-May-04 14:06 openassetio_mediacreation/traits.yml
--rw-r--r--  2.0 unx      245 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/__init__.py
--rw-r--r--  2.0 unx     1799 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/content.py
--rw-r--r--  2.0 unx     3695 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/identity.py
--rw-r--r--  2.0 unx     3858 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/managementPolicy.py
--rw-r--r--  2.0 unx     2266 b- defN 23-May-04 14:06 openassetio_mediacreation/traits/timeline.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1435 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1184 b- defN 23-May-04 14:06 openassetio_mediacreation-1.0.0a4.dist-info/RECORD
-12 files, 32656 bytes uncompressed, 11635 bytes compressed:  64.4%
+Zip file size: 15055 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      188 b- defN 23-May-23 13:53 openassetio_mediacreation/__init__.py
+-rw-r--r--  2.0 unx     6511 b- defN 23-May-23 13:53 openassetio_mediacreation/traits.yml
+-rw-r--r--  2.0 unx      245 b- defN 23-May-23 13:53 openassetio_mediacreation/traits/__init__.py
+-rw-r--r--  2.0 unx     3084 b- defN 23-May-23 13:53 openassetio_mediacreation/traits/content.py
+-rw-r--r--  2.0 unx     4982 b- defN 23-May-23 13:53 openassetio_mediacreation/traits/identity.py
+-rw-r--r--  2.0 unx     6425 b- defN 23-May-23 13:53 openassetio_mediacreation/traits/managementPolicy.py
+-rw-r--r--  2.0 unx     6115 b- defN 23-May-23 13:53 openassetio_mediacreation/traits/timeline.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-23 13:53 openassetio_mediacreation-1.0.0a5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1435 b- defN 23-May-23 13:53 openassetio_mediacreation-1.0.0a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 13:53 openassetio_mediacreation-1.0.0a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 23-May-23 13:53 openassetio_mediacreation-1.0.0a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1184 b- defN 23-May-23 13:53 openassetio_mediacreation-1.0.0a5.dist-info/RECORD
+12 files, 41644 bytes uncompressed, 13003 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: openassetio_mediacreation/traits/managementPolicy.py
 Comment: 
 
 Filename: openassetio_mediacreation/traits/timeline.py
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a4.dist-info/LICENSE
+Filename: openassetio_mediacreation-1.0.0a5.dist-info/LICENSE
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a4.dist-info/METADATA
+Filename: openassetio_mediacreation-1.0.0a5.dist-info/METADATA
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a4.dist-info/WHEEL
+Filename: openassetio_mediacreation-1.0.0a5.dist-info/WHEEL
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a4.dist-info/top_level.txt
+Filename: openassetio_mediacreation-1.0.0a5.dist-info/top_level.txt
 Comment: 
 
-Filename: openassetio_mediacreation-1.0.0a4.dist-info/RECORD
+Filename: openassetio_mediacreation-1.0.0a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openassetio_mediacreation/traits/content.py

```diff
@@ -5,53 +5,98 @@
 Traits related to abstract content.
 """
 
 # WARNING: This file is auto-generated by openassetio-traitgen, do not edit.
 
 from typing import Union
 
-from openassetio import TraitBase
+from openassetio import TraitsData
 
 
-class LocatableContentTrait(TraitBase):
+class LocatableContentTrait:
     """
     This trait characterizes an entity whose data is persisted
     externally to the API through data accessible via a valid URL.
 
     The `location` property holds the most applicable location of the
     entity's content for the current process environment - considering
     platform, host, etc. Location is in the form of a URL.
     Usage: entity
     """
     kId = "openassetio-mediacreation:content.LocatableContent"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
     
     def setLocation(self, location: str):
         """
         Sets the location property.
 
         The location of the entities external content.
 
         This must be a valid URL so special characters need to be
         encoded.
         """
         if not isinstance(location, str):
             raise TypeError("location must be a 'str'.")
-        self._data.setTraitProperty(self.kId, "location", location)
+        self.__data.setTraitProperty(self.kId, "location", location)
 
     def getLocation(self, defaultValue: str=None) -> Union[str, None]:
         """
         Gets the value of the location property or the supplied default.
 
         The location of the entities external content.
 
         This must be a valid URL so special characters need to be
         encoded.
         """
-        value = self._data.getTraitProperty(self.kId, "location")
+        value = self.__data.getTraitProperty(self.kId, "location")
         if value is None:
             return defaultValue
 
         if not isinstance(value, str):
             if defaultValue is None:
                 raise TypeError(f"Invalid stored value type: '{type(value).__name__}' should be 'str'.")
             return defaultValue
```

## openassetio_mediacreation/traits/identity.py

```diff
@@ -5,54 +5,99 @@
 Traits that aid identification of an entity
 """
 
 # WARNING: This file is auto-generated by openassetio-traitgen, do not edit.
 
 from typing import Union
 
-from openassetio import TraitBase
+from openassetio import TraitsData
 
 
-class DisplayNameTrait(TraitBase):
+class DisplayNameTrait:
     """
     Names that can be presented to a user in order to identify and/or
     disambiguate the entity. These strings are potentially unstable and
     should not be used as a UUID or other persistent anchor.
     Usage: entity
     """
     kId = "openassetio-mediacreation:identity.DisplayName"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
     
     def setName(self, name: str):
         """
         Sets the name property.
 
         The humanized name of entity itself, not including any
         hierarchy or classification.
 
         For example:
         - `"Cuttlefish v1"` - for a version of an asset
         - `"seq003"` - for a sequence in a hierarchy
         """
         if not isinstance(name, str):
             raise TypeError("name must be a 'str'.")
-        self._data.setTraitProperty(self.kId, "name", name)
+        self.__data.setTraitProperty(self.kId, "name", name)
 
     def getName(self, defaultValue: str=None) -> Union[str, None]:
         """
         Gets the value of the name property or the supplied default.
 
         The humanized name of entity itself, not including any
         hierarchy or classification.
 
         For example:
         - `"Cuttlefish v1"` - for a version of an asset
         - `"seq003"` - for a sequence in a hierarchy
         """
-        value = self._data.getTraitProperty(self.kId, "name")
+        value = self.__data.getTraitProperty(self.kId, "name")
         if value is None:
             return defaultValue
 
         if not isinstance(value, str):
             if defaultValue is None:
                 raise TypeError(f"Invalid stored value type: '{type(value).__name__}' should be 'str'.")
             return defaultValue
@@ -72,15 +117,15 @@
         - `"dive / build / cuttlefish / model / v1"` for a version
             of an asset in an 'open recent' menu.
         - `"Sequence 003 [ Dive / Episode 1 ]"` for a sequence in
            an hierarchy as a window title.
         """
         if not isinstance(qualifiedName, str):
             raise TypeError("qualifiedName must be a 'str'.")
-        self._data.setTraitProperty(self.kId, "qualifiedName", qualifiedName)
+        self.__data.setTraitProperty(self.kId, "qualifiedName", qualifiedName)
 
     def getQualifiedName(self, defaultValue: str=None) -> Union[str, None]:
         """
         Gets the value of the qualifiedName property or the supplied default.
 
         An unambiguous, humanised name for the entity.
 
@@ -90,15 +135,15 @@
 
         For example:
         - `"dive / build / cuttlefish / model / v1"` for a version
             of an asset in an 'open recent' menu.
         - `"Sequence 003 [ Dive / Episode 1 ]"` for a sequence in
            an hierarchy as a window title.
         """
-        value = self._data.getTraitProperty(self.kId, "qualifiedName")
+        value = self.__data.getTraitProperty(self.kId, "qualifiedName")
         if value is None:
             return defaultValue
 
         if not isinstance(value, str):
             if defaultValue is None:
                 raise TypeError(f"Invalid stored value type: '{type(value).__name__}' should be 'str'.")
             return defaultValue
```

## openassetio_mediacreation/traits/managementPolicy.py

```diff
@@ -5,18 +5,18 @@
 Traits used in a Manager's managementPolicy response.
 """
 
 # WARNING: This file is auto-generated by openassetio-traitgen, do not edit.
 
 from typing import Union
 
-from openassetio import TraitBase
+from openassetio import TraitsData
 
 
-class ManagedTrait(TraitBase):
+class ManagedTrait:
     """
     A trait indicating that the data matching the supplied trait set is
     handled by the manager.
 
     There are three possible policies determined by applying/querying
     this trait: * If the response is not imbued with this trait, then
     the
@@ -31,14 +31,59 @@
       * If  the "exclusive" property is set to true, then the Manager
         takes exclusive control over data with the queried trait set,
         and any standard host interfaces etc should be suppressed.
     Usage: managementPolicy
     """
     kId = "openassetio-mediacreation:managementPolicy.Managed"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
     
     def setExclusive(self, exclusive: bool):
         """
         Sets the exclusive property.
 
         Determines if the manager exclusively handles data matching the
         supplied trait set.
@@ -48,15 +93,15 @@
         determining where to load/save data.
 
         If False, then standard host controls can be presented in
         addition to any custom manager UI.
         """
         if not isinstance(exclusive, bool):
             raise TypeError("exclusive must be a 'bool'.")
-        self._data.setTraitProperty(self.kId, "exclusive", exclusive)
+        self.__data.setTraitProperty(self.kId, "exclusive", exclusive)
 
     def getExclusive(self, defaultValue: bool=None) -> Union[bool, None]:
         """
         Gets the value of the exclusive property or the supplied default.
 
         Determines if the manager exclusively handles data matching the
         supplied trait set.
@@ -64,28 +109,28 @@
         If True, then standard host contols should be disabled in favour
         of manager delegated UI. For example, file system browsers when
         determining where to load/save data.
 
         If False, then standard host controls can be presented in
         addition to any custom manager UI.
         """
-        value = self._data.getTraitProperty(self.kId, "exclusive")
+        value = self.__data.getTraitProperty(self.kId, "exclusive")
         if value is None:
             return defaultValue
 
         if not isinstance(value, bool):
             if defaultValue is None:
                 raise TypeError(f"Invalid stored value type: '{type(value).__name__}' should be 'bool'.")
             return defaultValue
         return value
         
     
 
 
-class ResolvesFutureEntitiesTrait(TraitBase):
+class ResolvesFutureEntitiesTrait:
     """
     A trait indicating a manager can potentially resolve the supplied
     trait set for future entities.
 
     If not imbued, the manager is not capable of determining data in
     advance for new entities, and is only capable of resolving traits
     for exising ones.
@@ -97,9 +142,54 @@
     working entity reference supplied by preflight in order to determine
     a suitable output path before work is done. In its absence, a host
     must use alternate means to determine a suitable output location.
     Usage: managementPolicy
     """
     kId = "openassetio-mediacreation:managementPolicy.ResolvesFutureEntities"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
```

## openassetio_mediacreation/traits/timeline.py

```diff
@@ -5,77 +5,212 @@
 Traits related to timelines.
 """
 
 # WARNING: This file is auto-generated by openassetio-traitgen, do not edit.
 
 from typing import Union
 
-from openassetio import TraitBase
+from openassetio import TraitsData
 
 
-class ClipTrait(TraitBase):
+class ClipTrait:
     """
     This trait characterizes the use of some range of external media,
     commonly on a track or timeline. Frequently used in non-linear
     editing environments such as Video and Audio production tools.
 
     TODO(TC) Define any additional properties, and companion traits such
     as 'frameRange' and 'handles'.
     Usage: entity, locale
     """
     kId = "openassetio-mediacreation:timeline.Clip"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
     
     def setName(self, name: str):
         """
         Sets the name property.
 
         The name of the clip.
         """
         if not isinstance(name, str):
             raise TypeError("name must be a 'str'.")
-        self._data.setTraitProperty(self.kId, "name", name)
+        self.__data.setTraitProperty(self.kId, "name", name)
 
     def getName(self, defaultValue: str=None) -> Union[str, None]:
         """
         Gets the value of the name property or the supplied default.
 
         The name of the clip.
         """
-        value = self._data.getTraitProperty(self.kId, "name")
+        value = self.__data.getTraitProperty(self.kId, "name")
         if value is None:
             return defaultValue
 
         if not isinstance(value, str):
             if defaultValue is None:
                 raise TypeError(f"Invalid stored value type: '{type(value).__name__}' should be 'str'.")
             return defaultValue
         return value
         
     
 
 
-class TimelineTrait(TraitBase):
+class TimelineTrait:
     """
     This trait characterizes a collection of tracks that evaluate
     concurrently to form layers of references to media. Frequently used
     in non-linear editing environments such as Video and Audio post
     production tools.
     Usage: entity, locale
     """
     kId = "openassetio-mediacreation:timeline.Timeline"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
     
 
 
-class TrackTrait(TraitBase):
+class TrackTrait:
     """
     This trait characterizes a lane or collection of media, arranged
     temporally such that only a single item in the collection is active
     at any given time. Frequently used in non-linear editing
     environments such as Video and Audio post production tools.
     Usage: entity, locale
     """
     kId = "openassetio-mediacreation:timeline.Track"
 
+    def __init__(self, traitsData):
+        """
+        Construct this trait view, wrapping the given data.
+
+        @param traitsData @fqref{TraitsData}} "TraitsData" The target
+        data that holds/will hold the traits properties.
+        """
+        self.__data = traitsData
+
+    def isImbued(self):
+        """
+        Checks whether the data this trait has been applied to
+        actually has this trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return self.isImbuedTo(self.__data)
+
+    @classmethod
+    def isImbuedTo(cls, traitsData):
+        """
+        Checks whether the given data actually has this trait.
+        @param traitsData: Data to check for trait.
+        @return `True` if the underlying data has this trait, `False`
+        otherwise.
+        """
+        return traitsData.hasTrait(cls.kId)
+
+    def imbue(self):
+        """
+        Adds this trait to the held data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        self.__data.addTrait(self.kId)
+
+    @classmethod
+    def imbueTo(cls, traitsData):
+        """
+        Adds this trait to the provided data.
+
+        If the data already has this trait, it is a no-op.
+        """
+        traitsData.addTrait(cls.kId)
+
```

## Comparing `openassetio_mediacreation-1.0.0a4.dist-info/LICENSE` & `openassetio_mediacreation-1.0.0a5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openassetio_mediacreation-1.0.0a4.dist-info/METADATA` & `openassetio_mediacreation-1.0.0a5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassetio-mediacreation
-Version: 1.0.0a4
+Version: 1.0.0a5
 Author-email: Contributors to the OpenAssetIO project <openassetio-discussion@lists.aswf.io>
 Project-URL: OpenAssetIO, https://github.com/OpenAssetIO/OpenAssetIO
 Project-URL: Source, https://github.com/OpenAssetIO/OpenAssetIO-MediaCreation
 Project-URL: Issues, https://github.com/OpenAssetIO/OpenAssetIO-MediaCreation/issues
 Keywords: openassetio,mediacreation,trait
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `openassetio_mediacreation-1.0.0a4.dist-info/RECORD` & `openassetio_mediacreation-1.0.0a5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openassetio_mediacreation/__init__.py,sha256=b36NTLJZmYaj3l4k8veMMRaPokuvK14r8uNPrzQHgDM,188
 openassetio_mediacreation/traits.yml,sha256=pVElMrhNQC-sHZMPbbjTsjzAf9llok7ieTJoZnglovY,6511
 openassetio_mediacreation/traits/__init__.py,sha256=8saXUuM5QygSsob839NLYrMDY95t0GUvkmmecgVFTlM,245
-openassetio_mediacreation/traits/content.py,sha256=iXirrok8GUdDjUJzB_HSYj4wcgpmYv7YmCGzgM_XcfI,1799
-openassetio_mediacreation/traits/identity.py,sha256=SEFLRoVz5EtA1FOQcTbYG4WUug1iFXOHlzyhQuxIVeQ,3695
-openassetio_mediacreation/traits/managementPolicy.py,sha256=L1-2ZQmEjurdK1HqwMQjUZ3tHRaqm4t388a1lw2ejfo,3858
-openassetio_mediacreation/traits/timeline.py,sha256=rBy_oMEjtJGvoLWfoRGPobEHvjxgulp7RDDDn5m2SzY,2266
-openassetio_mediacreation-1.0.0a4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-openassetio_mediacreation-1.0.0a4.dist-info/METADATA,sha256=ZPtwS01GmZpFnXYI3302GrGeiPru1vYhcvKNTu-zF1U,1435
-openassetio_mediacreation-1.0.0a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openassetio_mediacreation-1.0.0a4.dist-info/top_level.txt,sha256=6wrwB2f-cI98-MIfAnoKwTFdaYJQv206KEx50rAT7D0,26
-openassetio_mediacreation-1.0.0a4.dist-info/RECORD,,
+openassetio_mediacreation/traits/content.py,sha256=6JlQRaBfd89oIXcZgZ2oBuf9g1R0lRxHsoZ_OPzkHFc,3084
+openassetio_mediacreation/traits/identity.py,sha256=TKFyT_lI-_weRsIi-4mruwv-b24fxJHtFwQhPlfI-ww,4982
+openassetio_mediacreation/traits/managementPolicy.py,sha256=1ncGIJXPj_MmmGR767JjyjVxZzf9pviSD86_1rparPM,6425
+openassetio_mediacreation/traits/timeline.py,sha256=Abn8fidQZBHIlnZ4fxxSaEu7IneEgpsQI6qyIW-oDms,6115
+openassetio_mediacreation-1.0.0a5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+openassetio_mediacreation-1.0.0a5.dist-info/METADATA,sha256=GH48qUIRc42-0RvF-qkOPuS1nS2QKm8k6bQWoINE104,1435
+openassetio_mediacreation-1.0.0a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openassetio_mediacreation-1.0.0a5.dist-info/top_level.txt,sha256=6wrwB2f-cI98-MIfAnoKwTFdaYJQv206KEx50rAT7D0,26
+openassetio_mediacreation-1.0.0a5.dist-info/RECORD,,
```

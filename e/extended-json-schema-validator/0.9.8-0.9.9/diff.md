# Comparing `tmp/extended_json_schema_validator-0.9.8.tar.gz` & `tmp/extended_json_schema_validator-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extended_json_schema_validator-0.9.8.tar", last modified: Thu Sep 30 13:15:54 2021, max compression
+gzip compressed data, was "extended_json_schema_validator-0.9.9.tar", last modified: Thu Sep 30 18:16:50 2021, max compression
```

## Comparing `extended_json_schema_validator-0.9.8.tar` & `extended_json_schema_validator-0.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 13:15:54.529147 extended_json_schema_validator-0.9.8/
--rw-r--r--   0 jmfernandez (10012) users      (100)    26526 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.8/LICENSE
--rw-r--r--   0 jmfernandez (10012) users      (100)       58 2021-09-29 11:06:48.000000 extended_json_schema_validator-0.9.8/MANIFEST.in
--rw-r--r--   0 jmfernandez (10012) users      (100)     4212 2021-09-30 13:15:54.528147 extended_json_schema_validator-0.9.8/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)     3561 2021-09-29 10:50:46.000000 extended_json_schema_validator-0.9.8/README.md
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 13:15:54.509147 extended_json_schema_validator-0.9.8/extended_json_schema_validator/
--rw-r--r--   0 jmfernandez (10012) users      (100)       97 2021-09-30 13:11:43.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/__init__.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     7390 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extend_validator_helpers.py
--rw-r--r--   0 jmfernandez (10012) users      (100)    25829 2021-09-30 13:11:24.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensible_validator.py
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 13:15:54.525147 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/
--rw-r--r--   0 jmfernandez (10012) users      (100)        0 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/__init__.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     2320 2021-09-28 12:25:36.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/abstract_check.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     6892 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/fk_check.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     5924 2021-09-28 12:30:05.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/pk_check.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     6195 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/unique_check.py
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 13:15:54.509147 extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/
--rw-r--r--   0 jmfernandez (10012) users      (100)     4212 2021-09-30 13:15:54.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)      792 2021-09-30 13:15:54.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/SOURCES.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)        1 2021-09-30 13:15:54.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/dependency_links.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       42 2021-09-30 13:15:54.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/requires.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       31 2021-09-30 13:15:54.000000 extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/top_level.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)     5945 2021-09-29 13:13:52.000000 extended_json_schema_validator-0.9.8/jsonValidate.py
--rw-r--r--   0 jmfernandez (10012) users      (100)       98 2021-09-29 09:44:18.000000 extended_json_schema_validator-0.9.8/pyproject.toml
--rw-r--r--   0 jmfernandez (10012) users      (100)      130 2021-09-28 11:09:05.000000 extended_json_schema_validator-0.9.8/requirements.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       38 2021-09-30 13:15:54.529147 extended_json_schema_validator-0.9.8/setup.cfg
--rw-r--r--   0 jmfernandez (10012) users      (100)     1613 2021-09-29 10:53:58.000000 extended_json_schema_validator-0.9.8/setup.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 18:16:50.482550 extended_json_schema_validator-0.9.9/
+-rw-r--r--   0 jmfernandez (10012) users      (100)    26526 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.9/LICENSE
+-rw-r--r--   0 jmfernandez (10012) users      (100)       58 2021-09-29 11:06:48.000000 extended_json_schema_validator-0.9.9/MANIFEST.in
+-rw-r--r--   0 jmfernandez (10012) users      (100)     4355 2021-09-30 18:16:50.481550 extended_json_schema_validator-0.9.9/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)     3704 2021-09-30 17:49:19.000000 extended_json_schema_validator-0.9.9/README.md
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 18:16:50.480550 extended_json_schema_validator-0.9.9/extended_json_schema_validator/
+-rw-r--r--   0 jmfernandez (10012) users      (100)       97 2021-09-30 17:33:01.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/__init__.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     7432 2021-09-30 17:15:35.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extend_validator_helpers.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)    25877 2021-09-30 15:48:00.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensible_validator.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 18:16:50.481550 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/
+-rw-r--r--   0 jmfernandez (10012) users      (100)        0 2021-09-28 09:49:51.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/__init__.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     2352 2021-09-30 15:51:39.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/abstract_check.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     6917 2021-09-30 15:50:03.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/fk_check.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     5948 2021-09-30 15:51:04.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/pk_check.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     6066 2021-09-30 17:27:45.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/unique_check.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2021-09-30 18:16:50.481550 extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/
+-rw-r--r--   0 jmfernandez (10012) users      (100)     4355 2021-09-30 18:16:50.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)      792 2021-09-30 18:16:50.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)        1 2021-09-30 18:16:50.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       42 2021-09-30 18:16:50.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/requires.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       31 2021-09-30 18:16:50.000000 extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/top_level.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)     6212 2021-09-30 17:13:11.000000 extended_json_schema_validator-0.9.9/jsonValidate.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)       98 2021-09-29 09:44:18.000000 extended_json_schema_validator-0.9.9/pyproject.toml
+-rw-r--r--   0 jmfernandez (10012) users      (100)      130 2021-09-28 11:09:05.000000 extended_json_schema_validator-0.9.9/requirements.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       38 2021-09-30 18:16:50.482550 extended_json_schema_validator-0.9.9/setup.cfg
+-rw-r--r--   0 jmfernandez (10012) users      (100)     1613 2021-09-29 10:53:58.000000 extended_json_schema_validator-0.9.9/setup.py
```

### Comparing `extended_json_schema_validator-0.9.8/LICENSE` & `extended_json_schema_validator-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `extended_json_schema_validator-0.9.8/PKG-INFO` & `extended_json_schema_validator-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extended_json_schema_validator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Extended JSON Schema Validator
 Home-page: https://github.com/inab/python-extended-json-schema-validator
 Author: José Mª Fernández
 Author-email: jose.m.fernandez@bsc.es
 License: LGPLv2
 Project-URL: Bug Tracker, https://github.com/inab/python-extended-json-schema-validator/issues
 Platform: UNKNOWN
@@ -34,19 +34,19 @@
 ## Usage
 
 ```bash
 python jsonValidate.py --help
 ```
 ```
 usage: jsonValidate.py [-h] [--log-file LOGFILENAME] [--log-format LOGFORMAT] [-q] [-v] [-d] [-C CONFIGFILENAME]
-                       [--cache-dir CACHEDIR] [--report REPORTFILENAME] [--verbose-report] [--invalidate]
+                       [--cache-dir CACHEDIR] [--report REPORTFILENAME] [--verbose-report] [--invalidate | --read-only]
                        [--warm-up | --lazy-load] [-V]
                        json_schema_or_dir [json_file_or_dir [json_file_or_dir ...]]
 
-Validate JSON against JSON Schemas with extensions (version 0.9.7)
+Validate JSON against JSON Schemas with extensions (version 0.9.9)
 
 positional arguments:
   json_schema_or_dir    The JSON Schema file or directory to validate and use
   json_file_or_dir      The JSON files or directories to be validated
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -60,14 +60,15 @@
   -C CONFIGFILENAME, --config CONFIGFILENAME
                         Configuration file (used by extensions)
   --cache-dir CACHEDIR  Caching directory (used by extensions)
   --report REPORTFILENAME
                         Store validation report (in JSON format) in a file
   --verbose-report      When this flag is enabled, the report also embeds the json contents which were validated
   --invalidate          Caches are invalidated on startup
+  --read-only           When this flag is enabled, the caches are read-only, avoiding expensive operations related to the caches
   --warm-up             Caches are warmed up on startup
   --lazy-load           Caches are warmed up in a lazy way
   -V, --version         show program's version number and exit
 ```
 
 Next lines run validations using test data:
```

### Comparing `extended_json_schema_validator-0.9.8/README.md` & `extended_json_schema_validator-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 ## Usage
 
 ```bash
 python jsonValidate.py --help
 ```
 ```
 usage: jsonValidate.py [-h] [--log-file LOGFILENAME] [--log-format LOGFORMAT] [-q] [-v] [-d] [-C CONFIGFILENAME]
-                       [--cache-dir CACHEDIR] [--report REPORTFILENAME] [--verbose-report] [--invalidate]
+                       [--cache-dir CACHEDIR] [--report REPORTFILENAME] [--verbose-report] [--invalidate | --read-only]
                        [--warm-up | --lazy-load] [-V]
                        json_schema_or_dir [json_file_or_dir [json_file_or_dir ...]]
 
-Validate JSON against JSON Schemas with extensions (version 0.9.7)
+Validate JSON against JSON Schemas with extensions (version 0.9.9)
 
 positional arguments:
   json_schema_or_dir    The JSON Schema file or directory to validate and use
   json_file_or_dir      The JSON files or directories to be validated
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -43,14 +43,15 @@
   -C CONFIGFILENAME, --config CONFIGFILENAME
                         Configuration file (used by extensions)
   --cache-dir CACHEDIR  Caching directory (used by extensions)
   --report REPORTFILENAME
                         Store validation report (in JSON format) in a file
   --verbose-report      When this flag is enabled, the report also embeds the json contents which were validated
   --invalidate          Caches are invalidated on startup
+  --read-only           When this flag is enabled, the caches are read-only, avoiding expensive operations related to the caches
   --warm-up             Caches are warmed up on startup
   --lazy-load           Caches are warmed up in a lazy way
   -V, --version         show program's version number and exit
 ```
 
 Next lines run validations using test data:
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator/extend_validator_helpers.py` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator/extend_validator_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 	'http://json-schema.org/draft-06/schema#': JSV.validators.Draft6Validator,
 	'http://json-schema.org/draft-06/hyper-schema#': JSV.validators.Draft4Validator,
 	'http://json-schema.org/draft-07/schema#': JSV.validators.Draft7Validator,
 	'http://json-schema.org/draft-07/hyper-schema#': JSV.validators.Draft7Validator
 }
 
 
-def extendValidator(schemaURI, validator, inputCustomTypes, inputCustomValidators,config={}, jsonSchemaSource='(unknown)'):
+def extendValidator(schemaURI, validator, inputCustomTypes, inputCustomValidators,config={}, jsonSchemaSource='(unknown)', isRW=True):
 	extendedValidators = validator.VALIDATORS.copy()
 	customValidatorsInstances = []
 	
 	# Validators which must be instantiated
 	if None in inputCustomValidators:
 		instancedCustomValidators = inputCustomValidators.copy()
 		
 		# Removing the special entry
 		del instancedCustomValidators[None]
 		
 		# Now, populating
 		for dynamicValidatorClass in inputCustomValidators[None]:
-			dynamicValidator = dynamicValidatorClass(schemaURI,jsonSchemaSource,config)
+			dynamicValidator = dynamicValidatorClass(schemaURI,jsonSchemaSource, config=config, isRW=isRW)
 			customValidatorsInstances.append(dynamicValidator)
 			
 			for triggerAttribute,triggeredValidation in dynamicValidator.getValidators():
 				if triggerAttribute in instancedCustomValidators:
 					raise AssertionError("FATAL: Two custom validators are using the same triggering attribute: {}".format(triggerAttribute))
 				
 				# The method must exist, and accept the parameters
@@ -57,17 +57,17 @@
 REF_FEATURE='$ref'
 
 # It returns the set of values' ids 
 def traverseJSONSchema(jsonObj, schemaURI=None, keys=set(), fragment=None, refSchemaListSet={}):
 	# Should we try getting it?
 	if schemaURI is None:
 		if isinstance(jsonObj,dict):
-			startingSchemaURI = j.get('$id')
+			startingSchemaURI = jsonObj.get('$id')
 			if startingSchemaURI is None:
-				startingSchemaURI = j.get('id')
+				startingSchemaURI = jsonObj.get('id')
 			
 			# End / fail fast
 			if startingSchemaURI is None:
 				return None
 			
 			schemaURI , fragment = uritools.uridefrag(startingSchemaURI)
 		else:
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensible_validator.py` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensible_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	SCHEMA_KEY = '$schema'
 	ALT_SCHEMA_KEYS = [
 		'@schema',
 		'_schema',
 		SCHEMA_KEY
 	]
 	
-	def __init__(self, customFormats=[], customTypes={}, customValidators=CustomBaseValidators, config={}, jsonRootTag=None):
+	def __init__(self, customFormats=[], customTypes={}, customValidators=CustomBaseValidators, config={}, jsonRootTag=None, isRW = True):
 		self.logger = logging.getLogger(self.__class__.__name__)
 		
 		self.schemaHash = {}
 		self.refSchemaCache = {}
 		self.refSchemaSet = {}
 		self.customFormatCheckerInstance = JSV.FormatChecker()
 
@@ -45,14 +45,15 @@
 		for customFormat in customFormats:
 			self.customFormatCheckerInstance.checks(customFormat.FormatName)(customFormat.IsCorrectFormat)
 		
 		self.customTypes = customTypes
 		self.customValidators = customValidators
 		self.config = config
 		self.jsonRootTag = jsonRootTag
+		self.isRW = isRW
 		self.doNotValidateNoId = not bool(config.get('validate-no-id',True))
 	
 	def loadJSONSchemas(self, *args, verbose=None):
 		p_schemaHash = self.schemaHash
 		# Schema validation stats
 		numDirOK = 0
 		numDirFail = 0
@@ -197,15 +198,15 @@
 			schemaValId = jsonSchema.get(self.SCHEMA_KEY)
 			plain_validator = PLAIN_VALIDATOR_MAPPER.get(schemaValId)
 			
 			# Getting the JSON Schema URI, needed by this
 			idKey = '$id'  if '$id' in jsonSchema else 'id'
 			jsonSchemaURI = jsonSchema.get(idKey)
 			
-			validator , customFormatInstances = extendValidator(jsonSchemaURI, plain_validator, self.customTypes, self.customValidators, config=self.config, jsonSchemaSource=jsonSchemaFile)
+			validator , customFormatInstances = extendValidator(jsonSchemaURI, plain_validator, self.customTypes, self.customValidators, config=self.config, jsonSchemaSource=jsonSchemaFile, isRW=self.isRW)
 			
 			schemaObj['customFormatInstances'] = customFormatInstances
 			schemaObj['validator'] = validator
 			
 			# Validate the extended JSON schema properly
 			metaSchema = validator.META_SCHEMA
 			if len(customFormatInstances) > 0:
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/abstract_check.py` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/abstract_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 import copy
 import logging
 
 CheckContext = namedtuple('CheckContext',['schemaURI','context'])
 
 class AbstractCustomFeatureValidator(abc.ABC):
-	def __init__(self, schemaURI, jsonSchemaSource='(unknown)', config = {}):
+	def __init__(self, schemaURI, jsonSchemaSource='(unknown)', config = {}, isRW = True):
 		self.logger = logging.getLogger(self.__class__.__name__)
 		
 		self.schemaURI = schemaURI
 		self.jsonSchemaSource = jsonSchemaSource
 		self.config = config
+		self.isRW = isRW
 		self.bootstrapMessages = None
 		self.currentJSONFile = '(unset)'
 
 	@abc.abstractmethod
 	def validate(self,validator,schema_attr_val,value,schema):
 		pass
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/fk_check.py` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/fk_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 class ForeignKey(AbstractCustomFeatureValidator):
 	KeyAttributeName = 'foreign_keys'
 	SchemaErrorReason = 'stale_fk'
 	DanglingFKErrorReason = 'dangling_fk'
 	
 	# Each instance represents the set of keys from one ore more JSON Schemas
-	def __init__(self,schemaURI, jsonSchemaSource='(unknown)',config={}):
-		super().__init__(schemaURI,jsonSchemaSource,config)
+	def __init__(self,schemaURI, jsonSchemaSource='(unknown)', config={}, isRW=True):
+		super().__init__(schemaURI, jsonSchemaSource, config, isRW=isRW)
 		self.FKWorld = dict()
 	
 	@property
 	def triggerAttribute(self):
 		return self.KeyAttributeName
 	
 	@property
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/pk_check.py` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/pk_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import codecs
 
 class PrimaryKey(UniqueKey):
 	KeyAttributeName = 'primary_key'
 	SchemaErrorReason = 'dup_pk'
 	
 	# Each instance represents the set of keys from one ore more JSON Schemas
-	def __init__(self,schemaURI, jsonSchemaSource='(unknown)', config={}):
-		super().__init__(schemaURI,jsonSchemaSource,config)
+	def __init__(self,schemaURI, jsonSchemaSource='(unknown)', config={}, isRW=True):
+		super().__init__(schemaURI, jsonSchemaSource, config, isRW=isRW)
 		self.doPopulate = False
 		self.gotIdsSet = None
 		self.warmedUp = False
 	
 	@property
 	def triggerAttribute(self):
 		return self.KeyAttributeName
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator/extensions/unique_check.py` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator/extensions/unique_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,33 +7,27 @@
 
 from jsonschema.exceptions import FormatError, ValidationError
 
 import sys
 import re
 import json
 
-if sys.version_info[0] > 2:
-	ALLOWED_KEY_TYPES=(bytes,str)
-	ALLOWED_ATOMIC_VALUE_TYPES=(int,bytes,str,float,bool,type(None))
-	# py3k
-	pass
-else:
-	ALLOWED_KEY_TYPES=(str,unicode)
-	ALLOWED_ATOMIC_VALUE_TYPES=(int,long,str,unicode,float,bool,type(None))
+ALLOWED_KEY_TYPES=(bytes,str)
+ALLOWED_ATOMIC_VALUE_TYPES=(int,bytes,str,float,bool,type(None))
 
 UniqueLoc = namedtuple('UniqueLoc',['schemaURI','path'])
 UniqueDef = namedtuple('UniqueDef',['uniqueLoc','members','values'])
 
 class UniqueKey(AbstractCustomFeatureValidator):
 	KeyAttributeName = 'unique'
 	SchemaErrorReason = 'dup_unique'
 	
 	# Each instance represents the set of keys from one ore more JSON Schemas
-	def __init__(self,schemaURI,jsonSchemaSource='(unknown)',config={}):
-		super().__init__(schemaURI,jsonSchemaSource,config)
+	def __init__(self, schemaURI, jsonSchemaSource='(unknown)', config={}, isRW=True):
+		super().__init__(schemaURI, jsonSchemaSource, config, isRW=isRW)
 		self.UniqueWorld = dict()
 	
 	@property
 	def triggerAttribute(self):
 		return self.KeyAttributeName
 	
 	@property
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/PKG-INFO` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extended-json-schema-validator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Extended JSON Schema Validator
 Home-page: https://github.com/inab/python-extended-json-schema-validator
 Author: José Mª Fernández
 Author-email: jose.m.fernandez@bsc.es
 License: LGPLv2
 Project-URL: Bug Tracker, https://github.com/inab/python-extended-json-schema-validator/issues
 Platform: UNKNOWN
@@ -34,19 +34,19 @@
 ## Usage
 
 ```bash
 python jsonValidate.py --help
 ```
 ```
 usage: jsonValidate.py [-h] [--log-file LOGFILENAME] [--log-format LOGFORMAT] [-q] [-v] [-d] [-C CONFIGFILENAME]
-                       [--cache-dir CACHEDIR] [--report REPORTFILENAME] [--verbose-report] [--invalidate]
+                       [--cache-dir CACHEDIR] [--report REPORTFILENAME] [--verbose-report] [--invalidate | --read-only]
                        [--warm-up | --lazy-load] [-V]
                        json_schema_or_dir [json_file_or_dir [json_file_or_dir ...]]
 
-Validate JSON against JSON Schemas with extensions (version 0.9.7)
+Validate JSON against JSON Schemas with extensions (version 0.9.9)
 
 positional arguments:
   json_schema_or_dir    The JSON Schema file or directory to validate and use
   json_file_or_dir      The JSON files or directories to be validated
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -60,14 +60,15 @@
   -C CONFIGFILENAME, --config CONFIGFILENAME
                         Configuration file (used by extensions)
   --cache-dir CACHEDIR  Caching directory (used by extensions)
   --report REPORTFILENAME
                         Store validation report (in JSON format) in a file
   --verbose-report      When this flag is enabled, the report also embeds the json contents which were validated
   --invalidate          Caches are invalidated on startup
+  --read-only           When this flag is enabled, the caches are read-only, avoiding expensive operations related to the caches
   --warm-up             Caches are warmed up on startup
   --lazy-load           Caches are warmed up in a lazy way
   -V, --version         show program's version number and exit
 ```
 
 Next lines run validations using test data:
```

### Comparing `extended_json_schema_validator-0.9.8/extended_json_schema_validator.egg-info/SOURCES.txt` & `extended_json_schema_validator-0.9.9/extended_json_schema_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extended_json_schema_validator-0.9.8/jsonValidate.py` & `extended_json_schema_validator-0.9.9/jsonValidate.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,17 @@
 	ap.add_argument('-d', '--debug', dest='logLevel', action='store_const', const=logging.DEBUG, help='Show debug messages (use with care, as it could potentially disclose sensitive contents)')
 	ap.add_argument('-C','--config',dest="configFilename",help="Configuration file (used by extensions)")
 	ap.add_argument('--cache-dir',dest="cacheDir",help="Caching directory (used by extensions)")
 	
 	ap.add_argument('--report',dest="reportFilename",help="Store validation report (in JSON format) in a file")
 	ap.add_argument('--verbose-report',dest="isQuietReport",help="When this flag is enabled, the report also embeds the json contents which were validated", action='store_false', default=True)
 	
-	ap.add_argument('--invalidate',help="Caches are invalidated on startup", action='store_true')
+	grp0 = ap.add_mutually_exclusive_group()
+	grp0.add_argument('--invalidate', help="Caches are invalidated on startup", action='store_true')
+	grp0.add_argument('--read-only', dest="isRWCache",help="When this flag is enabled, the caches are read-only, avoiding expensive operations related to the caches", action='store_false', default=True)
 	grp = ap.add_mutually_exclusive_group()
 	grp.add_argument('--warm-up',dest="warmUp",help="Caches are warmed up on startup", action='store_const', const=True)
 	grp.add_argument('--lazy-load',dest="warmUp",help="Caches are warmed up in a lazy way", action='store_false')
 	ap.add_argument('jsonSchemaDir', metavar='json_schema_or_dir', help='The JSON Schema file or directory to validate and use')
 	ap.add_argument('json_files', metavar='json_file_or_dir', nargs='*', help='The JSON files or directories to be validated')
 	ap.add_argument('-V', '--version', action='version', version='%(prog)s version ' + ejsv_version)
 	args = ap.parse_args()
@@ -100,15 +102,15 @@
 		local_config['cacheDir'] = args.cacheDir
 	
 	# In any case, assuring the cache directory does exist
 	cacheDir = local_config.get('cacheDir')
 	if cacheDir:
 		os.makedirs(cacheDir, exist_ok=True)
 	
-	ev = ExtensibleValidator(config=local_config)
+	ev = ExtensibleValidator(config=local_config, isRW=args.isRWCache)
 	
 	isVerbose = logLevel <= logging.INFO
 	numSchemas = ev.loadJSONSchemas(args.jsonSchemaDir, verbose=isVerbose)
 	
 	if numSchemas > 0:
 		# Should we invalidate caches?
 		if args.invalidate:
@@ -121,15 +123,15 @@
 			ev.warmUpCaches()
 			t1 = time.time()
 			logging.info("\t{} seconds".format(t1-t0))
 			
 			
 	if len(sys.argv) > 2:
 		if numSchemas == 0:
-			logging.critical("FATAL ERROR: No schema was successfuly loaded. Exiting...\n")
+			logging.critical("FATAL ERROR: No schema was successfully loaded. Exiting...\n")
 			sys.exit(1)
 		
 		jsonFiles = tuple(args.json_files)
 		report = ev.jsonValidate(*jsonFiles,verbose=isVerbose)
 		
 		if args.reportFilename is not None:
 			logging.info("* Storing JSON report at {}".format(args.reportFilename))
```

### Comparing `extended_json_schema_validator-0.9.8/setup.py` & `extended_json_schema_validator-0.9.9/setup.py`

 * *Files identical despite different names*


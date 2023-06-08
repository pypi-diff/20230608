# Comparing `tmp/sop-0.4.0.tar.gz` & `tmp/sop-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sop-0.4.0.tar", last modified: Wed Aug 24 01:43:20 2022, max compression
+gzip compressed data, was "sop-0.5.0.tar", last modified: Thu Jun  8 20:28:59 2023, max compression
```

## Comparing `sop-0.4.0.tar` & `sop-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dkg       (1000) dkg       (1000)        0 2022-08-24 01:43:20.333789 sop-0.4.0/
--rw-r--r--   0 dkg       (1000) dkg       (1000)     1087 2022-02-02 00:56:03.000000 sop-0.4.0/LICENSE
--rw-r--r--   0 dkg       (1000) dkg       (1000)     2973 2022-08-24 01:43:20.329789 sop-0.4.0/PKG-INFO
--rw-r--r--   0 dkg       (1000) dkg       (1000)     2329 2022-04-29 17:09:27.000000 sop-0.4.0/README.md
--rw-r--r--   0 dkg       (1000) dkg       (1000)       38 2022-08-24 01:43:20.333789 sop-0.4.0/setup.cfg
--rw-r--r--   0 dkg       (1000) dkg       (1000)      942 2022-02-02 03:36:09.000000 sop-0.4.0/setup.py
-drwxr-xr-x   0 dkg       (1000) dkg       (1000)        0 2022-08-24 01:43:20.329789 sop-0.4.0/sop/
--rwxr-xr-x   0 dkg       (1000) dkg       (1000)    42817 2022-08-24 01:07:59.000000 sop-0.4.0/sop/__init__.py
--rw-r--r--   0 dkg       (1000) dkg       (1000)      266 2019-10-29 03:00:41.000000 sop-0.4.0/sop/__main__.py
--rw-r--r--   0 dkg       (1000) dkg       (1000)       26 2022-08-24 01:41:30.000000 sop-0.4.0/sop/__version__.py
--rw-r--r--   0 dkg       (1000) dkg       (1000)        0 2022-02-02 03:35:31.000000 sop-0.4.0/sop/py.typed
-drwxr-xr-x   0 dkg       (1000) dkg       (1000)        0 2022-08-24 01:43:20.329789 sop-0.4.0/sop.egg-info/
--rw-r--r--   0 dkg       (1000) dkg       (1000)     2973 2022-08-24 01:43:20.000000 sop-0.4.0/sop.egg-info/PKG-INFO
--rw-r--r--   0 dkg       (1000) dkg       (1000)      198 2022-08-24 01:43:20.000000 sop-0.4.0/sop.egg-info/SOURCES.txt
--rw-r--r--   0 dkg       (1000) dkg       (1000)        1 2022-08-24 01:43:20.000000 sop-0.4.0/sop.egg-info/dependency_links.txt
--rw-r--r--   0 dkg       (1000) dkg       (1000)        4 2022-08-24 01:43:20.000000 sop-0.4.0/sop.egg-info/top_level.txt
+drwxr-xr-x   0 dkg       (1000) dkg       (1000)        0 2023-06-08 20:28:59.311673 sop-0.5.0/
+-rw-r--r--   0 dkg       (1000) dkg       (1000)     1087 2022-02-02 00:56:03.000000 sop-0.5.0/LICENSE
+-rw-r--r--   0 dkg       (1000) dkg       (1000)     2936 2023-06-08 20:28:59.311673 sop-0.5.0/PKG-INFO
+-rw-r--r--   0 dkg       (1000) dkg       (1000)     2329 2022-04-29 17:09:27.000000 sop-0.5.0/README.md
+-rw-r--r--   0 dkg       (1000) dkg       (1000)       38 2023-06-08 20:28:59.311673 sop-0.5.0/setup.cfg
+-rw-r--r--   0 dkg       (1000) dkg       (1000)      942 2022-02-02 03:36:09.000000 sop-0.5.0/setup.py
+drwxr-xr-x   0 dkg       (1000) dkg       (1000)        0 2023-06-08 20:28:59.307673 sop-0.5.0/sop/
+-rwxr-xr-x   0 dkg       (1000) dkg       (1000)    47883 2023-06-01 21:44:57.000000 sop-0.5.0/sop/__init__.py
+-rw-r--r--   0 dkg       (1000) dkg       (1000)      266 2019-10-29 03:00:41.000000 sop-0.5.0/sop/__main__.py
+-rw-r--r--   0 dkg       (1000) dkg       (1000)       26 2023-06-08 20:27:07.000000 sop-0.5.0/sop/__version__.py
+-rw-r--r--   0 dkg       (1000) dkg       (1000)        0 2022-02-02 03:35:31.000000 sop-0.5.0/sop/py.typed
+drwxr-xr-x   0 dkg       (1000) dkg       (1000)        0 2023-06-08 20:28:59.311673 sop-0.5.0/sop.egg-info/
+-rw-r--r--   0 dkg       (1000) dkg       (1000)     2936 2023-06-08 20:28:58.000000 sop-0.5.0/sop.egg-info/PKG-INFO
+-rw-r--r--   0 dkg       (1000) dkg       (1000)      198 2023-06-08 20:28:59.000000 sop-0.5.0/sop.egg-info/SOURCES.txt
+-rw-r--r--   0 dkg       (1000) dkg       (1000)        1 2023-06-08 20:28:58.000000 sop-0.5.0/sop.egg-info/dependency_links.txt
+-rw-r--r--   0 dkg       (1000) dkg       (1000)        4 2023-06-08 20:28:58.000000 sop-0.5.0/sop.egg-info/top_level.txt
```

### Comparing `sop-0.4.0/LICENSE` & `sop-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sop-0.4.0/PKG-INFO` & `sop-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sop
-Version: 0.4.0
+Version: 0.5.0
 Summary: A framework for implementing the Stateless OpenPGP CLI
 Home-page: https://gitlab.com/dkg/python-sop
 Author: Daniel Kahn Gillmor
 Author-email: dkg@fifthhorseman.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
@@ -95,9 +93,7 @@
 
 The major version number will only change when backward-incompatible
 changes are made.
 
 As long as the major version number is 0, the same holds true for the
 minor version number.
 
-
-
```

### Comparing `sop-0.4.0/README.md` & `sop-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sop-0.4.0/setup.py` & `sop-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sop-0.4.0/sop/__init__.py` & `sop-0.5.0/sop/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -182,14 +182,17 @@
     mnemonic = 'AMBIGUOUS_INPUT'
 class SOPKeyCannotSign(SOPException):
     exit_code = 79
     mnemonic = 'KEY_CANNOT_SIGN'
 class SOPIncompatibleOptions(SOPException):
     exit_code = 83
     mnemonic = 'INCOMPATIBLE_OPTIONS'
+class SOPUnsupportedProfile(SOPException):
+    exit_code = 89
+    mnemonic = 'UNSUPPORTED_PROFILE'
 
 
 class SOPSessionKey(object):
     '''Stateless OpenPGP session key
 
     Simple class to represent an OpenPGP session key.
 
@@ -205,36 +208,59 @@
         self.algo:int = algo
         self.key:bytes = key
 
     def __str__(self) -> str:
         key:str = hexlify(self.key).decode('ascii')
         return f'{self.algo}:{key}'
 
+
+class SOPProfile(object):
+    '''A Profile for SOP
+
+    Simple baseclass to represent a profile, for example for key
+    generation or encryption.
+
+    Initialize it with a name (a UTF-8 string with no whitespace) and
+    a description (a UTF-8 string with no newlines).
+    '''
+    def __init__(self, name:str, description:str):
+        if len(list(filter(str.isspace, name))):
+            raise ValueError(f'Bad profile name "{name}": must not contain whitespace')
+        if description.count('\n'):
+            raise ValueError(f'Bad profile description "{description}": must not contain any newline')
+        self.name = name
+        self.description = description
+    def __str__(self) -> str:
+        return f'{self.name}: {self.description}'
     
 class SOPSigResult(object):
     '''Stateless OpenPGP Signature Result
 
     This class describes a valid OpenPGP signature.
     '''
-    def __init__(self, when:datetime, signing_fpr:str, primary_fpr:str, moreinfo:str = ''):
+    def __init__(self, when:datetime, signing_fpr:str, primary_fpr:str, sig_type:Optional[SOPSigType] = None, moreinfo:str = ''):
         self._when:datetime = when
         self._signing_fpr:str = signing_fpr
         self._primary_fpr:str = primary_fpr
+        self._sig_type:Optional[SOPSigType] = sig_type
         self._moreinfo:str = moreinfo
 
     def __str__(self) -> str:
         # ensure tz=UTC:
         whendt:datetime = datetime.fromtimestamp(self._when.timestamp(), tz=timezone.utc)
         when:str = whendt.strftime('%Y-%m-%dT%H:%M:%SZ')
         # strip all whitespace from fprs:
         signing_fpr:str = self._signing_fpr.translate(str.maketrans('', '', string.whitespace))
         primary_fpr:str = self._primary_fpr.translate(str.maketrans('', '', string.whitespace))
+        sig_type:str = ''
+        if self._sig_type is not None:
+            sig_type = f'mode:{self._sig_type.name} '
         # strip all newlines from moreinfo
         moreinfo:str = self._moreinfo.translate(str.maketrans('\n\r', '  '))
-        return f'{when} {signing_fpr} {primary_fpr} {moreinfo}'
+        return f'{when} {signing_fpr} {primary_fpr} {sig_type}{moreinfo}'
     
 class StatelessOpenPGP(object):
     '''Stateless OpenPGP baseclass
 
     Subclass this object, overriding the methods with code that
     implements their declared behavior.  The methods to override are:
     generate_key, extract_cert, sign, verify, encrypt, decrypt, armor,
@@ -242,15 +268,16 @@
 
     Then, instantiate your subclass and call dispatch() on it.
 
     '''
     def __init__(self, version:str, name:Optional[str]=None,
                  description:Optional[str]='A Stateless OpenPGP implementation',
                  backend:Optional[str]=None,
-                 extended:Optional[str]=None):
+                 extended:Optional[str]=None,
+                 sop_spec:Optional[str]=None):
         '''Set up Stateless OpenPGP command line interface parser
 
         `version` should be a version string like "0.17.3"
 
         `name` should be a human-readable name for the project with no
         whitespace in it.
 
@@ -261,44 +288,53 @@
         backend, for example "CryptoLib 1.14".
 
         `extended` is any amount of version-related text that
         describes the tool.  This module will add its own information
         to the output of `sop version --extended` in addition to any
         text supplied here.
 
+        `sop_spec` is the string of the version of sop.  Only provide
+        this if the version is fully implemented.
+
         '''
         self._version = version
         self._backend = backend
         self._extended = extended
+        self._sop_spec = sop_spec
 
         self._parser = ArgumentParser(prog=name, description=description)
         self._parser.add_argument('--debug', action='store_true',
                                   help='show debugging data')
         _cmds:_SubParsersAction[ArgumentParser] = self._parser.add_subparsers(required=True,
                                             metavar='SUBCOMMAND',
                                             dest='subcmd')
         _subs = {}
         _version = _cmds.add_parser('version', help='emit version')
         version_type = _version.add_mutually_exclusive_group(required=False)
         version_type.add_argument('--backend', action='store_true')
         version_type.add_argument('--extended', action='store_true')
+        version_type.add_argument('--sop-spec', action='store_true')
         _subs['version'] = _version
 
         def _add_armor_flag(parser:ArgumentParser) -> None:
             parser.add_argument('--no-armor', dest='armor', action='store_false',
                                 help='generate binary output')
             parser.set_defaults(armor=True)
         
         _generate_key = _cmds.add_parser('generate-key',
                                          help='generate a secret key to stdout')
         _add_armor_flag(_generate_key)
         _generate_key.add_argument('--with-key-password',
                                     dest='keypassword',
                                     metavar='PASSWORD',
                                     help='filename containing a password to encrypt the secret key')
+        _generate_key.add_argument('--profile',
+                                   metavar='PROFILE',
+                                   choices=[x.name for x in self.generate_key_profiles],
+                                   help=f'Available key generation profiles: [{" ".join(x.name for x in self.generate_key_profiles)}]')
         _generate_key.add_argument('uids', metavar='USERID', nargs='*',
                                    help='a User ID (a UTF-8 string)')
         _subs['generate-key'] = _generate_key
 
         _extract_cert_h = 'convert a secret key from stdin to a certificate on stdout'
         _extract_cert = _cmds.add_parser('extract-cert',
                                           help=_extract_cert_h)
@@ -345,14 +381,18 @@
                               action='append',
                               help='filename containing a password for symmetric encryption')
         _encrypt.add_argument('--sign-with', dest='signers', metavar='KEYS', action='append',
                               help='filename containing one or more secret keys to sign with')
         _encrypt.add_argument('--with-key-password', dest='keypasswords', metavar='PASSWORD',
                               action='append',
                               help='filename containing a password for unlocking the signing KEYS')
+        _encrypt.add_argument('--profile',
+                              metavar='PROFILE',
+                              choices=[x.name for x in self.encrypt_profiles],
+                              help=f'Available encryption profiles: [{" ".join(x.name for x in self.encrypt_profiles)}]')
         _encrypt.add_argument('recipients', metavar='CERTS', nargs='*',
                               help='filename containing certificate')
         _subs['encrypt'] = _encrypt
 
 
         _decrypt = _cmds.add_parser('decrypt', help='decrypt message')
         _decrypt.add_argument('--session-key-out', dest='sessionkeyout', metavar='SESSIONKEY',
@@ -428,14 +468,21 @@
                                     help='filename to output verification status')
         _inline_verify.add_argument('signers', metavar='CERTS', nargs='+',
                                     help='filename containing certificate of acceptable signer')
         _subs['inline-verify'] = _inline_verify
 
         
         self.extend_parsers(_cmds, _subs)
+
+        _list_profiles = _cmds.add_parser('list-profiles', help='Describe available profiles for subcommand')
+        _list_profiles.add_argument('subcommand', metavar='SUBCOMMAND',
+                                    choices= list(_subs.keys()) + ['list-profiles'],
+                                    help='The subcommand to list profiles for')
+        _subs['list-profiles'] = _list_profiles
+
         if argcomplete:
             argcomplete.autocomplete(self._parser)
         elif '_ARGCOMPLETE' in os.environ:
             logging.error('Argument completion requested but the "argcomplete" module is not installed.'
                           'It can be obtained at https://pypi.python.org/pypi/argcomplete')
             sys.exit(1)
 
@@ -509,14 +556,17 @@
         subcommand).
 
         '''
         pass
 
     def raise_on_unknown_options(self, **kwargs:Namespace) -> None:
         '''if any options are left in the `args` namespace, raise an exception'''
+        # an empty or default value for --profile can be ignored:
+        if 'profile' in kwargs and kwargs['profile'] is None or kwargs['profile'] == 'default':
+            del kwargs['profile']
         if kwargs:
             missingargs:str = ','.join([f'--{arg}' for arg in kwargs.keys()])
             s:str = ''
             if len(kwargs) > 1:
                 s = 's'
             raise SOPUnsupportedOption(f'Unsupported argument{s} {missingargs}')
 
@@ -552,40 +602,84 @@
         except SOPException as e:
             logging.error(f'[{e.mnemonic}] {e}')
             exit(e.exit_code)
 
 
     def _handle_version(self, inp:io.BufferedReader,
                         backend:bool = False,
-                        extended:bool = False) -> bytes:
+                        extended:bool = False,
+                        sop_spec:bool = False) -> bytes:
+        if sop_spec:
+            if self._sop_spec is not None:
+                return f'{self._sop_spec}\n'.encode('utf-8')
+            else:
+                return '~draft-dkg-openpgp-stateless-cli-06\n'.encode('utf-8')
         if backend:
             if self._backend:
                 return f'{self._backend}\n'.encode('utf-8')
             else:
                 raise SOPUnsupportedOption('--backend')
         verstring = f'{self._parser.prog} {self._version}\n'
         if extended:
             verstring += f'python-sop {__version__}\n'
             if self._extended:
                 verstring += f'{self._extended}\n'
             if self._backend:
                 verstring += f'{self._backend}\n'
         return verstring.encode('utf-8')
 
+
+    @property
+    def generate_key_profiles(self) -> List[SOPProfile]:
+        '''Override this to offer multiple key generation profiles'''
+        return [SOPProfile('default', 'The default key generation profile')]
+
+    @property
+    def encrypt_profiles(self) -> List[SOPProfile]:
+        '''Override this to offer multiple encryption profiles'''
+        return [SOPProfile('default', 'The default encryption profile')]
+
+
+    def _handle_list_profiles(self,
+                              inp:io.BufferedReader,
+                              subcommand:str,
+                              **kwargs:Namespace) -> bytes:
+        if subcommand == 'generate-key':
+            return ('\n'.join(map(lambda x: str(x), self.generate_key_profiles)) + '\n').encode()
+        if subcommand == 'encrypt':
+            return ('\n'.join(map(lambda x: str(x), self.encrypt_profiles)) + '\n').encode()
+        else:
+            raise SOPUnsupportedProfile(f'no profiles for subcommand "{subcommand}"')
+
+
     def _handle_generate_key(self,
                              inp:io.BufferedReader,
                              armor:bool=True,
                              keypassword:Optional[str]=None,
                              uids:List[str]=[],
+                             profile:Optional[str]=None,
                              **kwargs:Namespace) -> bytes:
+        prof:Optional[SOPProfile] = None
+        if profile is not None:
+            if profile == 'default':
+                prof = self.generate_key_profiles[0]
+            else:
+                for p in self.generate_key_profiles:
+                    if p.name == profile:
+                        prof = p
+                        break
+            if prof is None:
+                raise SOPUnsupportedProfile(f'profile "{profile}" not supported for generate_key subcommand')
         return self.generate_key(armor=armor, uids=uids,
                                  keypassword=self._get_indirect_input(keypassword) if keypassword else None,
+                                 profile=prof,
                                  **kwargs)
     def generate_key(self, armor:bool=True, uids:List[str]=[],
-                     keypassword:Optional[str]=None,
+                     keypassword:Optional[bytes]=None,
+                     profile:Optional[SOPProfile]=None,
                      **kwargs:Namespace) -> bytes:
         '''Produce an OpenPGP transferable secret key
 
 `armor`: whether to produce an ASCII-armored form or a binary-encoded form.
 
 `key_password`: if present, ensure that all secret key material is locked with this password.
         '''
@@ -713,34 +807,48 @@
                         inp:io.BufferedReader,
                         literaltype:str,
                         armor:bool,
                         passwords:List[str],
                         signers:List[str],
                         keypasswords:List[str],
                         recipients:List[str],
+                        profile:Optional[str] = None,
                         **kwargs:Namespace) -> bytes:
+        prof:Optional[SOPProfile] = None
+        if profile is not None:
+            if profile == 'default':
+                prof = self.encrypt_profiles[0]
+            else:
+                for p in self.encrypt_profiles:
+                    if p.name == profile:
+                        prof = p
+                        break
+            if prof is None:
+                raise SOPUnsupportedProfile(f'profile "{profile}" not supported for encrypt subcommand')
         return self.encrypt(inp.read(),
                             literaltype=SOPLiteralDataType.__members__[literaltype],
                             armor=armor,
                             passwords=dict((password, self._get_indirect_input(password))
                                            for password in passwords) if passwords else dict(),
                             signers=dict((signer, self._get_indirect_input(signer))
                                          for signer in signers) if signers else dict(),
                             keypasswords=dict((password, self._get_indirect_input(password))
                                            for password in keypasswords) if keypasswords else dict(),
                             recipients=dict((recipient, self._get_indirect_input(recipient))
                                             for recipient in recipients) if recipients else dict(),
+                            profile=prof,
                             **kwargs)
     def encrypt(self, data:bytes,
                 literaltype:SOPLiteralDataType=SOPLiteralDataType.binary,
                 armor:bool=True,
                 passwords:MutableMapping[str,bytes]={},
                 signers:MutableMapping[str,bytes]={},
                 keypasswords:MutableMapping[str,bytes]={},
                 recipients:MutableMapping[str,bytes]={},
+                profile:Optional[SOPProfile]=None,
                 **kwargs:Namespace) -> bytes:
         '''Encrypt a message
 
         Encrypt a message so that only the intended recipients (or
         someone with access to a provided password) can read it.
 
         `data`: the message to be encrypted
```

### Comparing `sop-0.4.0/sop.egg-info/PKG-INFO` & `sop-0.5.0/sop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sop
-Version: 0.4.0
+Version: 0.5.0
 Summary: A framework for implementing the Stateless OpenPGP CLI
 Home-page: https://gitlab.com/dkg/python-sop
 Author: Daniel Kahn Gillmor
 Author-email: dkg@fifthhorseman.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
@@ -95,9 +93,7 @@
 
 The major version number will only change when backward-incompatible
 changes are made.
 
 As long as the major version number is 0, the same holds true for the
 minor version number.
 
-
-
```


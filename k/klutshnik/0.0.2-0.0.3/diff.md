# Comparing `tmp/klutshnik-0.0.2.tar.gz` & `tmp/klutshnik-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klutshnik-0.0.2.tar", last modified: Fri Mar 31 21:37:27 2023, max compression
+gzip compressed data, was "klutshnik-0.0.3.tar", last modified: Sat Apr  8 19:54:24 2023, max compression
```

## Comparing `klutshnik-0.0.2.tar` & `klutshnik-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-03-31 21:37:27.525593 klutshnik-0.0.2/
--rw-r--r--   0 s         (1000) s         (1000)       32 2023-03-31 21:36:27.000000 klutshnik-0.0.2/MANIFEST.in
--rw-r--r--   0 s         (1000) s         (1000)      509 2023-03-31 21:37:27.525593 klutshnik-0.0.2/PKG-INFO
--rw-r--r--   0 s         (1000) s         (1000)       51 2023-03-30 23:57:11.000000 klutshnik-0.0.2/README.org
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-03-31 21:37:27.525593 klutshnik-0.0.2/klutshnik/
--rwxr-xr-x   0 s         (1000) s         (1000)     5868 2023-03-31 00:11:11.000000 klutshnik-0.0.2/klutshnik/client.py
--rwxr-xr-x   0 s         (1000) s         (1000)      382 2023-03-31 00:11:23.000000 klutshnik-0.0.2/klutshnik/genkey.py
--rwxr-xr-x   0 s         (1000) s         (1000)     2698 2023-03-30 23:42:57.000000 klutshnik-0.0.2/klutshnik/noiseclient.py
--rwxr-xr-x   0 s         (1000) s         (1000)      808 2023-03-30 22:41:46.000000 klutshnik-0.0.2/klutshnik/utils.py
--rwxr-xr-x   0 s         (1000) s         (1000)     5597 2023-03-31 00:00:11.000000 klutshnik-0.0.2/klutshnik/wrapper.py
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-03-31 21:37:27.525593 klutshnik-0.0.2/klutshnik.egg-info/
--rw-r--r--   0 s         (1000) s         (1000)      509 2023-03-31 21:37:27.000000 klutshnik-0.0.2/klutshnik.egg-info/PKG-INFO
--rw-r--r--   0 s         (1000) s         (1000)      336 2023-03-31 21:37:27.000000 klutshnik-0.0.2/klutshnik.egg-info/SOURCES.txt
--rw-r--r--   0 s         (1000) s         (1000)        1 2023-03-31 21:37:27.000000 klutshnik-0.0.2/klutshnik.egg-info/dependency_links.txt
--rw-r--r--   0 s         (1000) s         (1000)       88 2023-03-31 21:37:27.000000 klutshnik-0.0.2/klutshnik.egg-info/entry_points.txt
--rw-r--r--   0 s         (1000) s         (1000)       32 2023-03-31 21:37:27.000000 klutshnik-0.0.2/klutshnik.egg-info/requires.txt
--rw-r--r--   0 s         (1000) s         (1000)       10 2023-03-31 21:37:27.000000 klutshnik-0.0.2/klutshnik.egg-info/top_level.txt
--rw-r--r--   0 s         (1000) s         (1000)       38 2023-03-31 21:37:27.525593 klutshnik-0.0.2/setup.cfg
--rwxr-xr-x   0 s         (1000) s         (1000)     1381 2023-03-31 21:36:55.000000 klutshnik-0.0.2/setup.py
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-08 19:54:24.880515 klutshnik-0.0.3/
+-rw-r--r--   0 s         (1000) s         (1000)       32 2023-03-31 21:36:27.000000 klutshnik-0.0.3/MANIFEST.in
+-rw-r--r--   0 s         (1000) s         (1000)      509 2023-04-08 19:54:24.880515 klutshnik-0.0.3/PKG-INFO
+-rw-r--r--   0 s         (1000) s         (1000)       51 2023-03-30 23:57:11.000000 klutshnik-0.0.3/README.org
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-08 19:54:24.879515 klutshnik-0.0.3/klutshnik/
+-rw-r--r--   0 s         (1000) s         (1000)        1 2023-04-08 19:29:00.000000 klutshnik-0.0.3/klutshnik/__init__.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     5889 2023-04-08 19:51:39.000000 klutshnik-0.0.3/klutshnik/client.py
+-rwxr-xr-x   0 s         (1000) s         (1000)      382 2023-03-31 00:11:23.000000 klutshnik-0.0.3/klutshnik/genkey.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     2698 2023-03-30 23:42:57.000000 klutshnik-0.0.3/klutshnik/noiseclient.py
+-rwxr-xr-x   0 s         (1000) s         (1000)      808 2023-03-30 22:41:46.000000 klutshnik-0.0.3/klutshnik/utils.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     5597 2023-03-31 00:00:11.000000 klutshnik-0.0.3/klutshnik/wrapper.py
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2023-04-08 19:54:24.880515 klutshnik-0.0.3/klutshnik.egg-info/
+-rw-r--r--   0 s         (1000) s         (1000)      509 2023-04-08 19:54:24.000000 klutshnik-0.0.3/klutshnik.egg-info/PKG-INFO
+-rw-r--r--   0 s         (1000) s         (1000)      358 2023-04-08 19:54:24.000000 klutshnik-0.0.3/klutshnik.egg-info/SOURCES.txt
+-rw-r--r--   0 s         (1000) s         (1000)        1 2023-04-08 19:54:24.000000 klutshnik-0.0.3/klutshnik.egg-info/dependency_links.txt
+-rw-r--r--   0 s         (1000) s         (1000)       88 2023-04-08 19:54:24.000000 klutshnik-0.0.3/klutshnik.egg-info/entry_points.txt
+-rw-r--r--   0 s         (1000) s         (1000)       32 2023-04-08 19:54:24.000000 klutshnik-0.0.3/klutshnik.egg-info/requires.txt
+-rw-r--r--   0 s         (1000) s         (1000)       10 2023-04-08 19:54:24.000000 klutshnik-0.0.3/klutshnik.egg-info/top_level.txt
+-rw-r--r--   0 s         (1000) s         (1000)       38 2023-04-08 19:54:24.880515 klutshnik-0.0.3/setup.cfg
+-rwxr-xr-x   0 s         (1000) s         (1000)     1381 2023-04-08 19:54:08.000000 klutshnik-0.0.3/setup.py
```

### Comparing `klutshnik-0.0.2/klutshnik/client.py` & `klutshnik-0.0.3/klutshnik/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,38 @@
 
 import os, io, sys
 import pysodium, argparse, subprocess
 from binascii import unhexlify, a2b_base64, b2a_base64
 from dissononce.dh.x25519.keypair import KeyPair
 from dissononce.dh.x25519.public import PublicKey
 from klutshnik.noiseclient import NoiseWrapper
-from opaquestore import opaquestore
+from opaquestore import client as opaquestore
 
 from klutshnik.utils import getcfg
-from klutshnik.wrapper import dkg, update, decrypt, stream_encrypt, update_w, DKG, Evaluate, TUOKMS_Update
-
-KEYID_SIZE = 16
+from klutshnik.wrapper import dkg, update, decrypt, stream_encrypt, update_w, DKG, Evaluate, TUOKMS_Update, KEYID_SIZE
 
 config = None
 
 def getpwd(title):
     proc=subprocess.Popen(['/usr/bin/pinentry', '-g'], stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     out, err = proc.communicate(input=('SETTITLE klutshnik password prompt\nSETDESC %s\nSETPROMPT opaque-store password\ngetpin\n' % (title)).encode())
     if proc.returncode == 0:
         for line in out.split(b'\n'):
             if line.startswith(b"D "): return line[2:]
 
-def getauthkey(op, keyid):
+def getauthtok(op, keyid):
    cfg = config['opaque-storage']
    if op == DKG:
       keyid = b'unbound'
    keyid=pysodium.crypto_generichash(cfg['username'].encode('utf8') + keyid)
    pwd = getpwd("getting auth token from opaque-store password")
    s = NoiseWrapper.connect(cfg['address'], cfg['port'], cfg['noise_key'], cfg['server_pubkey'])
    return opaquestore.get(s, pwd, keyid)
 
-def setauthkey(keyid, token):
+def setauthtok(keyid, token):
    cfg = config['opaque-storage']
    keyid=pysodium.crypto_generichash(cfg['username'].encode('utf8') + keyid)
    pwd = getpwd("saving auth token to opaque-store password")
    opaquestore.test_pwd(pwd)
    s = NoiseWrapper.connect(cfg['address'], cfg['port'], cfg['noise_key'], cfg['server_pubkey'])
    opaquestore.create(s, pwd, keyid, token)
 
@@ -57,86 +55,87 @@
      config['key']=KeyPair.from_bytes(a2b_base64(fd.read()))
 
   config['servers'] = [(v.get('host',"localhost"),
                         v.get('port'),
                         PublicKey(a2b_base64(v['pubkey']))) 
                        for k,v in config.get('servers',{}).items()]
 
+  if 'authtok' in config:
+    config['authtok']=a2b_base64(config['authtok']+'==')
+
   if 'opaque-storage' not in config:
-     if 'authkey' not in config:
-        raise ValueError("no opaque-storage and no authkey in config file")
-     config['authkey']=a2b_base64(config['authkey']+'==')
-     return config
+        raise ValueError("no opaque-storage and no authtok in config file")
 
   config['opaque-storage']['noise_key']=KeyPair.from_bytes(a2b_base64(config['opaque-storage']['noise_key']+'=='))
   config['opaque-storage']['server_pubkey']=PublicKey(a2b_base64(config['opaque-storage']['server_pubkey']+'=='))
   opaquestore.config = config['opaque-storage']
 
   return config
 
-def authkey(op, keyid):
-  return config.get('authkey', getauthkey(op, keyid))
+def authtok(op, keyid):
+  return config.get('authtok') or getauthtok(op, keyid)
 
 def main(params=sys.argv):
     global config
     config = processcfg(getcfg("klutshnik"))
 
     parser = argparse.ArgumentParser(description='klutshnik cli'
     f"usage: {sys.argv[0]} -c <genkey|encrypt|decrypt|update>"
     f"       {sys.argv[0]} -c genkey -t threshold ..."
     f"       {sys.argv[0]} -c encrypt -k keyid <filetoencrypt >encryptedfile"
     f"       {sys.argv[0]} -c decrypt <filetodecrypt >decryptedfile"
     f"       {sys.argv[0]} -c update -k keyid <listoffilestoupdate")
 
-    parser.add_argument('-c', '--cmd', choices={"genkey", "encrypt", "decrypt", "update", 'authkey'})
+    parser.add_argument('-c', '--cmd', choices={"genkey", "encrypt", "decrypt", "update", 'authtok'})
     parser.add_argument('-t', '--threshold', type=int)
     parser.add_argument('-k', '--keyid')
     args = parser.parse_args()
 
     if args.cmd=="genkey":
         if args.threshold*2 + 1 < len(config['servers']):
             print("Warning this key will not be updatable.", file=sys.stderr)
             print("You need to have at least 2*threshold+1 servers for updatable keys", file=sys.stderr)
             if input("press y/Y to continue") not in ('y','Y'): return
-        pubkey, keyid, auth_token = dkg(config['servers'], args.threshold, config['key'], authkey)
+        pubkey, keyid, auth_token = dkg(config['servers'], args.threshold, config['key'], authtok)
+
+        setauthtok(keyid,auth_token)
+        if 'opaque-storage' not in config:
+          print("authtoken for new key: ", b2a_base64(auth_token).decode('utf8').strip())
 
-        setauthkey(keyid,auth_token)
-        print("authtoken for new key: ", b2a_base64(auth_token).decode('utf8').strip())
-     
         savekey(keyid.hex(), pubkey, args.threshold)
         print("keyid", keyid.hex())
 
     elif args.cmd=="encrypt":
         pubkey, _ = loadkey(args.keyid)
         os.write(1, unhexlify(args.keyid))
         stream_encrypt(pubkey)
 
     elif args.cmd=="decrypt":
         keyid = os.read(0, KEYID_SIZE)
         w = os.read(0, pysodium.crypto_core_ristretto255_BYTES)
         pubkey, threshold = loadkey(keyid.hex())
-        decrypt(w, pubkey, config['servers'], threshold, keyid, config['key'], authkey)
+        decrypt(w, pubkey, config['servers'], threshold, keyid, config['key'], authtok)
 
     elif args.cmd=="update":
         _, threshold = loadkey(args.keyid)
-        pubkey, delta = update(config['servers'], threshold, unhexlify(args.keyid), config['key'], authkey)
+        pubkey, delta = update(config['servers'], threshold, unhexlify(args.keyid), config['key'], authtok)
         savekey(args.keyid, pubkey, threshold)
         for path in sys.stdin:
             with open(path,'r+b') as fd:
                 fkeyid = fd.read(KEYID_SIZE)
                 if args.keyid!=fkeyid.hex():
                     print(f"{path} is not encrypted using keyid: {args.keyid}, skipping")
                     continue
                 w = fd.read(pysodium.crypto_core_ristretto255_BYTES)
                 w = update_w(delta, w)
                 fd.seek(-pysodium.crypto_core_ristretto255_BYTES,io.SEEK_CUR)
                 fd.write(w)
-    elif args.cmd=="authkey":
+    elif args.cmd=="authtok":
         token = a2b_base64(sys.stdin.buffer.readline().rstrip(b'\n')+b'==')
-        setauthkey(b'unbound', token)
+        setauthtok(b'unbound', token)
 
     else:
         parser.print_help()
         usage()
 
 if __name__ == '__main__':
   try:
```

### Comparing `klutshnik-0.0.2/klutshnik/noiseclient.py` & `klutshnik-0.0.3/klutshnik/noiseclient.py`

 * *Files identical despite different names*

### Comparing `klutshnik-0.0.2/klutshnik/utils.py` & `klutshnik-0.0.3/klutshnik/utils.py`

 * *Files identical despite different names*

### Comparing `klutshnik-0.0.2/klutshnik/wrapper.py` & `klutshnik-0.0.3/klutshnik/wrapper.py`

 * *Files identical despite different names*

### Comparing `klutshnik-0.0.2/setup.py` & `klutshnik-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(name = 'klutshnik',
-      version = '0.0.2',
+      version = '0.0.3',
       description = 'Klutshnik (and OPRF) CLI client',
       license = "GPLv3",
       author = 'Stefan Marsiske',
       author_email = 'klutshnik@ctrlc.hu',
       url = 'https://github.com/stef/klutshnik',
       long_description=read('README.org'),
       long_description_content_type="text/markdown",
```


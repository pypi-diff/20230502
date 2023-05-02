# Comparing `tmp/rtmidi-2.3.4.tar.gz` & `tmp/rtmidi-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rtmidi-2.3.4.tar", last modified: Thu Aug 16 00:24:02 2018, max compression
+gzip compressed data, was "rtmidi-2.5.0.tar", last modified: Tue May  2 08:19:14 2023, max compression
```

## Comparing `rtmidi-2.3.4.tar` & `rtmidi-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2018-08-16 00:24:02.000000 rtmidi-2.3.4/
--rw-r--r--   0 patrick    (501) staff       (20)     1217 2018-08-16 00:24:02.000000 rtmidi-2.3.4/PKG-INFO
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2018-08-16 00:24:02.000000 rtmidi-2.3.4/rtmidi/
--rw-r--r--   0 patrick    (501) staff       (20)     1421 2017-06-16 04:57:05.000000 rtmidi-2.3.4/rtmidi/randomout.py
--rw-r--r--   0 patrick    (501) staff       (20)     4520 2017-06-16 04:57:05.000000 rtmidi-2.3.4/rtmidi/collector.py
--rw-r--r--   0 patrick    (501) staff       (20)       88 2014-11-01 00:06:02.000000 rtmidi-2.3.4/rtmidi/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2018-08-16 00:24:02.000000 rtmidi-2.3.4/cpp_src/
--rw-r--r--   0 patrick    (501) staff       (20)    94483 2017-06-16 04:57:05.000000 rtmidi-2.3.4/cpp_src/RtMidi.cpp
--rw-r--r--   0 patrick    (501) staff       (20)    28782 2017-06-16 04:57:05.000000 rtmidi-2.3.4/cpp_src/RtMidi.h
--rw-r--r--   0 patrick    (501) staff       (20)    32571 2018-01-06 07:25:43.000000 rtmidi-2.3.4/cpp_src/MidiMessage.h
--rw-r--r--   0 patrick    (501) staff       (20)    33795 2018-08-16 00:18:51.000000 rtmidi-2.3.4/cpp_src/MidiMessage.cpp
--rw-r--r--   0 patrick    (501) staff       (20)    24683 2018-01-06 07:26:30.000000 rtmidi-2.3.4/cpp_src/rtmidimodule.cpp
--rw-r--r--   0 patrick    (501) staff       (20)     2041 2018-01-06 07:26:21.000000 rtmidi-2.3.4/cpp_src/pkglobals.h
--rw-r--r--   0 patrick    (501) staff       (20)     1515 2018-01-06 07:26:01.000000 rtmidi-2.3.4/cpp_src/PyMidiMessage.h
--rw-r--r--   0 patrick    (501) staff       (20)    37458 2018-01-06 07:25:55.000000 rtmidi-2.3.4/cpp_src/PyMidiMessage.cpp
--rw-r--r--   0 patrick    (501) staff       (20)      859 2017-06-16 04:57:05.000000 rtmidi-2.3.4/setup_pkechomidi.py
--rw-r--r--   0 patrick    (501) staff       (20)     4625 2018-08-16 00:23:53.000000 rtmidi-2.3.4/setup.py
--rw-r--r--   0 patrick    (501) staff       (20)      354 2017-06-16 04:57:05.000000 rtmidi-2.3.4/pkechomidi.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-02 08:19:14.604127 rtmidi-2.5.0/
+-rw-r--r--   0 patrick    (501) staff       (20)       74 2023-05-02 07:57:39.000000 rtmidi-2.5.0/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)     5044 2023-05-02 08:19:14.603726 rtmidi-2.5.0/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4547 2023-05-02 08:17:43.000000 rtmidi-2.5.0/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)      354 2020-05-15 19:00:14.000000 rtmidi-2.5.0/pkechomidi.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-02 08:19:14.592038 rtmidi-2.5.0/rtmidi/
+-rw-r--r--   0 patrick    (501) staff       (20)       88 2020-05-15 19:00:14.000000 rtmidi-2.5.0/rtmidi/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4520 2020-05-15 19:00:14.000000 rtmidi-2.5.0/rtmidi/collector.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1421 2020-05-15 19:00:14.000000 rtmidi-2.5.0/rtmidi/randomout.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-02 08:19:14.594171 rtmidi-2.5.0/rtmidi.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     5044 2023-05-02 08:19:14.000000 rtmidi-2.5.0/rtmidi.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)      409 2023-05-02 08:19:14.000000 rtmidi-2.5.0/rtmidi.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-02 08:19:14.000000 rtmidi-2.5.0/rtmidi.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        7 2023-05-02 08:19:14.000000 rtmidi-2.5.0/rtmidi.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-05-02 08:19:14.604238 rtmidi-2.5.0/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     4292 2023-05-02 08:17:51.000000 rtmidi-2.5.0/setup.py
+-rw-r--r--   0 patrick    (501) staff       (20)      859 2020-05-15 19:00:14.000000 rtmidi-2.5.0/setup_pkechomidi.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-02 08:19:14.602222 rtmidi-2.5.0/src/
+-rw-r--r--   0 patrick    (501) staff       (20)    33410 2023-05-02 07:40:25.000000 rtmidi-2.5.0/src/MidiMessage.cpp
+-rw-r--r--   0 patrick    (501) staff       (20)    32571 2020-05-15 19:00:14.000000 rtmidi-2.5.0/src/MidiMessage.h
+-rw-r--r--   0 patrick    (501) staff       (20)    39859 2023-05-02 07:40:21.000000 rtmidi-2.5.0/src/PyMidiMessage.cpp
+-rw-r--r--   0 patrick    (501) staff       (20)     1515 2020-05-15 19:00:14.000000 rtmidi-2.5.0/src/PyMidiMessage.h
+-rw-r--r--   0 patrick    (501) staff       (20)    94483 2020-05-15 19:00:14.000000 rtmidi-2.5.0/src/RtMidi.cpp
+-rw-r--r--   0 patrick    (501) staff       (20)    28782 2020-05-15 19:00:14.000000 rtmidi-2.5.0/src/RtMidi.h
+-rw-r--r--   0 patrick    (501) staff       (20)     2041 2020-05-15 19:00:14.000000 rtmidi-2.5.0/src/pkglobals.h
+-rw-r--r--   0 patrick    (501) staff       (20)    24683 2020-05-15 19:00:14.000000 rtmidi-2.5.0/src/rtmidimodule.cpp
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-02 08:19:14.602873 rtmidi-2.5.0/tests/
+-rwxr-xr-x   0 patrick    (501) staff       (20)     9494 2020-05-15 19:00:14.000000 rtmidi-2.5.0/tests/test_rtmidi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rtmidi-2.3.4/rtmidi/randomout.py` & `rtmidi-2.5.0/rtmidi/randomout.py`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/rtmidi/collector.py` & `rtmidi-2.5.0/rtmidi/collector.py`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/cpp_src/RtMidi.cpp` & `rtmidi-2.5.0/src/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/cpp_src/RtMidi.h` & `rtmidi-2.5.0/src/RtMidi.h`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/cpp_src/MidiMessage.h` & `rtmidi-2.5.0/src/MidiMessage.h`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/cpp_src/MidiMessage.cpp` & `rtmidi-2.5.0/src/MidiMessage.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /*
- #   Copyright (C) 2018 by Patrick Stinson                                 
- #   patrickkidd@gmail.com                                                   
- #                                                                         
- #   This program is free software; you can redistribute it and/or modify  
- #   it under the terms of the GNU General Public License as published by  
- #   the Free Software Foundation; either version 2 of the License, or     
- #   (at your option) any later version.                                   
- #                                                                         
- #   This program is distributed in the hope that it will be useful,       
- #   but WITHOUT ANY WARRANTY; without even the implied warranty of        
- #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the         
- #   GNU General Public License for more details.                          
- #                                                                         
- #   You should have received a copy of the GNU General Public License     
- #   along with this program; if not, write to the                         
- #   Free Software Foundation, Inc.,                                       
- #   59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.  
+ #   Copyright (C) 2018 by Patrick Stinson
+ #   patrickkidd@gmail.com
+ #
+ #   This program is free software; you can redistribute it and/or modify
+ #   it under the terms of the GNU General Public License as published by
+ #   the Free Software Foundation; either version 2 of the License, or
+ #   (at your option) any later version.
+ #
+ #   This program is distributed in the hope that it will be useful,
+ #   but WITHOUT ANY WARRANTY; without even the implied warranty of
+ #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ #   GNU General Public License for more details.
+ #
+ #   You should have received a copy of the GNU General Public License
+ #   along with this program; if not, write to the
+ #   Free Software Foundation, Inc.,
+ #   59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 */
 
 #include "MidiMessage.h"
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 #include <algorithm>
@@ -27,261 +27,260 @@
 
 #if defined(WIN32) || defined(__LITTLE_ENDIAN__)
 #define PK_LITTLE_ENDIAN 1
 #else
 #define PK_BIG_ENDIAN 1
 #endif
 
-
-#define pkassert(expression)           { /*if (! (expression)) printf("MidiMessage assertion: %s:%i\n", __FILE__, __LINE__);*/ }
+#define pkassert(expression)                                                                \
+    { /*if (! (expression)) printf("MidiMessage assertion: %s:%i\n", __FILE__, __LINE__);*/ \
+    }
 
 template <class Type>
-inline Type pklimit (const Type lowerLimit,
+inline Type pklimit(const Type lowerLimit,
                     const Type upperLimit,
                     const Type valueToConstrain) throw()
 {
-  pkassert (lowerLimit <= upperLimit); // if these are in the wrong order, results are unpredictable..
-  
-  return (valueToConstrain < lowerLimit) ? lowerLimit
-  : ((valueToConstrain > upperLimit) ? upperLimit
-     : valueToConstrain);
-}
-
+    pkassert(lowerLimit <= upperLimit); // if these are in the wrong order, results are unpredictable..
 
+    return (valueToConstrain < lowerLimit) ? lowerLimit
+                                           : ((valueToConstrain > upperLimit) ? upperLimit
+                                                                              : valueToConstrain);
+}
 
 template <typename FloatType>
-inline int roundToInt (const FloatType value) throw()
+inline int roundToInt(const FloatType value) throw()
 {
-  union { int asInt[2]; double asDouble; } n;
-  n.asDouble = ((double) value) + 6755399441055744.0;
+    union
+    {
+        int asInt[2];
+        double asDouble;
+    } n;
+    n.asDouble = ((double)value) + 6755399441055744.0;
 
 #if JUCE_BIG_ENDIAN
-  return n.asInt [1];
+    return n.asInt[1];
 #else
-  return n.asInt [0];
+    return n.asInt[0];
 #endif
 }
 
-inline int roundFloatToInt (const float value) throw()
+inline int roundFloatToInt(const float value) throw()
 {
-  return roundToInt (value);
+    return roundToInt(value);
 }
 
-
 class BlobKiller
 {
-  void *p;
+    void *p;
+
 public:
-  BlobKiller(void *x) : p(x) {}
-  ~BlobKiller() { free(p); }
+    BlobKiller(void *x) : p(x) {}
+    ~BlobKiller() { free(p); }
 };
 
 //==============================================================================
-int MidiMessage::readVariableLengthVal (const uint8* data,
-                                        int& numBytesUsed) throw()
+int MidiMessage::readVariableLengthVal(const uint8 *data,
+                                       int &numBytesUsed) throw()
 {
     numBytesUsed = 0;
     int v = 0;
     int i;
 
     do
     {
-        i = (int) *data++;
+        i = (int)*data++;
 
         if (++numBytesUsed > 6)
             break;
 
         v = (v << 7) + (i & 0x7f);
 
     } while (i & 0x80);
 
     return v;
 }
 
-int MidiMessage::getMessageLengthFromFirstByte (const uint8 firstByte) throw()
+int MidiMessage::getMessageLengthFromFirstByte(const uint8 firstByte) throw()
 {
     // this method only works for valid starting bytes of a short midi message
-    pkassert (firstByte >= 0x80
-              && firstByte != 0xf0
-              && firstByte != 0xf7);
+    pkassert(firstByte >= 0x80 && firstByte != 0xf0 && firstByte != 0xf7);
 
     static const char messageLengths[] =
-    {
-        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
-        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
-        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
-        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
-        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
-        2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
-        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
-        1, 2, 3, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1
-    };
+        {
+            3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+            3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+            3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+            3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+            2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+            2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2,
+            3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+            1, 2, 3, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1};
 
-    return messageLengths [firstByte & 0x7f];
+    return messageLengths[firstByte & 0x7f];
 }
 
-
 //==============================================================================
-MidiMessage::MidiMessage (const uint8* const d,
-                          const int dataSize,
-                          const double t) throw()
-   : timeStamp (t),
-     message (0),
-     size (dataSize)
+MidiMessage::MidiMessage(const uint8 *const d,
+                         const int dataSize,
+                         const double t) throw()
+    : timeStamp(t),
+      message(0),
+      size(dataSize)
 {
-    pkassert (dataSize > 0);
+    pkassert(dataSize > 0);
 
     if (dataSize <= 4)
-        data = (uint8*) &message;
+        data = (uint8 *)&message;
     else
-        data = (uint8*) malloc (dataSize);
+        data = (uint8 *)malloc(dataSize);
 
-    memcpy (data, d, dataSize);
+    memcpy(data, d, dataSize);
 
     // check that the length matches the data..
-    pkassert (size > 3 || *d >= 0xf0 || getMessageLengthFromFirstByte (*d) == size);
+    pkassert(size > 3 || *d >= 0xf0 || getMessageLengthFromFirstByte(*d) == size);
 }
 
-MidiMessage::MidiMessage (const int byte1,
-                          const double t) throw()
-   : timeStamp (t),
-     data ((uint8*) &message),
-     size (1)
+MidiMessage::MidiMessage(const int byte1,
+                         const double t) throw()
+    : timeStamp(t),
+      data((uint8 *)&message),
+      size(1)
 {
-    data[0] = (uint8) byte1;
+    data[0] = (uint8)byte1;
 
     // check that the length matches the data..
-    pkassert (byte1 >= 0xf0 || getMessageLengthFromFirstByte ((uint8) byte1) == 1);
+    pkassert(byte1 >= 0xf0 || getMessageLengthFromFirstByte((uint8)byte1) == 1);
 }
 
-MidiMessage::MidiMessage (const int byte1,
-                          const int byte2,
-                          const double t) throw()
-   : timeStamp (t),
-     data ((uint8*) &message),
-     size (2)
+MidiMessage::MidiMessage(const int byte1,
+                         const int byte2,
+                         const double t) throw()
+    : timeStamp(t),
+      data((uint8 *)&message),
+      size(2)
 {
-    data[0] = (uint8) byte1;
-    data[1] = (uint8) byte2;
+    data[0] = (uint8)byte1;
+    data[1] = (uint8)byte2;
 
     // check that the length matches the data..
-    pkassert (byte1 >= 0xf0 || getMessageLengthFromFirstByte ((uint8) byte1) == 2);
+    pkassert(byte1 >= 0xf0 || getMessageLengthFromFirstByte((uint8)byte1) == 2);
 }
 
-MidiMessage::MidiMessage (const int byte1,
-                          const int byte2,
-                          const int byte3,
-                          const double t) throw()
-   : timeStamp (t),
-     data ((uint8*) &message),
-     size (3)
-{
-    data[0] = (uint8) byte1;
-    data[1] = (uint8) byte2;
-    data[2] = (uint8) byte3;
+MidiMessage::MidiMessage(const int byte1,
+                         const int byte2,
+                         const int byte3,
+                         const double t) throw()
+    : timeStamp(t),
+      data((uint8 *)&message),
+      size(3)
+{
+    data[0] = (uint8)byte1;
+    data[1] = (uint8)byte2;
+    data[2] = (uint8)byte3;
 
     // check that the length matches the data..
-    pkassert (byte1 >= 0xf0 || getMessageLengthFromFirstByte ((uint8) byte1) == 3);
+    pkassert(byte1 >= 0xf0 || getMessageLengthFromFirstByte((uint8)byte1) == 3);
 }
 
-MidiMessage::MidiMessage (const MidiMessage& other) throw()
-   : timeStamp (other.timeStamp),
-     message (other.message),
-     size (other.size)
+MidiMessage::MidiMessage(const MidiMessage &other) throw()
+    : timeStamp(other.timeStamp),
+      message(other.message),
+      size(other.size)
 {
-    if (other.data != (uint8*) &other.message)
+    if (other.data != (uint8 *)&other.message)
     {
-        data = (uint8*) malloc (size);
-        memcpy (data, other.data, size);
+        data = (uint8 *)malloc(size);
+        memcpy(data, other.data, size);
     }
     else
     {
-        data = (uint8*) &message;
+        data = (uint8 *)&message;
     }
 }
 
-MidiMessage::MidiMessage (const MidiMessage& other,
-                          const double newTimeStamp) throw()
-   : timeStamp (newTimeStamp),
-     message (other.message),
-     size (other.size)
+MidiMessage::MidiMessage(const MidiMessage &other,
+                         const double newTimeStamp) throw()
+    : timeStamp(newTimeStamp),
+      message(other.message),
+      size(other.size)
 {
-    if (other.data != (uint8*) &other.message)
+    if (other.data != (uint8 *)&other.message)
     {
-        data = (uint8*) malloc (size);
-        memcpy (data, other.data, size);
+        data = (uint8 *)malloc(size);
+        memcpy(data, other.data, size);
     }
     else
     {
-        data = (uint8*) &message;
+        data = (uint8 *)&message;
     }
 }
 
-MidiMessage::MidiMessage (const uint8* src,
-                          int sz,
-                          int& numBytesUsed,
-                          const uint8 lastStatusByte,
-                          double t) throw()
-    : timeStamp (t),
-      data ((uint8*) &message),
-      message (0)
+MidiMessage::MidiMessage(const uint8 *src,
+                         int sz,
+                         int &numBytesUsed,
+                         const uint8 lastStatusByte,
+                         double t) throw()
+    : timeStamp(t),
+      data((uint8 *)&message),
+      message(0)
 {
-    unsigned int byte = (unsigned int) *src;
+    unsigned int byte = (unsigned int)*src;
 
     if (byte < 0x80)
     {
-        byte = (unsigned int) (uint8) lastStatusByte;
+        byte = (unsigned int)(uint8)lastStatusByte;
         numBytesUsed = -1;
     }
     else
     {
         numBytesUsed = 0;
         --sz;
         ++src;
     }
 
     if (byte >= 0x80)
     {
         if (byte == 0xf0)
         {
-            const uint8* d = (const uint8*) src;
+            const uint8 *d = (const uint8 *)src;
 
             while (d < src + sz)
             {
                 if (*d >= 0x80) // stop if we hit a status byte, and don't include it in this message
                 {
-                    if (*d == 0xf7)   // include an 0xf7 if we hit one
+                    if (*d == 0xf7) // include an 0xf7 if we hit one
                         ++d;
 
                     break;
                 }
 
                 ++d;
             }
 
-            size = 1 + (int) (d - src);
+            size = 1 + (int)(d - src);
 
-            data = (uint8*) malloc (size);
-            *data = (uint8) byte;
-            memcpy (data + 1, src, size - 1);
+            data = (uint8 *)malloc(size);
+            *data = (uint8)byte;
+            memcpy(data + 1, src, size - 1);
         }
         else if (byte == 0xff)
         {
             int n;
-            const int bytesLeft = readVariableLengthVal (src + 1, n);
-            size = std::min (sz + 1, n + 2 + bytesLeft);
+            const int bytesLeft = readVariableLengthVal(src + 1, n);
+            size = std::min(sz + 1, n + 2 + bytesLeft);
 
-            data = (uint8*) malloc (size);
-            *data = (uint8) byte;
-            memcpy (data + 1, src, size - 1);
+            data = (uint8 *)malloc(size);
+            *data = (uint8)byte;
+            memcpy(data + 1, src, size - 1);
         }
         else
         {
-            size = getMessageLengthFromFirstByte ((uint8) byte);
-            *data = (uint8) byte;
+            size = getMessageLengthFromFirstByte((uint8)byte);
+            *data = (uint8)byte;
 
             if (size > 1)
             {
                 data[1] = src[0];
 
                 if (size > 2)
                     data[2] = src[1];
@@ -293,93 +292,89 @@
     else
     {
         message = 0;
         size = 0;
     }
 }
 
-const MidiMessage& MidiMessage::operator= (const MidiMessage& other) throw()
+const MidiMessage &MidiMessage::operator=(const MidiMessage &other) throw()
 {
     if (this == &other)
         return *this;
 
     timeStamp = other.timeStamp;
     size = other.size;
     message = other.message;
 
-    if (data != (uint8*) &message)
-        free (data);
+    if (data != (uint8 *)&message)
+        free(data);
 
-    if (other.data != (uint8*) &other.message)
+    if (other.data != (uint8 *)&other.message)
     {
-        data = (uint8*) malloc (size);
-        memcpy (data, other.data, size);
+        data = (uint8 *)malloc(size);
+        memcpy(data, other.data, size);
     }
     else
     {
-        data = (uint8*) &message;
+        data = (uint8 *)&message;
     }
 
     return *this;
 }
 
 MidiMessage::~MidiMessage() throw()
 {
-    if (data != (uint8*) &message)
-        free (data);
+    if (data != (uint8 *)&message)
+        free(data);
 }
 
 int MidiMessage::getChannel() const throw()
 {
     if ((data[0] & 0xf0) != 0xf0)
         return (data[0] & 0xf) + 1;
     else
         return 0;
 }
 
-bool MidiMessage::isForChannel (const int channel) const throw()
+bool MidiMessage::isForChannel(const int channel) const throw()
 {
-    return ((data[0] & 0xf) == channel - 1)
-             && ((data[0] & 0xf0) != 0xf0);
+    return ((data[0] & 0xf) == channel - 1) && ((data[0] & 0xf0) != 0xf0);
 }
 
-void MidiMessage::setChannel (const int channel) throw()
+void MidiMessage::setChannel(const int channel) throw()
 {
-    if ((data[0] & 0xf0) != (uint8) 0xf0)
-        data[0] = (uint8) ((data[0] & (uint8)0xf0)
-                            | (uint8)(channel - 1));
+    if ((data[0] & 0xf0) != (uint8)0xf0)
+        data[0] = (uint8)((data[0] & (uint8)0xf0) | (uint8)(channel - 1));
 }
 
 bool MidiMessage::isNoteOn() const throw()
 {
-    return ((data[0] & 0xf0) == 0x90)
-             && (data[2] != 0);
+    return ((data[0] & 0xf0) == 0x90) && (data[2] != 0);
 }
 
 bool MidiMessage::isNoteOff() const throw()
 {
-    return ((data[0] & 0xf0) == 0x80)
-            || ((data[2] == 0) && ((data[0] & 0xf0) == 0x90));
+    return ((data[0] & 0xf0) == 0x80) || ((data[2] == 0) && ((data[0] & 0xf0) == 0x90));
 }
 
 bool MidiMessage::isNoteOnOrOff() const throw()
 {
     const int d = data[0] & 0xf0;
     return (d == 0x90) || (d == 0x80);
 }
 
 int MidiMessage::getNoteNumber() const throw()
 {
     return data[1];
 }
 
-void MidiMessage::setNoteNumber (const int newNoteNumber) throw()
+void MidiMessage::setNoteNumber(const int newNoteNumber) throw()
 {
     if (isNoteOnOrOff())
-        data[1] = (uint8) pklimit (0, 127, newNoteNumber);
+        data[1] = (uint8)pklimit(0, 127, newNoteNumber);
 }
 
 uint8 MidiMessage::getVelocity() const throw()
 {
     if (isNoteOnOrOff())
         return data[2];
     else
@@ -387,238 +382,236 @@
 }
 
 float MidiMessage::getFloatVelocity() const throw()
 {
     return getVelocity() * (1.0f / 127.0f);
 }
 
-void MidiMessage::setVelocity (const float newVelocity) throw()
+void MidiMessage::setVelocity(const float newVelocity) throw()
 {
     if (isNoteOnOrOff())
-        data[2] = (uint8) pklimit (0, 0x7f, roundFloatToInt (newVelocity * 127.0f));
+        data[2] = (uint8)pklimit(0, 0x7f, roundFloatToInt(newVelocity * 127.0f));
 }
 
-void MidiMessage::multiplyVelocity (const float scaleFactor) throw()
+void MidiMessage::multiplyVelocity(const float scaleFactor) throw()
 {
     if (isNoteOnOrOff())
-        data[2] = (uint8) pklimit (0, 0x7f, roundFloatToInt (scaleFactor * data[2]));
+        data[2] = (uint8)pklimit(0, 0x7f, roundFloatToInt(scaleFactor * data[2]));
 }
 
 bool MidiMessage::isAftertouch() const throw()
 {
     return (data[0] & 0xf0) == 0xa0;
 }
 
 int MidiMessage::getAfterTouchValue() const throw()
 {
     return data[2];
 }
 
-const MidiMessage MidiMessage::aftertouchChange (const int channel,
-                                                 const int noteNum,
-                                                 const int aftertouchValue) throw()
-{
-    pkassert (channel > 0 && channel <= 16);
-    pkassert (((unsigned int) noteNum) <= 127);
-    pkassert (((unsigned int) aftertouchValue) <= 127);
-
-    return MidiMessage (0xa0 | pklimit (0, 15, channel - 1),
-                        noteNum & 0x7f,
-                        aftertouchValue & 0x7f);
+const MidiMessage MidiMessage::aftertouchChange(const int channel,
+                                                const int noteNum,
+                                                const int aftertouchValue) throw()
+{
+    pkassert(channel > 0 && channel <= 16);
+    pkassert(((unsigned int)noteNum) <= 127);
+    pkassert(((unsigned int)aftertouchValue) <= 127);
+
+    return MidiMessage(0xa0 | pklimit(0, 15, channel - 1),
+                       noteNum & 0x7f,
+                       aftertouchValue & 0x7f);
 }
 
 bool MidiMessage::isChannelPressure() const throw()
 {
     return (data[0] & 0xf0) == 0xd0;
 }
 
 int MidiMessage::getChannelPressureValue() const throw()
 {
-    pkassert (isChannelPressure());
+    pkassert(isChannelPressure());
 
     return data[1];
 }
 
-const MidiMessage MidiMessage::channelPressureChange (const int channel,
-                                                      const int pressure) throw()
+const MidiMessage MidiMessage::channelPressureChange(const int channel,
+                                                     const int pressure) throw()
 {
-    pkassert (channel > 0 && channel <= 16);
-    pkassert (((unsigned int) pressure) <= 127);
+    pkassert(channel > 0 && channel <= 16);
+    pkassert(((unsigned int)pressure) <= 127);
 
-    return MidiMessage (0xd0 | pklimit (0, 15, channel - 1),
-                        pressure & 0x7f);
+    return MidiMessage(0xd0 | pklimit(0, 15, channel - 1),
+                       pressure & 0x7f);
 }
 
 bool MidiMessage::isProgramChange() const throw()
 {
     return (data[0] & 0xf0) == 0xc0;
 }
 
 int MidiMessage::getProgramChangeNumber() const throw()
 {
     return data[1];
 }
 
-const MidiMessage MidiMessage::programChange (const int channel,
-                                              const int programNumber) throw()
+const MidiMessage MidiMessage::programChange(const int channel,
+                                             const int programNumber) throw()
 {
-    pkassert (channel > 0 && channel <= 16);
+    pkassert(channel > 0 && channel <= 16);
 
-    return MidiMessage (0xc0 | pklimit (0, 15, channel - 1),
-                        programNumber & 0x7f);
+    return MidiMessage(0xc0 | pklimit(0, 15, channel - 1),
+                       programNumber & 0x7f);
 }
 
 bool MidiMessage::isPitchWheel() const throw()
 {
     return (data[0] & 0xf0) == 0xe0;
 }
 
 int MidiMessage::getPitchWheelValue() const throw()
 {
     return data[1] | (data[2] << 7);
 }
 
-const MidiMessage MidiMessage::pitchWheel (const int channel,
-                                           const int position) throw()
+const MidiMessage MidiMessage::pitchWheel(const int channel,
+                                          const int position) throw()
 {
-    pkassert (channel > 0 && channel <= 16);
-    pkassert (((unsigned int) position) <= 0x3fff);
+    pkassert(channel > 0 && channel <= 16);
+    pkassert(((unsigned int)position) <= 0x3fff);
 
-    return MidiMessage (0xe0 | pklimit (0, 15, channel - 1),
-                        position & 127,
-                        (position >> 7) & 127);
+    return MidiMessage(0xe0 | pklimit(0, 15, channel - 1),
+                       position & 127,
+                       (position >> 7) & 127);
 }
 
 bool MidiMessage::isController() const throw()
 {
     return (data[0] & 0xf0) == 0xb0;
 }
 
 int MidiMessage::getControllerNumber() const throw()
 {
-    pkassert (isController());
+    pkassert(isController());
 
     return data[1];
 }
 
 int MidiMessage::getControllerValue() const throw()
 {
-    pkassert (isController());
+    pkassert(isController());
 
     return data[2];
 }
 
-const MidiMessage MidiMessage::controllerEvent (const int channel,
-                                                const int controllerType,
-                                                const int value) throw()
+const MidiMessage MidiMessage::controllerEvent(const int channel,
+                                               const int controllerType,
+                                               const int value) throw()
 {
     // the channel must be between 1 and 16 inclusive
-    pkassert (channel > 0 && channel <= 16);
+    pkassert(channel > 0 && channel <= 16);
 
-    return MidiMessage (0xb0 | pklimit (0, 15, channel - 1),
-                        controllerType & 127,
-                        value & 127);
+    return MidiMessage(0xb0 | pklimit(0, 15, channel - 1),
+                       controllerType & 127,
+                       value & 127);
 }
 
-const MidiMessage MidiMessage::noteOn (const int channel,
-                                       const int noteNumber,
-                                       const float velocity) throw()
+const MidiMessage MidiMessage::noteOn(const int channel,
+                                      const int noteNumber,
+                                      const float velocity) throw()
 {
-    return noteOn (channel, noteNumber, (uint8)(velocity * 127.0f));
+    return noteOn(channel, noteNumber, (uint8)(velocity * 127.0f));
 }
 
-const MidiMessage MidiMessage::noteOn (const int channel,
-                                       const int noteNumber,
-                                       const uint8 velocity) throw()
+const MidiMessage MidiMessage::noteOn(const int channel,
+                                      const int noteNumber,
+                                      const uint8 velocity) throw()
 {
-    pkassert (channel > 0 && channel <= 16);
-    pkassert (((unsigned int) noteNumber) <= 127);
+    pkassert(channel > 0 && channel <= 16);
+    pkassert(((unsigned int)noteNumber) <= 127);
 
-    return MidiMessage (0x90 | pklimit (0, 15, channel - 1),
-                        noteNumber & 127,
-                        pklimit (0, 127, roundFloatToInt (velocity)));
+    return MidiMessage(0x90 | pklimit(0, 15, channel - 1),
+                       noteNumber & 127,
+                       pklimit(0, 127, roundFloatToInt(velocity)));
 }
 
-const MidiMessage MidiMessage::noteOff (const int channel,
-                                        const int noteNumber) throw()
+const MidiMessage MidiMessage::noteOff(const int channel,
+                                       const int noteNumber) throw()
 {
-    pkassert (channel > 0 && channel <= 16);
-    pkassert (((unsigned int) noteNumber) <= 127);
+    pkassert(channel > 0 && channel <= 16);
+    pkassert(((unsigned int)noteNumber) <= 127);
 
-    return MidiMessage (0x80 | pklimit (0, 15, channel - 1), noteNumber & 127, 0);
+    return MidiMessage(0x80 | pklimit(0, 15, channel - 1), noteNumber & 127, 0);
 }
 
-const MidiMessage MidiMessage::allNotesOff (const int channel) throw()
+const MidiMessage MidiMessage::allNotesOff(const int channel) throw()
 {
-    pkassert (channel > 0 && channel <= 16);
+    pkassert(channel > 0 && channel <= 16);
 
-    return controllerEvent (channel, 123, 0);
+    return controllerEvent(channel, 123, 0);
 }
 
 bool MidiMessage::isAllNotesOff() const throw()
 {
-    return (data[0] & 0xf0) == 0xb0
-            && data[1] == 123;
+    return (data[0] & 0xf0) == 0xb0 && data[1] == 123;
 }
 
-const MidiMessage MidiMessage::allSoundOff (const int channel) throw()
+const MidiMessage MidiMessage::allSoundOff(const int channel) throw()
 {
-    return controllerEvent (channel, 120, 0);
+    return controllerEvent(channel, 120, 0);
 }
 
 bool MidiMessage::isAllSoundOff() const throw()
 {
-    return (data[0] & 0xf0) == 0xb0
-             && data[1] == 120;
+    return (data[0] & 0xf0) == 0xb0 && data[1] == 120;
 }
 
-const MidiMessage MidiMessage::allControllersOff (const int channel) throw()
+const MidiMessage MidiMessage::allControllersOff(const int channel) throw()
 {
-    return controllerEvent (channel, 121, 0);
+    return controllerEvent(channel, 121, 0);
 }
 
-const MidiMessage MidiMessage::masterVolume (const float volume) throw()
+const MidiMessage MidiMessage::masterVolume(const float volume) throw()
 {
-    const int vol = pklimit (0, 0x3fff, roundFloatToInt (volume * 0x4000));
+    const int vol = pklimit(0, 0x3fff, roundFloatToInt(volume * 0x4000));
 
     uint8 buf[8];
     buf[0] = 0xf0;
     buf[1] = 0x7f;
     buf[2] = 0x7f;
     buf[3] = 0x04;
     buf[4] = 0x01;
-    buf[5] = (uint8) (vol & 0x7f);
-    buf[6] = (uint8) (vol >> 7);
+    buf[5] = (uint8)(vol & 0x7f);
+    buf[6] = (uint8)(vol >> 7);
     buf[7] = 0xf7;
 
-    return MidiMessage (buf, 8);
+    return MidiMessage(buf, 8);
 }
 
 //==============================================================================
 bool MidiMessage::isSysEx() const throw()
 {
     return *data == 0xf0;
 }
 
-const MidiMessage MidiMessage::createSysExMessage (const uint8* sysexData,
-                                                   const int dataSize) throw()
+const MidiMessage MidiMessage::createSysExMessage(const uint8 *sysexData,
+                                                  const int dataSize) throw()
 {
-    uint8* const m = (uint8*) malloc(dataSize + 2);
+    uint8 *const m = (uint8 *)malloc(dataSize + 2);
     BlobKiller k(m);
 
     m[0] = 0xf0;
-    memcpy (m + 1, sysexData, dataSize);
+    memcpy(m + 1, sysexData, dataSize);
     m[dataSize + 1] = 0xf7;
 
-    return MidiMessage (m, dataSize + 2);
+    return MidiMessage(m, dataSize + 2);
 }
 
-const uint8* MidiMessage::getSysExData() const throw()
+const uint8 *MidiMessage::getSysExData() const throw()
 {
-  return (isSysEx()) ? (uint8 *)getRawData() + 1
+    return (isSysEx()) ? (uint8 *)getRawData() + 1
                        : 0;
 }
 
 int MidiMessage::getSysExDataSize() const throw()
 {
     return (isSysEx()) ? size - 2
                        : 0;
@@ -644,25 +637,25 @@
 }
 
 int MidiMessage::getMetaEventLength() const throw()
 {
     if (*data == 0xff)
     {
         int n;
-        return std::min (size - 2, readVariableLengthVal (data + 2, n));
+        return std::min(size - 2, readVariableLengthVal(data + 2, n));
     }
 
     return 0;
 }
 
-const uint8* MidiMessage::getMetaEventData() const throw()
+const uint8 *MidiMessage::getMetaEventData() const throw()
 {
     int n;
-    const uint8* d = data + 2;
-    readVariableLengthVal (d, n);
+    const uint8 *d = data + 2;
+    readVariableLengthVal(d, n);
     return d + n;
 }
 
 bool MidiMessage::isTrackMetaEvent() const throw()
 {
     return getMetaEventType() == 0;
 }
@@ -677,512 +670,503 @@
     const int t = getMetaEventType();
 
     return t > 0 && t < 16;
 }
 
 const char *MidiMessage::getTextFromTextMetaEvent() const throw()
 {
-    return (const char*) getMetaEventData();
+    return (const char *)getMetaEventData();
 }
 
 bool MidiMessage::isTrackNameEvent() const throw()
 {
-    return (data[1] == 3)
-            && (*data == 0xff);
+    return (data[1] == 3) && (*data == 0xff);
 }
 
 bool MidiMessage::isTempoMetaEvent() const throw()
 {
-    return (data[1] == 81)
-            && (*data == 0xff);
+    return (data[1] == 81) && (*data == 0xff);
 }
 
 bool MidiMessage::isMidiChannelMetaEvent() const throw()
 {
-    return (data[1] == 0x20)
-            && (*data == 0xff)
-            && (data[2] == 1);
+    return (data[1] == 0x20) && (*data == 0xff) && (data[2] == 1);
 }
 
 int MidiMessage::getMidiChannelMetaEventChannel() const throw()
 {
     return data[3] + 1;
 }
 
 double MidiMessage::getTempoSecondsPerQuarterNote() const throw()
 {
-    if (! isTempoMetaEvent())
+    if (!isTempoMetaEvent())
         return 0.0;
 
-    const uint8* const d = getMetaEventData();
+    const uint8 *const d = getMetaEventData();
 
-    return (((unsigned int) d[0] << 16)
-             | ((unsigned int) d[1] << 8)
-             | d[2])
-            / 1000000.0;
+    return (((unsigned int)d[0] << 16) | ((unsigned int)d[1] << 8) | d[2]) / 1000000.0;
 }
 
-double MidiMessage::getTempoMetaEventTickLength (const short timeFormat) const throw()
+double MidiMessage::getTempoMetaEventTickLength(const short timeFormat) const throw()
 {
     if (timeFormat > 0)
     {
-        if (! isTempoMetaEvent())
+        if (!isTempoMetaEvent())
             return 0.5 / timeFormat;
 
         return getTempoSecondsPerQuarterNote() / timeFormat;
     }
     else
     {
         const int frameCode = (-timeFormat) >> 8;
         double framesPerSecond;
 
         switch (frameCode)
         {
-            case 24: framesPerSecond = 24.0;   break;
-            case 25: framesPerSecond = 25.0;   break;
-            case 29: framesPerSecond = 29.97;  break;
-            case 30: framesPerSecond = 30.0;   break;
-            default: framesPerSecond = 30.0;   break;
+        case 24:
+            framesPerSecond = 24.0;
+            break;
+        case 25:
+            framesPerSecond = 25.0;
+            break;
+        case 29:
+            framesPerSecond = 29.97;
+            break;
+        case 30:
+            framesPerSecond = 30.0;
+            break;
+        default:
+            framesPerSecond = 30.0;
+            break;
         }
 
         return (1.0 / framesPerSecond) / (timeFormat & 0xff);
     }
 }
 
-const MidiMessage MidiMessage::tempoMetaEvent (int microsecondsPerQuarterNote) throw()
+const MidiMessage MidiMessage::tempoMetaEvent(int microsecondsPerQuarterNote) throw()
 {
     uint8 d[8];
     d[0] = 0xff;
     d[1] = 81;
     d[2] = 3;
-    d[3] = (uint8) (microsecondsPerQuarterNote >> 16);
-    d[4] = (uint8) ((microsecondsPerQuarterNote >> 8) & 0xff);
-    d[5] = (uint8) (microsecondsPerQuarterNote & 0xff);
+    d[3] = (uint8)(microsecondsPerQuarterNote >> 16);
+    d[4] = (uint8)((microsecondsPerQuarterNote >> 8) & 0xff);
+    d[5] = (uint8)(microsecondsPerQuarterNote & 0xff);
 
-    return MidiMessage (d, 6, 0.0);
+    return MidiMessage(d, 6, 0.0);
 }
 
 bool MidiMessage::isTimeSignatureMetaEvent() const throw()
 {
-    return (data[1] == 0x58)
-             && (*data == (uint8) 0xff);
+    return (data[1] == 0x58) && (*data == (uint8)0xff);
 }
 
-void MidiMessage::getTimeSignatureInfo (int& numerator,
-                                        int& denominator) const throw()
+void MidiMessage::getTimeSignatureInfo(int &numerator,
+                                       int &denominator) const throw()
 {
     if (isTimeSignatureMetaEvent())
     {
-        const uint8* const d = getMetaEventData();
+        const uint8 *const d = getMetaEventData();
         numerator = d[0];
         denominator = 1 << d[1];
     }
     else
     {
         numerator = 4;
         denominator = 4;
     }
 }
 
-const MidiMessage MidiMessage::timeSignatureMetaEvent (const int numerator,
-                                                       const int denominator) throw()
+const MidiMessage MidiMessage::timeSignatureMetaEvent(const int numerator,
+                                                      const int denominator) throw()
 {
     uint8 d[8];
     d[0] = 0xff;
     d[1] = 0x58;
     d[2] = 0x04;
-    d[3] = (uint8) numerator;
+    d[3] = (uint8)numerator;
 
     int n = 1;
     int powerOfTwo = 0;
 
     while (n < denominator)
     {
         n <<= 1;
         ++powerOfTwo;
     }
 
-    d[4] = (uint8) powerOfTwo;
+    d[4] = (uint8)powerOfTwo;
     d[5] = 0x01;
     d[6] = 96;
 
-    return MidiMessage (d, 7, 0.0);
+    return MidiMessage(d, 7, 0.0);
 }
 
-const MidiMessage MidiMessage::midiChannelMetaEvent (const int channel) throw()
+const MidiMessage MidiMessage::midiChannelMetaEvent(const int channel) throw()
 {
     uint8 d[8];
     d[0] = 0xff;
     d[1] = 0x20;
     d[2] = 0x01;
-    d[3] = (uint8) pklimit (0, 0xff, channel - 1);
+    d[3] = (uint8)pklimit(0, 0xff, channel - 1);
 
-    return MidiMessage (d, 4, 0.0);
+    return MidiMessage(d, 4, 0.0);
 }
 
 bool MidiMessage::isKeySignatureMetaEvent() const throw()
 {
     return getMetaEventType() == 89;
 }
 
 int MidiMessage::getKeySignatureNumberOfSharpsOrFlats() const throw()
 {
-    return (int) *getMetaEventData();
+    return (int)*getMetaEventData();
 }
 
 const MidiMessage MidiMessage::endOfTrack() throw()
 {
-    return MidiMessage (0xff, 0x2f, 0, 0.0);
+    return MidiMessage(0xff, 0x2f, 0, 0.0);
 }
 
 //==============================================================================
 bool MidiMessage::isSongPositionPointer() const throw()
 {
     return *data == 0xf2;
 }
 
 int MidiMessage::getSongPositionPointerMidiBeat() const throw()
 {
     return data[1] | (data[2] << 7);
 }
 
-const MidiMessage MidiMessage::songPositionPointer (const int positionInMidiBeats) throw()
+const MidiMessage MidiMessage::songPositionPointer(const int positionInMidiBeats) throw()
 {
-    return MidiMessage (0xf2,
-                        positionInMidiBeats & 127,
-                        (positionInMidiBeats >> 7) & 127);
+    return MidiMessage(0xf2,
+                       positionInMidiBeats & 127,
+                       (positionInMidiBeats >> 7) & 127);
 }
 
 bool MidiMessage::isMidiStart() const throw()
 {
     return *data == 0xfa;
 }
 
 const MidiMessage MidiMessage::midiStart() throw()
 {
-    return MidiMessage (0xfa);
+    return MidiMessage(0xfa);
 }
 
 bool MidiMessage::isMidiContinue() const throw()
 {
     return *data == 0xfb;
 }
 
 const MidiMessage MidiMessage::midiContinue() throw()
 {
-    return MidiMessage (0xfb);
+    return MidiMessage(0xfb);
 }
 
 bool MidiMessage::isMidiStop() const throw()
 {
     return *data == 0xfc;
 }
 
 const MidiMessage MidiMessage::midiStop() throw()
 {
-    return MidiMessage (0xfc);
+    return MidiMessage(0xfc);
 }
 
 bool MidiMessage::isMidiClock() const throw()
 {
     return *data == 0xf8;
 }
 
 const MidiMessage MidiMessage::midiClock() throw()
 {
-    return MidiMessage (0xf8);
+    return MidiMessage(0xf8);
 }
 
 bool MidiMessage::isQuarterFrame() const throw()
 {
     return *data == 0xf1;
 }
 
 int MidiMessage::getQuarterFrameSequenceNumber() const throw()
 {
-    return ((int) data[1]) >> 4;
+    return ((int)data[1]) >> 4;
 }
 
 int MidiMessage::getQuarterFrameValue() const throw()
 {
-    return ((int) data[1]) & 0x0f;
+    return ((int)data[1]) & 0x0f;
 }
 
-const MidiMessage MidiMessage::quarterFrame (const int sequenceNumber,
-                                             const int value) throw()
+const MidiMessage MidiMessage::quarterFrame(const int sequenceNumber,
+                                            const int value) throw()
 {
-    return MidiMessage (0xf1, (sequenceNumber << 4) | value);
+    return MidiMessage(0xf1, (sequenceNumber << 4) | value);
 }
 
 bool MidiMessage::isFullFrame() const throw()
 {
-    return data[0] == 0xf0
-            && data[1] == 0x7f
-            && size >= 10
-            && data[3] == 0x01
-            && data[4] == 0x01;
-}
-
-void MidiMessage::getFullFrameParameters (int& hours,
-                                          int& minutes,
-                                          int& seconds,
-                                          int& frames,
-                                          MidiMessage::SmpteTimecodeType& timecodeType) const throw()
+    return data[0] == 0xf0 && data[1] == 0x7f && size >= 10 && data[3] == 0x01 && data[4] == 0x01;
+}
+
+void MidiMessage::getFullFrameParameters(int &hours,
+                                         int &minutes,
+                                         int &seconds,
+                                         int &frames,
+                                         MidiMessage::SmpteTimecodeType &timecodeType) const throw()
 {
-    pkassert (isFullFrame());
+    pkassert(isFullFrame());
 
-    timecodeType = (SmpteTimecodeType) (data[5] >> 5);
-    hours   = data[5] & 0x1f;
+    timecodeType = (SmpteTimecodeType)(data[5] >> 5);
+    hours = data[5] & 0x1f;
     minutes = data[6];
     seconds = data[7];
-    frames  = data[8];
+    frames = data[8];
 }
 
-const MidiMessage MidiMessage::fullFrame (const int hours,
-                                          const int minutes,
-                                          const int seconds,
-                                          const int frames,
-                                          MidiMessage::SmpteTimecodeType timecodeType)
+const MidiMessage MidiMessage::fullFrame(const int hours,
+                                         const int minutes,
+                                         const int seconds,
+                                         const int frames,
+                                         MidiMessage::SmpteTimecodeType timecodeType)
 {
     uint8 d[10];
     d[0] = 0xf0;
     d[1] = 0x7f;
     d[2] = 0x7f;
     d[3] = 0x01;
     d[4] = 0x01;
-    d[5] = (uint8) ((hours & 0x01f) | (timecodeType << 5));
-    d[6] = (uint8) minutes;
-    d[7] = (uint8) seconds;
-    d[8] = (uint8) frames;
+    d[5] = (uint8)((hours & 0x01f) | (timecodeType << 5));
+    d[6] = (uint8)minutes;
+    d[7] = (uint8)seconds;
+    d[8] = (uint8)frames;
     d[9] = 0xf7;
 
-    return MidiMessage (d, 10, 0.0);
+    return MidiMessage(d, 10, 0.0);
 }
 
 bool MidiMessage::isMidiMachineControlMessage() const throw()
 {
-    return data[0] == 0xf0
-        && data[1] == 0x7f
-        && data[3] == 0x06
-        && size > 5;
+    return data[0] == 0xf0 && data[1] == 0x7f && data[3] == 0x06 && size > 5;
 }
 
 MidiMessage::MidiMachineControlCommand MidiMessage::getMidiMachineControlCommand() const throw()
 {
-    pkassert (isMidiMachineControlMessage());
+    pkassert(isMidiMachineControlMessage());
 
-    return (MidiMachineControlCommand) data[4];
+    return (MidiMachineControlCommand)data[4];
 }
 
-const MidiMessage MidiMessage::midiMachineControlCommand (MidiMessage::MidiMachineControlCommand command)
+const MidiMessage MidiMessage::midiMachineControlCommand(MidiMessage::MidiMachineControlCommand command)
 {
     uint8 d[6];
     d[0] = 0xf0;
     d[1] = 0x7f;
     d[2] = 0x00;
     d[3] = 0x06;
-    d[4] = (uint8) command;
+    d[4] = (uint8)command;
     d[5] = 0xf7;
 
-    return MidiMessage (d, 6, 0.0);
+    return MidiMessage(d, 6, 0.0);
 }
 
 //==============================================================================
-bool MidiMessage::isMidiMachineControlGoto (int& hours,
-                                            int& minutes,
-                                            int& seconds,
-                                            int& frames) const throw()
-{
-    if (size >= 12
-         && data[0] == 0xf0
-         && data[1] == 0x7f
-         && data[3] == 0x06
-         && data[4] == 0x44
-         && data[5] == 0x06
-         && data[6] == 0x01)
+bool MidiMessage::isMidiMachineControlGoto(int &hours,
+                                           int &minutes,
+                                           int &seconds,
+                                           int &frames) const throw()
+{
+    if (size >= 12 && data[0] == 0xf0 && data[1] == 0x7f && data[3] == 0x06 && data[4] == 0x44 && data[5] == 0x06 && data[6] == 0x01)
     {
-        hours = data[7] % 24;   // (that some machines send out hours > 24)
+        hours = data[7] % 24; // (that some machines send out hours > 24)
         minutes = data[8];
         seconds = data[9];
         frames = data[10];
 
         return true;
     }
 
     return false;
 }
 
-const MidiMessage MidiMessage::midiMachineControlGoto (int hours,
-                                                       int minutes,
-                                                       int seconds,
-                                                       int frames)
+const MidiMessage MidiMessage::midiMachineControlGoto(int hours,
+                                                      int minutes,
+                                                      int seconds,
+                                                      int frames)
 {
     uint8 d[12];
     d[0] = 0xf0;
     d[1] = 0x7f;
     d[2] = 0x00;
     d[3] = 0x06;
     d[4] = 0x44;
     d[5] = 0x06;
     d[6] = 0x01;
-    d[7] = (uint8) hours;
-    d[8] = (uint8) minutes;
-    d[9] = (uint8) seconds;
-    d[10] = (uint8) frames;
+    d[7] = (uint8)hours;
+    d[8] = (uint8)minutes;
+    d[9] = (uint8)seconds;
+    d[10] = (uint8)frames;
     d[11] = 0xf7;
 
-    return MidiMessage (d, 12, 0.0);
+    return MidiMessage(d, 12, 0.0);
 }
 
 //==============================================================================
-const char *MidiMessage::getMidiNoteName (int note,
-                                           bool useSharps,
-                                           bool includeOctaveNumber,
-                                           int octaveNumForMiddleC) throw()
-{
-    static const char* const sharpNoteNames[] = { "C", "C#", "D", "D#", "E",
-                                                  "F", "F#", "G", "G#", "A",
-                                                  "A#", "B" };
-
-    static const char* const flatNoteNames[]  = { "C", "Db", "D", "Eb", "E",
-                                                  "F", "Gb", "G", "Ab", "A",
-                                                  "Bb", "B" };
-
-    if (((unsigned int) note) < 128)
-    {
-      static char buf[16];
-      const char *noteName = (useSharps) ? sharpNoteNames [note % 12] : flatNoteNames [note % 12];
-      if (includeOctaveNumber)
-        sprintf(buf, "%s%i", noteName, note / 12 + (octaveNumForMiddleC - 5));
-      else
-        sprintf(buf, "%s", noteName);
-      return buf;      
+const char *MidiMessage::getMidiNoteName(int note,
+                                         bool useSharps,
+                                         bool includeOctaveNumber,
+                                         int octaveNumForMiddleC) throw()
+{
+    static const char *const sharpNoteNames[] = {"C", "C#", "D", "D#", "E",
+                                                 "F", "F#", "G", "G#", "A",
+                                                 "A#", "B"};
+
+    static const char *const flatNoteNames[] = {"C", "Db", "D", "Eb", "E",
+                                                "F", "Gb", "G", "Ab", "A",
+                                                "Bb", "B"};
+
+    if (((unsigned int)note) < 128)
+    {
+        static char buf[16];
+        const char *noteName = (useSharps) ? sharpNoteNames[note % 12] : flatNoteNames[note % 12];
+        if (includeOctaveNumber)
+            sprintf(buf, "%s%i", noteName, note / 12 + (octaveNumForMiddleC - 5));
+        else
+            sprintf(buf, "%s", noteName);
+        return buf;
     }
 
     return 0;
 }
 
-const double MidiMessage::getMidiNoteInHertz (int noteNumber) throw()
+const double MidiMessage::getMidiNoteInHertz(int noteNumber) throw()
 {
     noteNumber -= 12 * 6 + 9; // now 0 = A440
-    return 440.0 * pow (2.0, noteNumber / 12.0);
+    return 440.0 * pow(2.0, noteNumber / 12.0);
 }
 
-const char *MidiMessage::getGMInstrumentName (int n) throw()
+const char *MidiMessage::getGMInstrumentName(int n) throw()
 {
     const char *names[] =
-    {
-        "Acoustic Grand Piano", "Bright Acoustic Piano", "Electric Grand Piano", "Honky-tonk Piano",
-        "Electric Piano 1", "Electric Piano 2", "Harpsichord", "Clavinet", "Celesta", "Glockenspiel",
-        "Music Box", "Vibraphone", "Marimba", "Xylophone", "Tubular Bells", "Dulcimer", "Drawbar Organ",
-        "Percussive Organ", "Rock Organ", "Church Organ", "Reed Organ", "Accordion", "Harmonica",
-        "Tango Accordion", "Acoustic Guitar (nylon)", "Acoustic Guitar (steel)", "Electric Guitar (jazz)",
-        "Electric Guitar (clean)", "Electric Guitar (mute)", "Overdriven Guitar", "Distortion Guitar",
-        "Guitar Harmonics", "Acoustic Bass", "Electric Bass (finger)", "Electric Bass (pick)",
-        "Fretless Bass", "Slap Bass 1", "Slap Bass 2", "Synth Bass 1", "Synth Bass 2", "Violin",
-        "Viola", "Cello", "Contrabass", "Tremolo Strings", "Pizzicato Strings", "Orchestral Harp",
-        "Timpani", "String Ensemble 1", "String Ensemble 2", "SynthStrings 1", "SynthStrings 2",
-        "Choir Aahs", "Voice Oohs", "Synth Voice", "Orchestra Hit", "Trumpet", "Trombone", "Tuba",
-        "Muted Trumpet", "French Horn", "Brass Section", "SynthBrass 1", "SynthBrass 2", "Soprano Sax",
-        "Alto Sax", "Tenor Sax", "Baritone Sax", "Oboe", "English Horn", "Bassoon", "Clarinet",
-        "Piccolo", "Flute", "Recorder", "Pan Flute", "Blown Bottle", "Shakuhachi", "Whistle",
-        "Ocarina", "Lead 1 (square)", "Lead 2 (sawtooth)", "Lead 3 (calliope)", "Lead 4 (chiff)",
-        "Lead 5 (charang)", "Lead 6 (voice)", "Lead 7 (fifths)", "Lead 8 (bass+lead)", "Pad 1 (new age)",
-        "Pad 2 (warm)", "Pad 3 (polysynth)", "Pad 4 (choir)", "Pad 5 (bowed)", "Pad 6 (metallic)",
-        "Pad 7 (halo)", "Pad 8 (sweep)", "FX 1 (rain)", "FX 2 (soundtrack)", "FX 3 (crystal)",
-        "FX 4 (atmosphere)", "FX 5 (brightness)", "FX 6 (goblins)", "FX 7 (echoes)", "FX 8 (sci-fi)",
-        "Sitar", "Banjo", "Shamisen", "Koto", "Kalimba", "Bag pipe", "Fiddle", "Shanai", "Tinkle Bell",
-        "Agogo", "Steel Drums", "Woodblock", "Taiko Drum", "Melodic Tom", "Synth Drum", "Reverse Cymbal",
-        "Guitar Fret Noise", "Breath Noise", "Seashore", "Bird Tweet", "Telephone Ring", "Helicopter",
-        "Applause", "Gunshot"
-    };
-
-    return (((unsigned int) n) < 128) ? names[n] : 0;
-}
-
-const char *MidiMessage::getGMInstrumentBankName (int n) throw()
-{
-    const char* names[] =
-    {
-        "Piano", "Chromatic Percussion", "Organ", "Guitar",
-        "Bass", "Strings", "Ensemble", "Brass",
-        "Reed", "Pipe", "Synth Lead", "Synth Pad",
-        "Synth Effects", "Ethnic", "Percussive", "Sound Effects"
-    };
-
-    return (((unsigned int) n) <= 15) ? names[n] : 0;
-}
-
-const char *MidiMessage::getRhythmInstrumentName (int n) throw()
-{
-    const char* names[] =
-    {
-        "Acoustic Bass Drum", "Bass Drum 1", "Side Stick", "Acoustic Snare",
-        "Hand Clap", "Electric Snare", "Low Floor Tom", "Closed Hi-Hat", "High Floor Tom",
-        "Pedal Hi-Hat", "Low Tom", "Open Hi-Hat", "Low-Mid Tom", "Hi-Mid Tom", "Crash Cymbal 1",
-        "High Tom", "Ride Cymbal 1", "Chinese Cymbal", "Ride Bell", "Tambourine", "Splash Cymbal",
-        "Cowbell", "Crash Cymbal 2", "Vibraslap", "Ride Cymbal 2", "Hi Bongo", "Low Bongo",
-        "Mute Hi Conga", "Open Hi Conga", "Low Conga", "High Timbale", "Low Timbale", "High Agogo",
-        "Low Agogo", "Cabasa", "Maracas", "Short Whistle", "Long Whistle", "Short Guiro",
-        "Long Guiro", "Claves", "Hi Wood Block", "Low Wood Block", "Mute Cuica", "Open Cuica",
-        "Mute Triangle", "Open Triangle"
-    };
-
-  return (n >= 35 && n <= 81) ? names [n - 35] : 0;
-}
-
-const char *MidiMessage::getControllerName (int n) throw()
-{
-    const char* names[] =
-    {
-        "Bank Select", "Modulation Wheel (coarse)", "Breath controller (coarse)",
-        0, "Foot Pedal (coarse)", "Portamento Time (coarse)",
-        "Data Entry (coarse)", "Volume (coarse)", "Balance (coarse)",
-        0, "Pan position (coarse)", "Expression (coarse)", "Effect Control 1 (coarse)",
-        "Effect Control 2 (coarse)", 0, 0, "General Purpose Slider 1", "General Purpose Slider 2",
-        "General Purpose Slider 3", "General Purpose Slider 4", 0, 0, 0, 0, 0, 0, 0, 0,
-        0, 0, 0, 0, "Bank Select (fine)", "Modulation Wheel (fine)", "Breath controller (fine)",
-        0, "Foot Pedal (fine)", "Portamento Time (fine)", "Data Entry (fine)", "Volume (fine)",
-        "Balance (fine)", 0, "Pan position (fine)", "Expression (fine)", "Effect Control 1 (fine)",
-        "Effect Control 2 (fine)", 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
-        "Hold Pedal (on/off)", "Portamento (on/off)", "Sustenuto Pedal (on/off)", "Soft Pedal (on/off)",
-        "Legato Pedal (on/off)", "Hold 2 Pedal (on/off)", "Sound Variation", "Sound Timbre",
-        "Sound Release Time", "Sound Attack Time", "Sound Brightness", "Sound Control 6",
-        "Sound Control 7", "Sound Control 8", "Sound Control 9", "Sound Control 10",
-        "General Purpose Button 1 (on/off)", "General Purpose Button 2 (on/off)",
-        "General Purpose Button 3 (on/off)", "General Purpose Button 4 (on/off)",
-        0, 0, 0, 0, 0, 0, 0, "Reverb Level", "Tremolo Level",  "Chorus Level", "Celeste Level",
-        "Phaser Level", "Data Button increment", "Data Button decrement", "Non-registered Parameter (fine)",
-        "Non-registered Parameter (coarse)", "Registered Parameter (fine)", "Registered Parameter (coarse)",
-        0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, "All Sound Off", "All Controllers Off",
-        "Local Keyboard (on/off)", "All Notes Off", "Omni Mode Off", "Omni Mode On", "Mono Operation",
-        "Poly Operation"
-    };
-
-    const char *ret = ( ((unsigned int) n) < 128) ? names[n] : "";
-    if(ret != 0)
-      return ret;
+        {
+            "Acoustic Grand Piano", "Bright Acoustic Piano", "Electric Grand Piano", "Honky-tonk Piano",
+            "Electric Piano 1", "Electric Piano 2", "Harpsichord", "Clavinet", "Celesta", "Glockenspiel",
+            "Music Box", "Vibraphone", "Marimba", "Xylophone", "Tubular Bells", "Dulcimer", "Drawbar Organ",
+            "Percussive Organ", "Rock Organ", "Church Organ", "Reed Organ", "Accordion", "Harmonica",
+            "Tango Accordion", "Acoustic Guitar (nylon)", "Acoustic Guitar (steel)", "Electric Guitar (jazz)",
+            "Electric Guitar (clean)", "Electric Guitar (mute)", "Overdriven Guitar", "Distortion Guitar",
+            "Guitar Harmonics", "Acoustic Bass", "Electric Bass (finger)", "Electric Bass (pick)",
+            "Fretless Bass", "Slap Bass 1", "Slap Bass 2", "Synth Bass 1", "Synth Bass 2", "Violin",
+            "Viola", "Cello", "Contrabass", "Tremolo Strings", "Pizzicato Strings", "Orchestral Harp",
+            "Timpani", "String Ensemble 1", "String Ensemble 2", "SynthStrings 1", "SynthStrings 2",
+            "Choir Aahs", "Voice Oohs", "Synth Voice", "Orchestra Hit", "Trumpet", "Trombone", "Tuba",
+            "Muted Trumpet", "French Horn", "Brass Section", "SynthBrass 1", "SynthBrass 2", "Soprano Sax",
+            "Alto Sax", "Tenor Sax", "Baritone Sax", "Oboe", "English Horn", "Bassoon", "Clarinet",
+            "Piccolo", "Flute", "Recorder", "Pan Flute", "Blown Bottle", "Shakuhachi", "Whistle",
+            "Ocarina", "Lead 1 (square)", "Lead 2 (sawtooth)", "Lead 3 (calliope)", "Lead 4 (chiff)",
+            "Lead 5 (charang)", "Lead 6 (voice)", "Lead 7 (fifths)", "Lead 8 (bass+lead)", "Pad 1 (new age)",
+            "Pad 2 (warm)", "Pad 3 (polysynth)", "Pad 4 (choir)", "Pad 5 (bowed)", "Pad 6 (metallic)",
+            "Pad 7 (halo)", "Pad 8 (sweep)", "FX 1 (rain)", "FX 2 (soundtrack)", "FX 3 (crystal)",
+            "FX 4 (atmosphere)", "FX 5 (brightness)", "FX 6 (goblins)", "FX 7 (echoes)", "FX 8 (sci-fi)",
+            "Sitar", "Banjo", "Shamisen", "Koto", "Kalimba", "Bag pipe", "Fiddle", "Shanai", "Tinkle Bell",
+            "Agogo", "Steel Drums", "Woodblock", "Taiko Drum", "Melodic Tom", "Synth Drum", "Reverse Cymbal",
+            "Guitar Fret Noise", "Breath Noise", "Seashore", "Bird Tweet", "Telephone Ring", "Helicopter",
+            "Applause", "Gunshot"};
+
+    return (((unsigned int)n) < 128) ? names[n] : 0;
+}
+
+const char *MidiMessage::getGMInstrumentBankName(int n) throw()
+{
+    const char *names[] =
+        {
+            "Piano", "Chromatic Percussion", "Organ", "Guitar",
+            "Bass", "Strings", "Ensemble", "Brass",
+            "Reed", "Pipe", "Synth Lead", "Synth Pad",
+            "Synth Effects", "Ethnic", "Percussive", "Sound Effects"};
+
+    return (((unsigned int)n) <= 15) ? names[n] : 0;
+}
+
+const char *MidiMessage::getRhythmInstrumentName(int n) throw()
+{
+    const char *names[] =
+        {
+            "Acoustic Bass Drum", "Bass Drum 1", "Side Stick", "Acoustic Snare",
+            "Hand Clap", "Electric Snare", "Low Floor Tom", "Closed Hi-Hat", "High Floor Tom",
+            "Pedal Hi-Hat", "Low Tom", "Open Hi-Hat", "Low-Mid Tom", "Hi-Mid Tom", "Crash Cymbal 1",
+            "High Tom", "Ride Cymbal 1", "Chinese Cymbal", "Ride Bell", "Tambourine", "Splash Cymbal",
+            "Cowbell", "Crash Cymbal 2", "Vibraslap", "Ride Cymbal 2", "Hi Bongo", "Low Bongo",
+            "Mute Hi Conga", "Open Hi Conga", "Low Conga", "High Timbale", "Low Timbale", "High Agogo",
+            "Low Agogo", "Cabasa", "Maracas", "Short Whistle", "Long Whistle", "Short Guiro",
+            "Long Guiro", "Claves", "Hi Wood Block", "Low Wood Block", "Mute Cuica", "Open Cuica",
+            "Mute Triangle", "Open Triangle"};
+
+    return (n >= 35 && n <= 81) ? names[n - 35] : 0;
+}
+
+const char *MidiMessage::getControllerName(int n) throw()
+{
+    const char *names[] =
+        {
+            "Bank Select", "Modulation Wheel (coarse)", "Breath controller (coarse)",
+            0, "Foot Pedal (coarse)", "Portamento Time (coarse)",
+            "Data Entry (coarse)", "Volume (coarse)", "Balance (coarse)",
+            0, "Pan position (coarse)", "Expression (coarse)", "Effect Control 1 (coarse)",
+            "Effect Control 2 (coarse)", 0, 0, "General Purpose Slider 1", "General Purpose Slider 2",
+            "General Purpose Slider 3", "General Purpose Slider 4", 0, 0, 0, 0, 0, 0, 0, 0,
+            0, 0, 0, 0, "Bank Select (fine)", "Modulation Wheel (fine)", "Breath controller (fine)",
+            0, "Foot Pedal (fine)", "Portamento Time (fine)", "Data Entry (fine)", "Volume (fine)",
+            "Balance (fine)", 0, "Pan position (fine)", "Expression (fine)", "Effect Control 1 (fine)",
+            "Effect Control 2 (fine)", 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
+            "Hold Pedal (on/off)", "Portamento (on/off)", "Sustenuto Pedal (on/off)", "Soft Pedal (on/off)",
+            "Legato Pedal (on/off)", "Hold 2 Pedal (on/off)", "Sound Variation", "Sound Timbre",
+            "Sound Release Time", "Sound Attack Time", "Sound Brightness", "Sound Control 6",
+            "Sound Control 7", "Sound Control 8", "Sound Control 9", "Sound Control 10",
+            "General Purpose Button 1 (on/off)", "General Purpose Button 2 (on/off)",
+            "General Purpose Button 3 (on/off)", "General Purpose Button 4 (on/off)",
+            0, 0, 0, 0, 0, 0, 0, "Reverb Level", "Tremolo Level", "Chorus Level", "Celeste Level",
+            "Phaser Level", "Data Button increment", "Data Button decrement", "Non-registered Parameter (fine)",
+            "Non-registered Parameter (coarse)", "Registered Parameter (fine)", "Registered Parameter (coarse)",
+            0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, "All Sound Off", "All Controllers Off",
+            "Local Keyboard (on/off)", "All Notes Off", "Omni Mode Off", "Omni Mode On", "Mono Operation",
+            "Poly Operation"};
+
+    const char *ret = (((unsigned int)n) < 128) ? names[n] : "";
+    if (ret != 0)
+        return ret;
     else
-      return "";
+        return "";
 }
 
-bool MidiMessage::operator==(const MidiMessage &other) const throw() {
-  if(size != other.size)
-  {
-//    printf("MidiMessage::operator==() False (size)\n");
-    return false;
-  }
-  if(isNoteOff() && other.isNoteOff()) {
-    // avoid note-on / note-off confusion
-    return (getNoteNumber() == other.getNoteNumber());
-  } else {
-    for(int i=0; i < size; i++) {
-      if(data[i] != other.data[i]) {
-//        printf("MidiMessage::operator==() False (data %i: %i != %i)\n",
-//               i, data[i], other.data[i]);
+bool MidiMessage::operator==(const MidiMessage &other) const throw()
+{
+    if (size != other.size)
+    {
+        //    printf("MidiMessage::operator==() False (size)\n");
         return false;
-      }
     }
-  }
-//  printf("MidiMessage::operator==() True\n");
-  return true;
+    if (isNoteOff() && other.isNoteOff())
+    {
+        // avoid note-on / note-off confusion
+        return (getNoteNumber() == other.getNoteNumber());
+    }
+    else
+    {
+        for (int i = 0; i < size; i++)
+        {
+            if (data[i] != other.data[i])
+            {
+                //        printf("MidiMessage::operator==() False (data %i: %i != %i)\n",
+                //               i, data[i], other.data[i]);
+                return false;
+            }
+        }
+    }
+    //  printf("MidiMessage::operator==() True\n");
+    return true;
 }
```

### Comparing `rtmidi-2.3.4/cpp_src/rtmidimodule.cpp` & `rtmidi-2.5.0/src/rtmidimodule.cpp`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/cpp_src/pkglobals.h` & `rtmidi-2.5.0/src/pkglobals.h`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/cpp_src/PyMidiMessage.h` & `rtmidi-2.5.0/src/PyMidiMessage.h`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/setup_pkechomidi.py` & `rtmidi-2.5.0/setup_pkechomidi.py`

 * *Files identical despite different names*

### Comparing `rtmidi-2.3.4/setup.py` & `rtmidi-2.5.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,128 @@
-#   Copyright (C) 2018 by Patrick Stinson                                 
-#   patrickkidd@gmail.com                                                   
-#                                                                         
-#   This program is free software; you can redistribute it and/or modify  
-#   it under the terms of the GNU General Public License as published by  
-#   the Free Software Foundation; either version 2 of the License, or     
-#   (at your option) any later version.                                   
-#                                                                         
-#   This program is distributed in the hope that it will be useful,       
-#   but WITHOUT ANY WARRANTY; without even the implied warranty of        
-#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the         
-#   GNU General Public License for more details.                          
-#                                                                         
-#   You should have received a copy of the GNU General Public License     
-#   along with this program; if not, write to the                         
-#   Free Software Foundation, Inc.,                                       
-#   59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.  
-
+#!/bin/env python
+#   Copyright (C) 2023 by Patrick Stinson
+#   patrickkidd@gmail.com
+#
+#   This program is free software; you can redistribute it and/or modify
+#   it under the terms of the GNU General Public License as published by
+#   the Free Software Foundation; either version 2 of the License, or
+#   (at your option) any later version.
+#
+#   This program is distributed in the hope that it will be useful,
+#   but WITHOUT ANY WARRANTY; without even the implied warranty of
+#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#   GNU General Public License for more details.
+#
+#   You should have received a copy of the GNU General Public License
+#   along with this program; if not, write to the
+#   Free Software Foundation, Inc.,
+#   59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 
 import os, sys
-from distutils.core import setup, Extension
+from setuptools import setup, Extension
+
 
-if hasattr(os, 'uname'):
+if hasattr(os, "uname"):
     OSNAME = os.uname()[0]
 else:
-    OSNAME = 'Windows'
+    OSNAME = "Windows"
 
 
 define_macros = []
 libraries = []
 extra_link_args = []
 extra_compile_args = []
 library_dirs = []
 
 
-if OSNAME == 'Linux':
-    define_macros = [('__LINUX_ALSA__', '')]
-    libraries = ['asound', 'pthread']
-elif OSNAME == 'Darwin':
-    define_macros = [('__MACOSX_CORE__', '')]
-    libraries = ['pthread']
-    extra_compile_args = ['-Wno-missing-braces']
-    extra_link_args = ['-framework', 'CoreAudio',
-                       '-framework', 'CoreMidi',
-                       '-framework', 'CoreFoundation']
-elif OSNAME == 'Windows':
-    define_macros = [('__WINDOWS_MM__', ''),
-                     ('PK_WINDOWS', '1')]
-    library_dirs = ['C:\Program Files\Microsoft SDKs\Windows\v7.1\Lib']
-    libraries = ['winmm', 'python34']
-    extra_compile_args = ['/EHsc']
-elif OSNAME == 'Irix':
-    define_macros = [('__IRIX_MD__', '')]
-    libraries = ['pthread', 'md']
-
-if '--jack-midi' in sys.argv:
-    define_macros.append(('__UNIX_JACK__', ''))
-    libraries.append('jack')
-    sys.argv.pop(sys.argv.index('--jack-midi'))
-
-CPP_SRC_DIR = 'cpp_src'
-CPP_FNAMES = ['RtMidi.cpp',
-              'MidiMessage.cpp',
-              'PyMidiMessage.cpp',
-              'rtmidimodule.cpp',
-              ]
-
-CPP_HEADERS = ['RtMidi.h',
-               'pkglobals.h',
-               'MidiMessage.h',
-               'PyMidiMessage.h'
-               ]
-
-cpp_sources = [os.path.join(CPP_SRC_DIR, fname) for fname in CPP_FNAMES]
-cpp_headers = [os.path.join(CPP_SRC_DIR, fname) for fname in CPP_HEADERS]
-
-midi = Extension(name='rtmidi._rtmidi',
-                 sources=cpp_sources,
-                 headers=cpp_headers,
-                 library_dirs=library_dirs,
-                 libraries=libraries,
-                 define_macros=define_macros,
-                 extra_link_args=extra_link_args,
-                 extra_compile_args=extra_compile_args,
-                 )
-
-setup(name='rtmidi',
-      author='Patrick Stinson',
-      author_email='patrickkidd@gmail.com',
-      url='https://github.com/patrickkidd/pyrtmidi',
-      download_url='https://github.com/patrickkidd/pyrtmidi/tarball/2.3.4',
-      keywords=['midi audio hardware'],
-      version='2.3.4',
-      description = """Python RtMidi interface
+if OSNAME == "Linux":
+    define_macros = [("__LINUX_ALSA__", "")]
+    libraries = ["asound", "pthread"]
+elif OSNAME == "Darwin":
+    define_macros = [("__MACOSX_CORE__", "")]
+    libraries = ["pthread"]
+    extra_compile_args = ["-Wno-missing-braces", "-Wdeprecated-declarations"]
+    extra_link_args = [
+        "-framework",
+        "CoreAudio",
+        "-framework",
+        "CoreMidi",
+        "-framework",
+        "CoreFoundation",
+    ]
+elif OSNAME == "Windows":
+    define_macros = [("__WINDOWS_MM__", ""), ("PK_WINDOWS", "1")]
+    library_dirs = []
+    libraries = ["winmm"]
+    extra_compile_args = ["/EHsc"]
+elif OSNAME == "Irix":
+    define_macros = [("__IRIX_MD__", "")]
+    libraries = ["pthread", "md"]
+
+if "--jack-midi" in sys.argv:
+    define_macros.append(("__UNIX_JACK__", ""))
+    libraries.append("jack")
+    sys.argv.pop(sys.argv.index("--jack-midi"))
+
+
+setup(
+    name="rtmidi",
+    author="Patrick Stinson",
+    author_email="patrickkidd@gmail.com",
+    url="https://github.com/patrickkidd/pyrtmidi",
+    # download_url="https://github.com/patrickkidd/pyrtmidi/tarball/2.3.4",
+    keywords=["midi audio hardware"],
+    version="2.5.0",
+    description="Realtime MIDI I/O for Python on Windows, OS X, and Linux",
+    description_content_type="text/plain",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    ext_modules=[
+        Extension(
+            name="rtmidi._rtmidi",
+            sources=[
+                os.path.join("src", fname)
+                for fname in [
+                    "RtMidi.cpp",
+                    "MidiMessage.cpp",
+                    "PyMidiMessage.cpp",
+                    "rtmidimodule.cpp",
+                ]
+            ],
+            headers=[
+                os.path.join("src", fname)
+                for fname in [
+                    "RtMidi.h",
+                    "pkglobals.h",
+                    "MidiMessage.h",
+                    "PyMidiMessage.h",
+                ]
+            ],
+            library_dirs=library_dirs,
+            libraries=libraries,
+            define_macros=define_macros,
+            extra_link_args=extra_link_args,
+            extra_compile_args=extra_compile_args,
+        )
+    ],
+    packages=["rtmidi"],
+    scripts=["pkechomidi.py"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.11",
+    ],
+)
+
+
+DESCRIPTION = """
+Python RtMidi interface
+```
 def print_message(midi):
     if midi.isNoteOn():
         print 'ON: ', midi.getMidiNoteName(midi.getNoteNumber()), midi.getVelocity()
     elif midi.isNoteOff():
         print 'OFF:', midi.getMidiNoteName(midi.getNoteNumber())
     elif midi.isController():
         print 'CONTROLLER', midi.getControllerNumber(), midi.getControllerValue()
@@ -112,17 +138,9 @@
     midiin.openPort(1)
     while True:
         m = midiin.getMessage(250) # some timeout in ms
         if m != None:
             print_message(m)
 else:
     print 'NO MIDI INPUT PORTS!'
-""",
-      ext_modules=[midi],
-      packages=['rtmidi'],
-      scripts=['pkechomidi.py'],
-      classifiers=['Development Status :: 5 - Production/Stable',
-                   'Intended Audience :: Developers',
-                   'Programming Language :: Python :: 3',
-                   'Programming Language :: Python :: 3.4',
-                   ]
-      )
+```
+"""
```


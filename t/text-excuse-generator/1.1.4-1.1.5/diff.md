# Comparing `tmp/text_excuse_generator-1.1.4.tar.gz` & `tmp/text_excuse_generator-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.1.4.tar", last modified: Mon Apr 10 07:44:12 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.5.tar", last modified: Tue May  2 05:31:08 2023, max compression
```

## Comparing `text_excuse_generator-1.1.4.tar` & `text_excuse_generator-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:44:12.777505 text_excuse_generator-1.1.4/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.4/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:44:12.777267 text_excuse_generator-1.1.4/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-10 07:44:12.777576 text_excuse_generator-1.1.4/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)      986 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:44:12.776367 text_excuse_generator-1.1.4/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.4/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)    10312 2023-04-10 07:37:07.000000 text_excuse_generator-1.1.4/text_excuse_generator/excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-10 07:44:12.776984 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    12286 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      316 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-04-10 07:44:12.000000 text_excuse_generator-1.1.4/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:31:08.074087 text_excuse_generator-1.1.5/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.5/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12367 2023-05-02 05:31:08.073909 text_excuse_generator-1.1.5/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-05-02 05:31:08.074141 text_excuse_generator-1.1.5/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)     1089 2023-05-02 05:31:07.000000 text_excuse_generator-1.1.5/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:31:08.072842 text_excuse_generator-1.1.5/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.5/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    12322 2023-05-02 05:19:07.000000 text_excuse_generator-1.1.5/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:31:08.073685 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12367 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.1.4/LICENSE` & `text_excuse_generator-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.4/PKG-INFO` & `text_excuse_generator-1.1.5/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: text_excuse_generator
-Version: 1.1.4
+Name: text-excuse-generator
+Version: 1.1.5
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
+Home-page: https://github.com/Huckdirks/text-excuse-generator
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Text Excuse Generator
@@ -62,37 +63,37 @@
 
 You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 #### **Sending a Text Message**
 
 If you want to send a text with command line arguments, run:
 ```bash
-python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]
+python3 text_excuse_generator.py SENDER RECIPIENT PROBLEM EXCUSE [--send_text_flag]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py Me "Your mom" "I'm late to 😈" "Too many wizards around" -s
 ```
 Omit the `[--send_text_flag]` if you don't want to send the text message.
 
 #### **Setting Up .env File**
 If you want to set up the .env file, run:
 ```bash
-python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]
+python3 text_excuse_generator.py -e/--setup_env TWILIO_ACCOUNT_SID TWILIO_AUTH_TOKEN TWILIO_PHONE_NUMBER [OPENAI_API_KEY]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py -e "AC1234567890" "1234567890" "+15555555555" "sk-1234567890"
 ```
 
 #### **Saving a New Recipient**
 
 If you want to save a new recipient to the system, run:
 ```bash
-python3 text_excuse_generator.py [-a/--add] [NAME] [PHONE_NUMBER]
+python3 text_excuse_generator.py -a/--add NAME PHONE_NUMBER
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py -a "Your mom" +15555555555
 ```
 
 ### Importing as a Module
@@ -109,17 +110,17 @@
 ```python
 from text_excuse_generator.excuse_generator import *
 ```
 Or you can import the individual functions.
 
 #### `generate_excuse()` takes in:
 ```python
-generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> str
+generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> (str | None)
 ```
-`generate_excuse()` returns a string of the text message that was generated.
+`generate_excuse()` returns a string of the text message that was generated, or None if unable to generate the text message.
 
 If you want to generate a text message, call the function like this:
 
 ```python
 generate_excuse("user", "recipient", "problem", "excuse", True)
 ```
 e.g.
@@ -188,15 +189,15 @@
 - OpenAI API Key
 
 And then [set up the `.env` file](#setting-up-env-file-1) with this information.
 #### Install
 
 ##### For Command Line Use
 
-Double click [`dependencies`](../dependencies), or run `bash `[`dependencies`](../dependencies) or `./`[`dependencies`](../dependencies) in the root directory or to install the python dependencies. You must have [pip](https://pip.pypa.io/en/stable/installation/) installed to download the new dependencies. Also, you'll need to install [python](https://www.python.org/downloads/) yourself if you haven't already.
+Double click [`dependencies`](../dependencies), or run `bash `[`dependencies`](../dependencies) or `./`[`dependencies`](../dependencies) in the root directory to install the python dependencies. You must have [pip](https://pip.pypa.io/en/stable/installation/) installed to download the new dependencies. Also, you'll need to install [python](https://www.python.org/downloads/) yourself if you haven't already.
 
 ##### For Importing as a Module
 
 If you just run:
 ```bash
 pip install text-excuse-generator
 ```
@@ -208,15 +209,15 @@
 
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`setup_env()`](#setup_env-takes-in) function in the `text_excuse_generator` module.
 
 ### Running
 
 **YOU HAVE TO INSTALL THE DEPENDENCIES & SETUP THE `.env` FILE BEFORE TRYING TO RUN THE PROGRAM!!!**
 
-Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]` in the command line in the source directory.
+Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py SENDER RECIPIENT PROBLEM EXCUSE [--send_text_flag]` in the command line in the source directory.
 
 More detailed instructions are in the [Uses](#uses) section.
 
 ## Quality Assurance
 All variable, function, class, module, & file names are written in [snake_case](https://en.wikipedia.org/wiki/Snake_case) to make sure everything is consistent, and all `const` variables are written in ALL-CAPS. The code is also quite commented and the variable names are quite verbose, so it should be easy enough to understand what's going on.
 
 If there are any other/better ways to check for quality assurance, please let me know in the [suggestions](https://github.com/Huckdirks/Excuse_Text_Generator/discussions/new?category=suggestions)!
```

### Comparing `text_excuse_generator-1.1.4/setup.py` & `text_excuse_generator-1.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-	version = '1.1.4',
+	version = "1.1.5",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
+    url = "https://github.com/Huckdirks/text-excuse-generator",
     packages = find_packages(),
     install_requires = ["python-dotenv", "twilio", "openai", "phonenumbers"],
     keywords = ["text excuse generator", "openai", "twilio", "text message", "GPT-3.5"],
     classifiers = [
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires = ">=3.8"
+    python_requires = ">=3.8",
+    py_modules = ["text_excuse_generator"]
 )
```

### Comparing `text_excuse_generator-1.1.4/text_excuse_generator/excuse_generator.py` & `text_excuse_generator-1.1.5/text_excuse_generator/excuse_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Imported Libraries
 from dotenv import load_dotenv
 import openai   # I would just import the necessary functions, but api_key is too generic of a name, so I'm gonna keep the OpenAI namespace
 import twilio.rest
 from phonenumbers import is_valid_number, parse
 
 # Python Libraries
-from os import getenv
+from os import getenv, system
 from os.path import dirname, join, isfile
 from sys import argv
 
 # Constants
-ENV_NAME = "personal_info.env"  # CHANGE THIS TO YOUR ENVIRONMENT NAME (.env file)
+ENV_NAME = ".env"  # CHANGE THIS TO YOUR ENVIRONMENT NAME (.env file)
 ENV_PATH = join(dirname(__file__), ENV_NAME)
 
 
 # Set up .env file
 def setup_env(TWILIO_ACCOUNT_SID: str, TWILIO_AUTH_TOKEN: str, TWILIO_PHONE_NUMBER: str, OPENAI_API_KEY: str) -> bool:
     # Check if .env file exists and not empty
     if isfile(ENV_PATH):
@@ -67,15 +67,15 @@
 # If the -s or --send flag is given, send the text
 def send_twilio_text(TO_PHONE_NUMBER: str, MESSAGE: str) -> None:
     if not isfile(ENV_PATH):
         print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
         return
     
     # Load the .env file
-    load_dotenv(ENV_PATH)
+    load_dotenv()
 
     print("Sending text...")
     # Twilio API
     twilio_client = twilio.rest.Client(getenv("TWILIO_ACCOUNT_SID"), getenv("TWILIO_AUTH_TOKEN"))  # Login to Twilio
     twilio_client.messages.create(
         to = TO_PHONE_NUMBER,
         from_ = getenv("TWILIO_PHONE_NUMBER"),
@@ -83,16 +83,16 @@
     )
     
     print("Text sent!")
     return
 
 
 # Generate an excuse and text it to a recipient. If no parameters are given, either by being passed in or given via the Command Line, it will prompt the user for input
-def generate_excuse(**kwargs) -> str:
-    if kwargs:  # If parameters are passed in
+def generate_excuse(**kwargs) -> (str | None):
+    if kwargs and ("user" in kwargs and "recipient" in kwargs and "problem" in kwargs and "excuse" in kwargs):  # If parameters are passed in
         USER = kwargs["user"]
         RECIPIENT = kwargs["recipient"]
         PROBLEM = kwargs["problem"]
         EXCUSE = kwargs["excuse"]
         if "send_text" in kwargs:
             SEND_TEXT = kwargs["send_text"]
         if not USER or not RECIPIENT or not PROBLEM or not EXCUSE:
@@ -114,15 +114,15 @@
         EXCUSE = argv[4]
         if len(argv) == 6 and (argv[5].lower() == "-s" or argv[5].lower() == "--send"):
             SEND_TEXT = True
         elif len(argv) == 6:
             print("\nError: Invalid flag given! Use -s or --send to send the text")
             return
 
-    elif len(argv) == 1:    # If no arguments are given, ask for user input
+    elif len(argv) == 1 and not kwargs:    # If no arguments are given, ask for user input
         if not isfile(ENV_PATH):  # If the .env file is not set up, ask the user if they want to set it up
             set_up_env_question = input(f"Error: \'{ENV_NAME}\' file not set up!\nDo you want to set it up now? (y/n): ")
             if set_up_env_question.lower() == "y" or set_up_env_question.lower() == "yes":
                 TWILIO_ACCOUNT_SID = input("Enter your Twilio Account SID: ")
                 TWILIO_AUTH_TOKEN = input("Enter your Twilio Auth Token: ")
                 TWILIO_PHONE_NUMBER = input("Enter your Twilio Phone Number: ")
                 OPENAI_API_KEY = input("Enter your OpenAI API Key: ")
@@ -137,36 +137,56 @@
         PROBLEM = input("Enter the fake problem you are having: ")
         EXCUSE = input("Enter the excuse you want to use: ")
 
         send_text_question = input("Do you want to send the text? (y/n): ")
         if send_text_question.lower() == "y" or send_text_question.lower() == "yes":
             SEND_TEXT = True
 
-    else:   # Give info on how to use the program if the wrong # of parameters are given
-        print("\nUsage: python3 text_excuse_generator.py [SENDER] [SENDER] [SENDER] [SENDER] [--send_flag]")
+    else:
+        # Give info on how to use the program if the wrong # of parameters are given
+        system("clear")
+        print("\nExcuse Generator Help:")
+        print("\nThis program generates an excuse for you to send to someone. It uses the OpenAI API to generate the excuse, and the Twilio API to send the text.")
+        print("\nThe program can be called in one of two ways:")
+        print("\t1. From the command line (arguments are optional)")
+        print("\tUsage: python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_flag]\n\te.g. python3 text_excuse_generator.py \"John Doe\" \"Jane Doe\" \"Gonna miss dinner\" \"I'm sick\" -s")
+        print("\n\t2. As parameters in a function call")
+        print("\tUsage: generate_excuse(user = \"USER\", recipient = \"RECIPIENT\", problem = \"INSERT PROBLEM HERE\", excuse = \"INSERT EXCUSE HERE\", send_text = BOOL)\n\te.g. generate_excuse(user = \"John Doe\", recipient = \"Jane Doe\", problem = \"Gonna miss dinner\", excuse = \"I'm sick\", send_text = True)")
+        print("\nThis function takes 4 required parameters and 1 optional parameter:")
         print("\tsender: The person who is sending the text")
         print("\trecipient: The person you want to text (can be saved person or a phone number)")
         print("\tproblem: The \"problem\" you are having")
         print("\texcuse: The excuse you want to use")
         print("\t--send_flag: If you want to send the text, add -s or --send. If you don't want to send the text, omit this flag\n")
         print("Or just run the program with no arguments to be prompted for input")
         print("Put any parameters longer than a single word in quotes, e.g. \"I'm sick\"\n")
-        print("To add a new recipient to the .env file, run python3 text_excuse_generator.py [-a/--add] [RECIPIENT] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"\n")
-        print("To setup the .env file, run python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]\n\te.g. python3 text_excuse_generator.py -e \"AC1234567890abcdef1234567890abcdef\" \"1234567890abcdef1234567890abcdef\" \"+15555555555\" \"1234567890abcdef1234567890abcdef\"\n")
-        print("The prompt sent to ChatGPT is: \"Write a text message to [RECIPIENT] explaining that you [PROBLEM] because [EXCUSE]. Also start the message by stating this is [USER], and end the message by telling the recipient to text my actual phone number back if you really need me.\"\n")
+        print("\nYou can also add new recipients to the .env file in one of two ways:")
+        print("\t1. As command line arguments")
+        print("\tUsage: python3 text_excuse_generator.py [-a/--add] [RECIPIENT] [PHONE_NUMBER]\n\te.g. python3 text_excuse_generator.py -a \"John Doe\" \"+15555555555\"")
+        print("\n\t2. As parameters in a function call")
+        print("\tUsage: add_recipient(\"RECIPIENT\", \"PHONE_NUMBER\")\n\te.g. add_recipient(\"John Doe\", \"+15555555555\")")
+        print("\nThis function takes 2 required parameters:")
+        print("\trecipient: The person you want to text (can be saved person or a phone number)")
+        print("\tphone_number: The phone number you want to text the recipient at")
+        print("\nYou can also set up the .env file in one of two ways:")
+        print("\t1. As command line arguments")
+        print("\tUsage: python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]\n\te.g. python3 text_excuse_generator.py -e \"AC1234567890abcdef1234567890abcdef\" \"1234567890abcdef1234567890abcdef\" \"+15555555555\" \"sk-1234567890abcdef1234567890abcdef\"")
+        print("\n\t2. As parameters in a function call")
+        print("\tUsage: setup_env(\"TWILIO_ACCOUNT_SID\", \"TWILIO_AUTH_TOKEN\", \"TWILIO_PHONE_NUMBER\", \"OPENAI_API_KEY\")\n\te.g. setup_env(\"AC1234567890abcdef1234567890abcdef\", \"1234567890abcdef1234567890abcdef\", \"+15555555555\", \"sk-1234567890abcdef1234567890abcdef\")")
+        print("\nThe prompt sent to ChatGPT is: \"Write a text message to [RECIPIENT] explaining that you [PROBLEM] because [EXCUSE]. Also start the message by stating this is [USER], and end the message by telling the recipient to text my actual phone number back if you really need me.\"\n")
         return
         
 
     # If the .env file is not set up, or is empty, return   
     if not isfile(ENV_PATH):
         print(f"Error: \'{ENV_NAME}\' file not set up! Use the -e or --setup_env flag to set up the .env file")
         return
     
     # Load the .env file
-    load_dotenv(ENV_PATH)
+    load_dotenv()
 
     to_phone_number = ""
     if (RECIPIENT[0] == '+' and RECIPIENT[1:].isnumeric()) and is_valid_number(parse(RECIPIENT)):   # Check if RECIPIENT is a phone number
         to_phone_number = RECIPIENT
     elif SEND_TEXT:
         RECIPIENT_FORMATTED = RECIPIENT.replace(" ", "_")
         to_phone_number = getenv(f"{RECIPIENT_FORMATTED.upper()}_PHONE_NUMBER")
```

### Comparing `text_excuse_generator-1.1.4/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: text-excuse-generator
-Version: 1.1.4
+Name: text_excuse_generator
+Version: 1.1.5
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
+Home-page: https://github.com/Huckdirks/text-excuse-generator
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Text Excuse Generator
@@ -62,37 +63,37 @@
 
 You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend just downloading [excuse_generator.py](../text_excuse_generator/excuse_generator.py) and running it from the command line. If you just want the [excuse_generator.py](../text_excuse_generator/excuse_generator.py) file for a project, please also include the [LICENSE](../LICENSE) file in the same directory as [excuse_generator.py](../text_excuse_generator/excuse_generator.py).
 
 #### **Sending a Text Message**
 
 If you want to send a text with command line arguments, run:
 ```bash
-python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]
+python3 text_excuse_generator.py SENDER RECIPIENT PROBLEM EXCUSE [--send_text_flag]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py Me "Your mom" "I'm late to 😈" "Too many wizards around" -s
 ```
 Omit the `[--send_text_flag]` if you don't want to send the text message.
 
 #### **Setting Up .env File**
 If you want to set up the .env file, run:
 ```bash
-python3 text_excuse_generator.py [-e/--setup_env] [TWILIO_ACCOUNT_SID] [TWILIO_AUTH_TOKEN] [TWILIO_PHONE_NUMBER] [OPENAI_API_KEY]
+python3 text_excuse_generator.py -e/--setup_env TWILIO_ACCOUNT_SID TWILIO_AUTH_TOKEN TWILIO_PHONE_NUMBER [OPENAI_API_KEY]
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py -e "AC1234567890" "1234567890" "+15555555555" "sk-1234567890"
 ```
 
 #### **Saving a New Recipient**
 
 If you want to save a new recipient to the system, run:
 ```bash
-python3 text_excuse_generator.py [-a/--add] [NAME] [PHONE_NUMBER]
+python3 text_excuse_generator.py -a/--add NAME PHONE_NUMBER
 ```
 e.g.
 ```bash
 python3 text_excuse_generator.py -a "Your mom" +15555555555
 ```
 
 ### Importing as a Module
@@ -109,17 +110,17 @@
 ```python
 from text_excuse_generator.excuse_generator import *
 ```
 Or you can import the individual functions.
 
 #### `generate_excuse()` takes in:
 ```python
-generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> str
+generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> (str | None)
 ```
-`generate_excuse()` returns a string of the text message that was generated.
+`generate_excuse()` returns a string of the text message that was generated, or None if unable to generate the text message.
 
 If you want to generate a text message, call the function like this:
 
 ```python
 generate_excuse("user", "recipient", "problem", "excuse", True)
 ```
 e.g.
@@ -188,15 +189,15 @@
 - OpenAI API Key
 
 And then [set up the `.env` file](#setting-up-env-file-1) with this information.
 #### Install
 
 ##### For Command Line Use
 
-Double click [`dependencies`](../dependencies), or run `bash `[`dependencies`](../dependencies) or `./`[`dependencies`](../dependencies) in the root directory or to install the python dependencies. You must have [pip](https://pip.pypa.io/en/stable/installation/) installed to download the new dependencies. Also, you'll need to install [python](https://www.python.org/downloads/) yourself if you haven't already.
+Double click [`dependencies`](../dependencies), or run `bash `[`dependencies`](../dependencies) or `./`[`dependencies`](../dependencies) in the root directory to install the python dependencies. You must have [pip](https://pip.pypa.io/en/stable/installation/) installed to download the new dependencies. Also, you'll need to install [python](https://www.python.org/downloads/) yourself if you haven't already.
 
 ##### For Importing as a Module
 
 If you just run:
 ```bash
 pip install text-excuse-generator
 ```
@@ -208,15 +209,15 @@
 
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`setup_env()`](#setup_env-takes-in) function in the `text_excuse_generator` module.
 
 ### Running
 
 **YOU HAVE TO INSTALL THE DEPENDENCIES & SETUP THE `.env` FILE BEFORE TRYING TO RUN THE PROGRAM!!!**
 
-Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [SENDER] [RECIPIENT] [PROBLEM] [EXCUSE] [--send_text_flag]` in the command line in the source directory.
+Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py SENDER RECIPIENT PROBLEM EXCUSE [--send_text_flag]` in the command line in the source directory.
 
 More detailed instructions are in the [Uses](#uses) section.
 
 ## Quality Assurance
 All variable, function, class, module, & file names are written in [snake_case](https://en.wikipedia.org/wiki/Snake_case) to make sure everything is consistent, and all `const` variables are written in ALL-CAPS. The code is also quite commented and the variable names are quite verbose, so it should be easy enough to understand what's going on.
 
 If there are any other/better ways to check for quality assurance, please let me know in the [suggestions](https://github.com/Huckdirks/Excuse_Text_Generator/discussions/new?category=suggestions)!
```


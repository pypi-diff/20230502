# Comparing `tmp/gimme aws creds-2.5.0.tar.gz` & `tmp/gimme aws creds-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme aws creds-2.5.0.tar", last modified: Thu Jan  5 15:54:17 2023, max compression
+gzip compressed data, was "gimme aws creds-2.6.0.tar", last modified: Tue May  2 15:51:58 2023, max compression
```

## Comparing `gimme aws creds-2.5.0.tar` & `gimme aws creds-2.6.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 15:54:17.712370 gimme aws creds-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-05 15:54:17.712370 gimme aws creds-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 15:54:17.712370 gimme aws creds-2.5.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/bin/gimme-aws-creds
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/bin/gimme-aws-creds.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 15:54:17.712370 gimme aws creds-2.5.0/gimme_aws_creds/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26380 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/duo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    36787 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    47339 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/okta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/registered_authenticators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/gimme_aws_creds/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 15:54:17.712370 gimme aws creds-2.5.0/gimme_aws_creds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-05 15:54:17.000000 gimme aws creds-2.5.0/gimme_aws_creds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-05 15:54:17.000000 gimme aws creds-2.5.0/gimme_aws_creds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 15:54:17.000000 gimme aws creds-2.5.0/gimme_aws_creds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-05 15:54:17.000000 gimme aws creds-2.5.0/gimme_aws_creds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-05 15:54:17.000000 gimme aws creds-2.5.0/gimme_aws_creds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-05 15:54:17.712370 gimme aws creds-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-05 15:54:05.000000 gimme aws creds-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/bin/gimme-aws-creds
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/bin/gimme-aws-creds-autocomplete.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/bin/gimme-aws-creds.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/gimme_aws_creds/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26779 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47402 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/okta_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/okta_identity_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/registered_authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/gimme_aws_creds/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:58.810083 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 15:51:58.000000 gimme aws creds-2.6.0/gimme_aws_creds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 15:51:58.814083 gimme aws creds-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-02 15:51:48.000000 gimme aws creds-2.6.0/setup.py
```

### Comparing `gimme aws creds-2.5.0/LICENSE` & `gimme aws creds-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/NOTICE` & `gimme aws creds-2.6.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/README.md` & `gimme aws creds-2.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Gimme AWS Creds
 
 [![][license img]][license]
-[![Build Status](https://travis-ci.org/Nike-Inc/gimme-aws-creds.svg?branch=master)](https://travis-ci.org/Nike-Inc/gimme-aws-creds)
+[![][cicd img]][cicd]
 
 gimme-aws-creds is a CLI that utilizes an [Okta](https://www.okta.com/) IdP via SAML to acquire temporary AWS credentials via AWS STS.
 
 Okta is a SAML identity provider (IdP), that can be easily set-up to do SSO to your AWS console. Okta does offer an [OSS java CLI]((https://github.com/oktadeveloper/okta-aws-cli-assume-role)) tool to obtain temporary AWS credentials, but I found it needs more information than the average Okta user would have and doesn't scale well if have more than one Okta App.
 
 With gimme-aws-creds all you need to know is your username, password, Okta url and MFA token, if MFA is enabled. gimme-aws-creds gives you the option to select which Okta AWS application and role you want credentials for. Alternatively, you can pre-configure the app and role name by passing -c or editing the config file. This is all covered in the usage section.
 
+## Disclaimer
+Okta is a registered trademark of Okta, Inc. and this tool has no affiliation with or sponsorship by Okta, Inc.
+
 ## Prerequisites
 
 [Okta SAML integration to AWS using the AWS App](https://help.okta.com/en/prod/Content/Topics/Miscellaneous/References/OktaAWSMulti-AccountConfigurationGuide.pdf)
 
-Python 3.6+
+Python 3.7+
 
 ### Optional
 
 [Gimme-creds-lambda](https://github.com/Nike-Inc/gimme-aws-creds/tree/master/lambda) can be used as a proxy to the Okta APIs needed by gimme-aws-creds.  This removes the requirement of an Okta API key.  Gimme-aws-creds authenticates to gimme-creds-lambda using OpenID Connect and the lambda handles all interactions with the Okta APIs.  Alternately, you can set the `OKTA_API_KEY` environment variable and the `gimme_creds_server` configuration value to 'internal' to call the Okta APIs directly from gimme-aws-creds.
 
 ## Installation
 
@@ -130,34 +133,64 @@
   -v ~/.aws/credentials:/root/.aws/credentials \
   -v ~/.okta_aws_login_config:/root/.okta_aws_login_config \
   gimme-aws-creds"
 ```
 
 With this config, you will be able to run further commands seamlessly!
 
+## Command Auto Completion
+
+If you are using Bash or Zsh, you can add autocompletion for the gimme-aws-creds commandline options and profile names.  To add the autocomplete config, add the following to the end of your .bashrc or .zshrc:
+
+.bashrc
+```bash
+INSTALL_DIR=$(dirname $(which gimme-aws-creds))
+source ${INSTALL_DIR}/gimme-aws-creds-autocomplete.sh"
+```
+
+.zshrc
+```bash
+INSTALL_DIR=$(dirname $(which gimme-aws-creds))
+autoload bashcompinit
+bashcompinit
+source ${INSTALL_DIR}/gimme-aws-creds-autocomplete.sh
+```
+
+## Using gimme-aws-creds with Okta Identity Engine
+
+To use gimme-aws-creds with an Okta Identity Engine (OIE) domain, you must create a new OIDC Native Application and connect it to your AWS integration app(s).
+
+The OIDC Native Application requires Grant Types `Authorization Code`, `Device Authorization` , and `Token Exchange`. These settings are in the Okta Admin UI at `Applications > [the OIDC app] > General Settings > Grant type`.
+
+The pairing with the AWS Federation Application is achieved in the Fed app's Sign On Settings. These settings are in the Okta Admin UI at `Applications > [the AWS Fed app] > Sign On`. Make sure to set the `Allowed Web SSO Client` value to the Client ID of the OIDC Native Application. Repeat that setting for each AWS application you want to access with gimme-aws-creds.
+
+Finally, set the Client ID in gimme-aws-creds (`gimme-aws-creds --action-configure` or update the `client_id` parameter in your config file)
+
+**When using gimme-aws-creds with an OIE domain, you will authenticate using your browser.  Storing credentials in keychain or passing MFA codes through the command-line is NOT POSSIBLE.**
+
 ## Configuration
 
 To set-up the configuration run:
 
 ```bash
 gimme-aws-creds --action-configure
 ```
 
-You can also set up different Okta configuration profiles, this useful if you have multiple Okta accounts or environments you need credentials for. You can use the configuration wizard or run:
+You can also set up different Okta configuration profiles, this is useful if you have multiple Okta accounts or environments you need credentials for. You can use the configuration wizard or run:
 
 ```bash
 gimme-aws-creds --action-configure --profile profileName
 ```
 
 A configuration wizard will prompt you to enter the necessary configuration parameters for the tool to run, the only one that is required is the `okta_org_url`. The configuration file is written to `~/.okta_aws_login_config`, but you can change the location with the environment variable `OKTA_CONFIG`.
 
 - conf_profile - This sets the Okta configuration profile name, the default is DEFAULT.
 - okta_org_url - This is your Okta organization url, which is typically something like `https://companyname.okta.com`.
 - okta_auth_server - [Okta API Authorization Server](https://help.okta.com/en/prev/Content/Topics/Security/API_Access.htm) used for OpenID Connect authentication for gimme-creds-lambda
-- client_id - OAuth client ID for gimme-creds-lambda
+- client_id - OAuth client ID for user authentication in Okta Identity Engine and gimme-creds-lambda in Okta "classic"
 - gimme_creds_server
   - URL for gimme-creds-lambda
   - 'internal' for direct interaction with the Okta APIs (`OKTA_API_KEY` environment variable required)
   - 'appurl' to set an aws application link url. This setting removes the need of an OKTA API key.
 - write_aws_creds - True or False - If True, the AWS credentials will be written to `~/.aws/credentials` otherwise it will be written to stdout.
 - cred_profile - If writing to the AWS cred file, this sets the name of the AWS credential profile.
   - The reserved word `role` will use the name component of the role arn as the profile name. i.e. arn:aws:iam::123456789012:role/okta-1234-role becomes section [okta-1234-role] in the aws credentials file
@@ -178,14 +211,15 @@
   - web - DUO uses localhost webbrowser to support push|call|passcode
   - passcode - DUO uses `OKTA_MFA_CODE` or `--mfa-code` if set, or prompts user for passcode(OTP).
   
 - resolve_aws_alias - y or n. If yes, gimme-aws-creds will try to resolve AWS account ids with respective alias names (default: n). This option can also be set interactively in the command line using `-r` or `--resolve` parameter
 - include_path - (optional) Includes full role path to the role name in AWS credential profile name. (default: n).  If `y`: `<acct>-/some/path/administrator`. If `n`: `<acct>-administrator`
 - remember_device - y or n. If yes, the MFA device will be remembered by Okta service for a limited time. This option can also be set interactively in the command line using `-m` or `--remember-device`
 - output_format - `json` , `export` or `windows`, determines default credential output format, can be also specified by `--output-format FORMAT` and `-o FORMAT`.
+- open-browser - Open the device authentication link in the default web browser automatically (Okta Identity Engine domains only)
 
 ## Configuration File
 
 The config file follows a [configfile](https://docs.python.org/3/library/configparser.html) format.
 By default, it is located in $HOME/.okta_aws_login_config
 
 Example file:
@@ -272,14 +306,18 @@
 
 `gimme-aws-creds --action-list-profiles` will go to your okta config file and print out all profiles created and their settings.
 
 ### Viewing roles
 
 `gimme-aws-creds --action-list-roles` will print all available roles to STDOUT without retrieving their credentials.
 
+### Credential expiration time
+
+Writing to the AWS credentials file will include the `x_security_token_expires` value in RFC3339 format. This allows tools to validate if the credentials are expiring or are expiring soon and warn the user or trigger a refresh.
+
 ### Generate credentials as json
 
 `gimme-aws-creds -o json` will print out credentials in JSON format - 1 entry per line
 
 ### Store credentials from json
 
 `gimme-aws-creds --action-store-json-creds` will store JSON formatted credentials from `stdin` to
@@ -342,35 +380,39 @@
 gimme-aws-creds --action-setup-fido-authenticator
 ```
 
 Then, you can choose the newly registered authenticator from the factors list.
 
 ## Running Tests
 
-You can run all the unit tests using nosetests. Most of the tests are mocked.
+You can run all the unit tests using pytest. Most of the tests are mocked.
 
 ```bash
-nosetests --verbosity=2 tests/
+pytest -vv tests
 ```
 
 ## Maintenance
 
-This project is maintained by [Ann Wallace](https://github.com/anners), [Eric Pierce](https://github.com/epierce), and [Justin Wiley](https://github.com/sector95).
+This project is maintained by [Eric Pierce](https://github.com/epierce)
 
 ## Thanks and Credit
 
 I came across [okta_aws_login](https://github.com/nimbusscale/okta_aws_login) written by Joe Keegan, when I was searching for a CLI tool that generates AWS tokens via Okta. Unfortunately it hasn't been updated since 2015 and didn't seem to work with the current Okta version. But there was still some great code I was able to reuse under the MIT license for gimme-aws-creds. I have noted in the comments where I used his code, to make sure he receives proper credit.
 
 ## Etc
 
-[Okta's Java tool](https://github.com/oktadeveloper/okta-aws-cli-assume-role)
+[okta-aws-cli](https://github.com/okta/okta-aws-cli)
+
+[okta-aws-cli-assume-role](https://github.com/oktadev/okta-aws-cli-assume-role)
 
 [AWS - How to Implement Federated API and CLI Access Using SAML 2.0 and AD FS](https://aws.amazon.com/blogs/security/how-to-implement-federated-api-and-cli-access-using-saml-2-0-and-ad-fs/)
 
 ## [Contributing](https://github.com/Nike-Inc/gimme-aws-creds/blob/master/CONTRIBUTING.md)
 
 ## License
 
 Gimme AWS Creds is released under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
 
 [license]:LICENSE
 [license img]:https://img.shields.io/badge/License-Apache%202-blue.svg
+[cicd]:https://github.com/Nike-Inc/gimme-aws-creds/actions/workflows/cicd.yml
+[cicd img]:https://github.com/Nike-Inc/gimme-aws-creds/actions/workflows/cicd.yml/badge.svg
```

### Comparing `gimme aws creds-2.5.0/bin/gimme-aws-creds` & `gimme aws creds-2.6.0/bin/gimme-aws-creds`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/bin/gimme-aws-creds.cmd` & `gimme aws creds-2.6.0/bin/gimme-aws-creds.cmd`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/aws.py` & `gimme aws creds-2.6.0/gimme_aws_creds/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         if verify_ssl_certs is False:
             requests.packages.urllib3.disable_warnings()
 
         # Allow up to 5 retries on requests to AWS in case we have network issues
         self._http_client = requests.Session()
         retries = Retry(total=5, backoff_factor=1,
-                        method_whitelist=['POST'])
+                        allowed_methods=['POST'])
         self._http_client.mount('https://', HTTPAdapter(max_retries=retries))
 
     def get_signinpage(self, saml_token, saml_target_url):
         """ Post SAML token to aws sign in page and get back html result"""
         payload = {
             'SAMLResponse': saml_token,
             'RelayState': ''
```

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/common.py` & `gimme aws creds-2.6.0/gimme_aws_creds/common.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/config.py` & `gimme aws creds-2.6.0/gimme_aws_creds/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         """
         self.ui = gac_ui
         self.FILE_ROOT = self.ui.HOME
         self.OKTA_CONFIG = self.ui.environ.get(
             'OKTA_CONFIG',
             os.path.join(self.FILE_ROOT, '.okta_aws_login_config')
         )
+        self.open_browser = False
         self.action_register_device = False
         self.username = None
         self.api_key = None
         self.conf_profile = 'DEFAULT'
         self.verify_ssl_certs = True
         self.app_url = None
         self.resolve = False
@@ -141,22 +142,27 @@
         parser.add_argument(
             '--action-store-json-creds', action='store_true',
             help='Read credentials from stdin (in json format) and store them in ~/.aws/credentials file')
         parser.add_argument(
             '--action-setup-fido-authenticator', action='store_true',
             help='Sets up a new FIDO WebAuthn authenticator in Okta'
         )
+        parser.add_argument(
+            '--open-browser', action='store_true',
+            help='Automatically open a webbrowser for device authorization (Okta Identity Engine only)'
+        )
         args = parser.parse_args(self.ui.args)
 
         self.action_configure = args.action_configure
         self.action_list_profiles = args.action_list_profiles
         self.action_list_roles = args.action_list_roles
         self.action_store_json_creds = args.action_store_json_creds
         self.action_register_device = args.action_register_device
         self.action_setup_fido_authenticator = args.action_setup_fido_authenticator
+        self.open_browser = args.open_browser
 
         if args.insecure is True:
             ui.default.warning("Warning: SSL certificate validation is disabled!")
             self.verify_ssl_certs = False
         else:
             self.verify_ssl_certs = True
 
@@ -211,15 +217,15 @@
     def update_config_file(self):
         """
            Prompts user for config details for the okta_aws_login tool.
            Either updates existing config file or creates new one.
            Config Options:
                 okta_org_url = Okta URL
                 gimme_creds_server = URL of the gimme-creds-server or 'internal' for local processing or 'appurl' when app url available
-                client_id = OAuth Client id for the gimme-creds-server
+                client_id = OAuth Client ID - used for the gimme-creds-server in Okta classic and user authentication in Okta Identity Engine
                 okta_auth_server = Server ID for the OAuth authorization server used by gimme-creds-server
                 write_aws_creds = Option to write creds to ~/.aws/credentials
                 cred_profile = Use DEFAULT or Role-based name as the profile in ~/.aws/credentials
                 aws_appname = (optional) Okta AWS App Name
                 aws_rolename =  (optional) Okta Role ARN
                 okta_username = Okta username
                 aws_default_duration = Default AWS session duration (3600)
@@ -339,39 +345,39 @@
         self._okta_auth_server = okta_auth_server
 
         return okta_auth_server
 
     def _get_client_id_entry(self, default_entry):
         """ Get and validate client_id """
         ui.default.message(
-            "Enter the OAuth client id for the gimme-creds-server. If you do not know this value, contact your Okta admin")
+            "Enter the OAuth Client ID for the gimme-aws-creds. This value is REQUIRED for Okta Identity Engine domains. If you do not know this value, contact your Okta admin")
 
         client_id = self._get_user_input("Client ID", default_entry)
         self._client_id = client_id
 
         return client_id
 
     def _get_appurl_entry(self, default_entry):
         """ Get and validate app_url """
         ui.default.message(
             "Enter the application link. This is https://something.okta[preview].com/home/amazon_aws/<app_id>/something")
-        okta_org_url_valid = False
+        okta_app_url_valid = False
         app_url = default_entry
 
-        while okta_org_url_valid is False:
+        while okta_app_url_valid is False:
             app_url = self._get_user_input("Application url", default_entry)
             url_parse_results = urlparse(app_url)
             allowlist = [
                 "okta.com",
                 "oktapreview.com",
                 "okta-emea.com",
             ]
 
             if url_parse_results.scheme == "https" and any(urlelement in url_parse_results.hostname for urlelement in allowlist):
-                okta_org_url_valid = True
+                okta_app_url_valid = True
             else:
                 ui.default.warning(
                     "Okta organization URL must be HTTPS URL for okta.com or oktapreview.com or okta-emea.com domain")
 
         self._app_url = app_url
 
         return app_url
```

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/default.py` & `gimme aws creds-2.6.0/gimme_aws_creds/default.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/duo.py` & `gimme aws creds-2.6.0/gimme_aws_creds/duo.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/errors.py` & `gimme aws creds-2.6.0/gimme_aws_creds/errors.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/main.py` & `gimme aws creds-2.6.0/gimme_aws_creds/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 import configparser
 import json
 import os
 import re
 import sys
 import concurrent.futures
 
-
 # extras
 import boto3
+import requests
 from botocore.exceptions import ClientError
 from okta.framework.ApiClient import ApiClient
 from okta.framework.OktaError import OktaError
 
 # local imports
-from . import errors, ui
+from . import errors, ui, version
 from .aws import AwsResolver
 from .config import Config
 from .default import DefaultResolver
-from .okta import OktaClient
+from .okta_identity_engine import OktaIdentityEngine
+from .okta_classic import OktaClassicClient
 from .registered_authenticators import RegisteredAuthenticators
 
 
 class GimmeAWSCreds(object):
     """
        This is a CLI tool that gets temporary AWS credentials
        from Okta based the available AWS Okta Apps and roles
@@ -112,15 +113,15 @@
         self.AWS_CONFIG = self.ui.environ.get(
             'AWS_SHARED_CREDENTIALS_FILE',
             os.path.join(self.FILE_ROOT, '.aws', 'credentials')
         )
         self._cache = {}
 
     #  this is modified code from https://github.com/nimbusscale/okta_aws_login
-    def _write_aws_creds(self, profile, access_key, secret_key, token, aws_config=None):
+    def _write_aws_creds(self, profile, access_key, secret_key, token, expiration, aws_config=None):
         """ Writes the AWS STS token into the AWS credential file"""
         # Check to see if the aws creds path exists, if not create it
         aws_config = aws_config or self.AWS_CONFIG
         creds_dir = os.path.dirname(aws_config)
 
         if os.path.exists(creds_dir) is False:
             os.makedirs(creds_dir)
@@ -136,14 +137,15 @@
         if not config.has_section(profile):
             config.add_section(profile)
 
         config.set(profile, 'aws_access_key_id', access_key)
         config.set(profile, 'aws_secret_access_key', secret_key)
         config.set(profile, 'aws_session_token', token)
         config.set(profile, 'aws_security_token', token)
+        config.set(profile, 'x_security_token_expires', expiration)
 
         # Write the updated config file
         with open(aws_config, 'w+') as configfile:
             config.write(configfile)
         # Update file permissions to secure  sensitive credentials file
         os.chmod(aws_config, 0o600)
         self.ui.result('Written profile {} to {}'.format(profile, aws_config))
@@ -167,15 +169,16 @@
                     errs.append('{} is not set {} in profile! {}'.format(key, repr(value), str(profile.keys())))
 
         if not isinstance(credentials, dict):
             errs.append('credentials are not a dict!' + repr(credentials))
         else:
             for key in ('aws_access_key_id',
                         'aws_secret_access_key',
-                        'aws_session_token'):
+                        'aws_session_token',
+                        'expiration'):
                 value = credentials.get(key, None)
                 if not value:
                     errs.append(
                         '{} is not set {} in credentials! {}'.format(key, repr(value), str(credentials.keys())))
 
         if errs:
             for error in errs:
@@ -185,14 +188,15 @@
         arn = data.get('role', {}).get('arn', '<no-arn>')
         self.ui.result('Saving {} as {}'.format(arn, profile['name']))
         self._write_aws_creds(
             profile['name'],
             credentials['aws_access_key_id'],
             credentials['aws_secret_access_key'],
             credentials['aws_session_token'],
+            credentials['expiration'],
             aws_config=aws_config,
         )
 
     @staticmethod
     def _get_partition_from_saml_acs(saml_acs_url):
         """ Determine the AWS partition by looking at the ACS endpoint URL"""
         if saml_acs_url == 'https://signin.aws.amazon.com/saml':
@@ -510,14 +514,47 @@
         config = self.config
         return self._cache['conf_dict']
 
     @property
     def output_format(self):
         return self.conf_dict.setdefault('output_format', self.config.output_format)
 
+    def set_okta_platform(self, okta_platform):
+        self._cache['okta_platform'] = okta_platform
+    
+    @property
+    def okta_platform(self):
+        if 'okta_platform' in self._cache:
+            return self._cache['okta_platform']
+        
+        response = requests.get(
+            self.okta_org_url + '/.well-known/okta-organization',
+            headers={
+                'Accept': 'application/json',
+                'User-Agent': "gimme-aws-creds {}".format(version)
+            }
+        )
+
+        response_data = response.json()
+
+        if response.status_code == 200:
+            if response_data['pipeline'] == 'v1':
+                ret = 'classic'
+            elif response_data['pipeline'] == 'idx':
+                ret = 'identity_engine'
+                if not self.conf_dict.get('client_id'):
+                    raise errors.GimmeAWSCredsError('OAuth Client ID is required for Okta Identity Engine domains.  Try running --config again.')
+            else:
+                raise RuntimeError('Unknown Okta platform type: {}'.format(response_data['pipeline']))
+        else:
+            response.raise_for_status()
+
+        self.set_okta_platform(ret)
+        return ret
+
     @property
     def okta_org_url(self):
         ret = self.conf_dict.get('okta_org_url')
         if not ret:
             raise errors.GimmeAWSCredsError('No Okta organization URL in configuration.  Try running --config again.')
         return ret
 
@@ -529,39 +566,47 @@
         return ret
 
     @property
     def okta(self):
         if 'okta' in self._cache:
             return self._cache['okta']
 
-        okta = self._cache['okta'] = OktaClient(
-            self.ui,
-            self.okta_org_url,
-            self.config.verify_ssl_certs,
-            self.device_token,
-        )
+        if self.okta_platform == 'identity_engine':
+            okta = self._cache['okta'] = OktaIdentityEngine(
+                self.ui,
+                self.okta_org_url,
+                self.conf_dict.get('client_id'),
+                self.config.verify_ssl_certs
+            )
+        else:
+            okta = self._cache['okta'] = OktaClassicClient(
+                self.ui,
+                self.okta_org_url,
+                self.config.verify_ssl_certs,
+                self.device_token,
+            )
 
-        if self.config.username is not None:
-            okta.set_username(self.config.username)
-        elif self.conf_dict.get('okta_username'):
-            okta.set_username(self.conf_dict['okta_username'])
-
-        if self.conf_dict.get('okta_password'):
-            okta.set_password(self.conf_dict['okta_password'])
-
-        if self.conf_dict.get('preferred_mfa_type'):
-            okta.set_preferred_mfa_type(self.conf_dict['preferred_mfa_type'])
-
-        if self.config.mfa_code is not None:
-            okta.set_mfa_code(self.config.mfa_code)
-        elif self.conf_dict.get('okta_mfa_code'):
-            okta.set_mfa_code(self.conf_dict.get('okta_mfa_code'))
+            if self.config.username is not None:
+                okta.set_username(self.config.username)
+            elif self.conf_dict.get('okta_username'):
+                okta.set_username(self.conf_dict['okta_username'])
+
+            if self.conf_dict.get('okta_password'):
+                okta.set_password(self.conf_dict['okta_password'])
+
+            if self.conf_dict.get('preferred_mfa_type'):
+                okta.set_preferred_mfa_type(self.conf_dict['preferred_mfa_type'])
+
+            if self.config.mfa_code is not None:
+                okta.set_mfa_code(self.config.mfa_code)
+            elif self.conf_dict.get('okta_mfa_code'):
+                okta.set_mfa_code(self.conf_dict.get('okta_mfa_code'))
 
-        okta.set_remember_device(self.config.remember_device
-                                 or self.conf_dict.get('remember_device', False))
+            okta.set_remember_device(self.config.remember_device
+                or self.conf_dict.get('remember_device', False))
         return okta
 
     def get_resolver(self):
         if self.config.resolve:
             return AwsResolver(self.config.verify_ssl_certs)
         elif str(self.conf_dict.get('resolve_aws_alias')) == 'True':
             return AwsResolver(self.config.verify_ssl_certs)
@@ -577,16 +622,17 @@
     def set_auth_session(self, auth_session):
         self._cache['auth_session'] = auth_session
 
     @property
     def auth_session(self):
         if 'auth_session' in self._cache:
             return self._cache['auth_session']
-        auth_result = self.okta.auth_session(redirect_uri=self.conf_dict.get('app_url'))
+        auth_result = self.okta.auth_session(redirect_uri=self.conf_dict.get('app_url'), open_browser=self.config.open_browser)
         self.set_auth_session(auth_result)
+
         return auth_result
 
     @property
     def aws_results(self):
         if 'aws_results' in self._cache:
             return self._cache['aws_results']
         # Call the Okta APIs and process data locally
@@ -611,32 +657,34 @@
             aws_results = []
             new_app_entry = {
                 'id': 'fakeid',  # not used anyway
                 'name': 'fakelabel',  # not used anyway
                 'links': {'appLink': self.config.app_url}
             }
             aws_results.append(new_app_entry)
-            self.ui.info("Authentication Success!")
 
         # Use the gimme_creds_lambda service
         else:
             if not self.conf_dict.get('client_id'):
                 raise errors.GimmeAWSCredsError('No OAuth Client ID in configuration.  Try running --config again.')
             if not self.conf_dict.get('okta_auth_server'):
                 raise errors.GimmeAWSCredsError(
                     'No OAuth Authorization server in configuration.  Try running --config again.')
 
-            # Authenticate with Okta and get an OAuth access token
-            self.okta.auth_oauth(
-                self.conf_dict['client_id'],
-                authorization_server=self.conf_dict['okta_auth_server'],
-                access_token=True,
-                id_token=False,
-                scopes=['openid']
-            )
+            if self.okta_platform == 'classic':
+                # Authenticate with Okta and get an OAuth access token
+                self.okta.auth_oauth(
+                    self.conf_dict['client_id'],
+                    authorization_server=self.conf_dict['okta_auth_server'],
+                    access_token=True,
+                    id_token=False,
+                    scopes=['openid']
+                )
+            elif self.okta_platform == 'identity_engine':
+                auth_result = self.auth_session
 
             # Add Access Tokens to Okta-protected requests
             self.okta.use_oauth_access_token(True)
 
             self.ui.info("Authentication Success! Calling Gimme-Creds Server...")
             aws_results = self._call_gimme_creds_server(self.okta, self.gimme_creds_server)
 
@@ -650,15 +698,15 @@
         self._cache['aws_app'] = aws_app = self._get_selected_app(self.conf_dict.get('aws_appname'), self.aws_results)
         return aws_app
 
     @property
     def saml_data(self):
         if 'saml_data' in self._cache:
             return self._cache['saml_data']
-        self._cache['saml_data'] = saml_data = self.okta.get_saml_response(self.aws_app['links']['appLink'])
+        self._cache['saml_data'] = saml_data = self.okta.get_saml_response(self.aws_app['links']['appLink'], self.auth_session)
         return saml_data
 
     @property
     def aws_roles(self):
         if 'aws_roles' in self._cache:
             return self._cache['aws_roles']
 
@@ -795,19 +843,20 @@
             return self._cache['selected_aws_credentials']
         self._cache['selected_aws_credentials'] = ret = list(self.iter_selected_aws_credentials())
         return ret
 
     def _run(self):
         """ Pulling it all together to make the CLI """
         self.handle_action_configure()
-        self.handle_action_register_device()
         self.handle_action_list_profiles()
-        self.handle_action_store_json_creds()
-        self.handle_action_list_roles()
-        self.handle_setup_fido_authenticator()
+        if self.okta_platform == 'classic':
+            self.handle_action_register_device()
+            self.handle_action_store_json_creds()
+            self.handle_action_list_roles()
+            self.handle_setup_fido_authenticator()
   
         # for each data item, if we have an override on output, prioritize that
         # if we do not, prioritize writing credentials to file if that is in our
         # configuration. If we are not writing to a credentials file, use whatever
         # is in the output format field (default to exports)
         for data in self.iter_selected_aws_credentials():
             if self.config.action_output_format:
@@ -879,15 +928,15 @@
                 self.ui.warning('error parsing json line {}'.format(repr(line)))
                 continue
             self.write_aws_creds_from_data(data)
         raise errors.GimmeAWSCredsExitSuccess()
 
     def handle_action_register_device(self):
         # Capture the Device Token and write it to the config file
-        if self.device_token is None or self.config.action_register_device is True:
+        if self.okta_platform == "classic" and ( self.device_token is None or self.config.action_register_device is True ):
             if not self.config.action_register_device:
                 self.ui.notify('\n*** No device token found in configuration file, it will be created.')
                 self.ui.notify('*** You may be prompted for MFA more than once for this run.\n')
 
             auth_result = self.auth_session
             base_config = self.config.get_config_dict(include_inherits = False)
             base_config['device_token'] = auth_result['device_token']
```

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/okta.py` & `gimme aws creds-2.6.0/gimme_aws_creds/okta_classic.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,29 +33,29 @@
 from gimme_aws_creds.u2f import FactorU2F
 from gimme_aws_creds.webauthn import WebAuthnClient, FakeAssertion
 from . import errors, ui, version, duo
 from .errors import GimmeAWSCredsMFAEnrollStatus
 from .registered_authenticators import RegisteredAuthenticators
 
 
-class OktaClient(object):
+class OktaClassicClient(object):
     """
        The Okta Client Class performs the necessary API
-       calls to Okta to get temporary AWS credentials. An
-       Okta API key and URL must be provided.
+       calls to an Okta Classic domain to get temporary AWS credentials.
     """
 
     KEYRING_SERVICE = 'gimme-aws-creds'
     KEYRING_ENABLED = not isinstance(keyring.get_keyring(), FailKeyring)
 
     def __init__(self, gac_ui, okta_org_url, verify_ssl_certs=True, device_token=None):
         """
         :type gac_ui: ui.UserInterface
         :param okta_org_url: Base URL string for Okta IDP.
         :param verify_ssl_certs: Enable/disable SSL verification
+        :param device_token: Device Token value for Okta device ID
         """
         self.ui = gac_ui
         self._okta_org_url = okta_org_url
         self._verify_ssl_certs = verify_ssl_certs
 
         if verify_ssl_certs is False:
             requests.packages.urllib3.disable_warnings()
@@ -76,15 +76,15 @@
         # Allow up to 5 retries on requests to Okta in case we have network issues
         self._http_client = requests.Session()
         self._http_client.cookies = self._jar
 
         self.device_token = device_token
 
         retries = Retry(total=5, backoff_factor=1,
-                        method_whitelist=['GET', 'POST'])
+                        allowed_methods=['GET', 'POST'])
         self._http_client.mount('https://', HTTPAdapter(max_retries=retries))
 
     @property
     def device_token(self):
         return self._http_client.cookies.get('DT')
 
     @device_token.setter
@@ -684,15 +684,15 @@
             if 'stateToken' in response_data:
                 return {'stateToken': response_data['stateToken'], 'apiResponse': response_data}
             if 'sessionToken' in response_data:
                 return {'stateToken': None, 'sessionToken': response_data['sessionToken'], 'apiResponse': response_data}
         else:
             return {'stateToken': None, 'sessionToken': None, 'apiResponse': response_data}
 
-    def get_saml_response(self, url):
+    def get_saml_response(self, url, auth_session = None):
         """ return the base64 SAML value object from the SAML Response"""
         response = self._http_client.get(url, verify=self._verify_ssl_certs)
         response.raise_for_status()
 
         saml_response = None
         relay_state = None
         form_action = None
```

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/registered_authenticators.py` & `gimme aws creds-2.6.0/gimme_aws_creds/registered_authenticators.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/u2f.py` & `gimme aws creds-2.6.0/gimme_aws_creds/u2f.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/ui.py` & `gimme aws creds-2.6.0/gimme_aws_creds/ui.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds/webauthn.py` & `gimme aws creds-2.6.0/gimme_aws_creds/webauthn.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.5.0/gimme_aws_creds.egg-info/SOURCES.txt` & `gimme aws creds-2.6.0/gimme_aws_creds.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 MANIFEST.in
 NOTICE
 README.md
 requirements.txt
 setup.cfg
 setup.py
 bin/gimme-aws-creds
+bin/gimme-aws-creds-autocomplete.sh
 bin/gimme-aws-creds.cmd
 gimme_aws_creds/__init__.py
 gimme_aws_creds/aws.py
 gimme_aws_creds/common.py
 gimme_aws_creds/config.py
 gimme_aws_creds/default.py
 gimme_aws_creds/duo.py
 gimme_aws_creds/errors.py
 gimme_aws_creds/main.py
-gimme_aws_creds/okta.py
+gimme_aws_creds/okta_classic.py
+gimme_aws_creds/okta_identity_engine.py
 gimme_aws_creds/registered_authenticators.py
 gimme_aws_creds/u2f.py
 gimme_aws_creds/ui.py
 gimme_aws_creds/webauthn.py
 gimme_aws_creds.egg-info/PKG-INFO
 gimme_aws_creds.egg-info/SOURCES.txt
 gimme_aws_creds.egg-info/dependency_links.txt
```

### Comparing `gimme aws creds-2.5.0/setup.py` & `gimme aws creds-2.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='gimme aws creds',
     version=gimme_aws_creds.version,
     install_requires=requirements,
-    author='Ann Wallace',
-    author_email='ann.wallace@nike.com',
+    author='Eric Pierce',
+    author_email='eric.pierce@nike.com',
     description="A CLI to get temporary AWS credentials from Okta",
     url='https://github.com/Nike-Inc/gimme-aws-creds',
+    long_description=open("LONG_DESCRIPTION.md").read(),
+    python_requires=">=3.7",
     license='Apache License, v2.0',
     packages=find_packages(exclude=('tests', 'docs')),
     test_suite="tests",
-    scripts=['bin/gimme-aws-creds', 'bin/gimme-aws-creds.cmd'],
+    scripts=['bin/gimme-aws-creds', 'bin/gimme-aws-creds.cmd', 'bin/gimme-aws-creds-autocomplete.sh'],
     classifiers=[
         'Natural Language :: English',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: Apache Software License'
     ]
 )
```


# Comparing `tmp/fme_packager-1.3.1-py3-none-any.whl.zip` & `tmp/fme_packager-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 20068 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat       22 b- defN 23-Feb-09 23:47 fme_packager/__init__.py
+Zip file size: 21312 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-02 17:25 fme_packager/__init__.py
 -rw-rw-rw-  2.0 fat       90 b- defN 22-Nov-29 23:42 fme_packager/__main__.py
--rw-rw-rw-  2.0 fat     3829 b- defN 23-Jan-12 22:04 fme_packager/cli.py
+-rw-rw-rw-  2.0 fat     4445 b- defN 23-May-02 17:25 fme_packager/cli.py
 -rw-rw-rw-  2.0 fat      647 b- defN 22-Nov-29 23:42 fme_packager/exception.py
 -rw-rw-rw-  2.0 fat      543 b- defN 22-Nov-29 23:42 fme_packager/fme_env.py
--rw-rw-rw-  2.0 fat     9196 b- defN 23-Feb-09 22:53 fme_packager/help.py
+-rw-rw-rw-  2.0 fat     9196 b- defN 23-Feb-10 01:59 fme_packager/help.py
 -rw-rw-rw-  2.0 fat     3356 b- defN 22-Nov-29 23:42 fme_packager/metadata.py
 -rw-rw-rw-  2.0 fat     2457 b- defN 23-Jan-31 23:37 fme_packager/operations.py
--rw-rw-rw-  2.0 fat    20875 b- defN 23-Feb-08 22:25 fme_packager/packager.py
+-rw-rw-rw-  2.0 fat    21780 b- defN 23-May-02 17:25 fme_packager/packager.py
 -rw-rw-rw-  2.0 fat     4692 b- defN 23-Jan-12 22:04 fme_packager/spec.json
 -rw-rw-rw-  2.0 fat     6158 b- defN 23-Jan-12 22:04 fme_packager/transformer.py
--rw-rw-rw-  2.0 fat     1307 b- defN 23-Feb-10 01:08 fme_packager-1.3.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3649 b- defN 23-Feb-10 01:08 fme_packager-1.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-10 01:08 fme_packager-1.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       54 b- defN 23-Feb-10 01:08 fme_packager-1.3.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Feb-10 01:08 fme_packager-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1391 b- defN 23-Feb-10 01:08 fme_packager-1.3.1.dist-info/RECORD
-17 files, 58371 bytes uncompressed, 17780 bytes compressed:  69.5%
+-rw-rw-rw-  2.0 fat     2270 b- defN 23-May-02 17:25 fme_packager/verifier.py
+-rw-rw-rw-  2.0 fat     1307 b- defN 23-May-02 17:25 fme_packager-1.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3649 b- defN 23-May-02 17:25 fme_packager-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 17:25 fme_packager-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       54 b- defN 23-May-02 17:25 fme_packager-1.4.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-May-02 17:25 fme_packager-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1472 b- defN 23-May-02 17:25 fme_packager-1.4.0.dist-info/RECORD
+18 files, 62244 bytes uncompressed, 18900 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -27,26 +27,29 @@
 
 Filename: fme_packager/spec.json
 Comment: 
 
 Filename: fme_packager/transformer.py
 Comment: 
 
-Filename: fme_packager-1.3.1.dist-info/LICENSE
+Filename: fme_packager/verifier.py
 Comment: 
 
-Filename: fme_packager-1.3.1.dist-info/METADATA
+Filename: fme_packager-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: fme_packager-1.3.1.dist-info/WHEEL
+Filename: fme_packager-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: fme_packager-1.3.1.dist-info/entry_points.txt
+Filename: fme_packager-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: fme_packager-1.3.1.dist-info/top_level.txt
+Filename: fme_packager-1.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fme_packager-1.3.1.dist-info/RECORD
+Filename: fme_packager-1.4.0.dist-info/top_level.txt
+Comment: 
+
+Filename: fme_packager-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fme_packager/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.3.1"
+__version__ = "1.4.0"
```

## fme_packager/cli.py

```diff
@@ -1,134 +1,145 @@
-"""
-fme_packager command line interface.
-"""
-import inspect
-import os
-import shutil
-import sys
-import sysconfig
-from pathlib import Path
-
-import click
-from cookiecutter.main import cookiecutter
-
-import fme_packager
-from fme_packager.packager import FMEPackager
-
-
-@click.group()
-def cli():
-    """
-    fme_packager: The FME Packages Tool.
-    """
-    pass
-
-
-COOKIECUTTER_TEMPLATES = {
-    "transformer": "https://github.com/safesoftware/fpkg-transformer-template/archive/refs/heads/main.zip",
-}
-
-
-@cli.command()
-@click.argument("template", type=click.Choice(sorted(COOKIECUTTER_TEMPLATES.keys())))
-def init(template):
-    """
-    Initialize an FME Package from a template.
-
-    The template is initialized in a subdirectory of the current directory.
-
-    TEMPLATE -- Name of the template to use.
-    """
-    print("Enter the values to use for the template. Press Enter to accept the [default].")
-    cookiecutter(COOKIECUTTER_TEMPLATES[template])
-
-
-@cli.command()
-@click.argument("help_path", type=click.Path(exists=True, file_okay=True))
-@click.argument("fpkg_path", type=click.Path(exists=True, file_okay=False, writable=True))
-def apply_help(help_path, fpkg_path):
-    """
-    Import an Safe TechPubs doc export into an FME Package directory.
-
-    This operation also converts package_aliases.flali to package_help.csv at the destination.
-
-    HELP_PATH -- Path to a ZIP or directory of an Safe TechPubs doc export. Read only.
-
-    FPKG_PATH -- Path to the FME Package root. Its 'help' subdirectory will be recreated.
-    """
-    steps = FMEPackager(fpkg_path)
-    steps.apply_help(help_path)
-
-
-@cli.command()
-@click.argument("path", type=click.Path(exists=True, file_okay=False, writable=True))
-def pack(path):
-    """
-    Create an .fpkg file.
-
-    Package contents are validated during this process.
-    Components not referenced by the package's metadata.yml may not be included in the resulting fpkg.
-
-    PATH -- Path to an FME Package directory.
-    """
-    steps = FMEPackager(path)
-    steps.build()
-    steps.make_fpkg()
-
-
-@cli.command()
-@click.option(
-    "--fme-home",
-    prompt=True,
-    default=lambda: os.environ.get("FME_HOME"),
-    show_default="FME_HOME environment variable",
-    type=click.Path(exists=True, file_okay=False, writable=True),
-    required=True,
-    help="Path to FME installation",
-)
-@click.option(
-    "--site-packages-dir",
-    default=lambda: sysconfig.get_paths()["purelib"],
-    show_default="current Python environment",
-    type=click.Path(exists=True, file_okay=False, writable=True),
-    required=True,
-    help="Path to Python environment's site-packages",
-)
-def config_env(fme_home, site_packages_dir):
-    """
-    Configure a Python environment for access to fmeobjects
-    and the Python libraries included with FME.
-    """
-    leaf_dir = "python%s%s" % (sys.version_info.major, sys.version_info.minor)
-    paths_to_add = [
-        "#" + fme_home,
-        os.path.join(fme_home, "python"),
-        os.path.join(fme_home, "python", leaf_dir),
-        os.path.join(fme_home, "fmeobjects", leaf_dir),
-    ]
-
-    dst_pth = os.path.join(site_packages_dir, "fme_env.pth")
-    print("Writing " + dst_pth)
-    with open(dst_pth, "w") as f:
-        for path in paths_to_add:
-            f.write(path + "\n")
-        f.write("import fme_env\n")
-
-    dst_py = os.path.join(site_packages_dir, "fme_env.py")
-    print("Writing " + dst_py)
-    src = Path(inspect.getfile(fme_packager)).parent / "fme_env.py"
-    shutil.copy(src, dst_py)
-
-    print("\nThis Python environment is now set up for access to FME and fmeobjects.")
-    print("If the FME install location changes, re-run this script to update paths.")
-
-
-@cli.command()
-def version():
-    """
-    Print the version of fme_packager.
-    """
-    print("fme_packager " + fme_packager.__version__)
-
-
-if __name__ == "__main__":
-    cli()
+"""
+fme_packager command line interface.
+"""
+import inspect
+import os
+import shutil
+import sys
+import sysconfig
+from pathlib import Path
+
+import click
+from cookiecutter.main import cookiecutter
+
+import fme_packager
+from fme_packager.packager import FMEPackager
+from fme_packager.verifier import FMEVerifier
+
+
+@click.group()
+@click.version_option(package_name="fme_packager")
+def cli():
+    """
+    fme_packager: The FME Packages Tool.
+    """
+    pass
+
+
+COOKIECUTTER_TEMPLATES = {
+    "transformer": "https://github.com/safesoftware/fpkg-transformer-template/archive/refs/heads/main.zip",
+}
+
+
+@cli.command()
+@click.argument("template", type=click.Choice(sorted(COOKIECUTTER_TEMPLATES.keys())))
+def init(template):
+    """
+    Initialize a FME Package from a template.
+
+    The template is initialized in a subdirectory of the current directory.
+
+    TEMPLATE -- Name of the template to use.
+    """
+    print("Enter the values to use for the template. Press Enter to accept the [default].")
+    cookiecutter(COOKIECUTTER_TEMPLATES[template])
+
+
+@cli.command()
+@click.argument("help_path", type=click.Path(exists=True, file_okay=True))
+@click.argument("fpkg_path", type=click.Path(exists=True, file_okay=False, writable=True))
+def apply_help(help_path, fpkg_path):
+    """
+    Import a Safe TechPubs doc export into an FME Package directory.
+
+    This operation also converts package_aliases.flali to package_help.csv at the destination.
+
+    HELP_PATH -- Path to a ZIP or directory of a Safe TechPubs doc export. Read only.
+
+    FPKG_PATH -- Path to the FME Package root. Its 'help' subdirectory will be recreated.
+    """
+    steps = FMEPackager(fpkg_path)
+    steps.apply_help(help_path)
+
+
+@cli.command()
+@click.argument("path", type=click.Path(exists=True, file_okay=False, writable=True))
+def pack(path):
+    """
+    Create an .fpkg file.
+
+    Package contents are validated during this process.
+    Components not referenced by the package's metadata.yml may not be included in the resulting fpkg.
+
+    PATH -- Path to an FME Package directory.
+    """
+    steps = FMEPackager(path)
+    steps.build()
+    steps.make_fpkg()
+
+
+@cli.command()
+@click.argument("file", type=click.Path(exists=False, file_okay=True))
+@click.option("--verbose", "-v", is_flag=True, help="Show build steps")
+@click.option("--json", is_flag=True, help="Output result as JSON")
+def verify(file, verbose, json):
+    """
+    Verify that a .fpkg file is valid.
+
+    Package contents are validated during this process.
+
+    FILE -- Path to an FME .fpkg package file.
+    """
+    verifier = FMEVerifier(file, verbose, json)
+    result = verifier.verify()
+    print(result)
+
+
+@cli.command()
+@click.option(
+    "--fme-home",
+    prompt=True,
+    default=lambda: os.environ.get("FME_HOME"),
+    show_default="FME_HOME environment variable",
+    type=click.Path(exists=True, file_okay=False, writable=True),
+    required=True,
+    help="Path to FME installation",
+)
+@click.option(
+    "--site-packages-dir",
+    default=lambda: sysconfig.get_paths()["purelib"],
+    show_default="current Python environment",
+    type=click.Path(exists=True, file_okay=False, writable=True),
+    required=True,
+    help="Path to Python environment's site-packages",
+)
+def config_env(fme_home, site_packages_dir):
+    """
+    Configure a Python environment for access to fmeobjects
+    and the Python libraries included with FME.
+    """
+    leaf_dir = "python%s%s" % (sys.version_info.major, sys.version_info.minor)
+    paths_to_add = [
+        "#" + fme_home,
+        os.path.join(fme_home, "python"),
+        os.path.join(fme_home, "python", leaf_dir),
+        os.path.join(fme_home, "fmeobjects", leaf_dir),
+    ]
+
+    dst_pth = os.path.join(site_packages_dir, "fme_env.pth")
+    print("Writing " + dst_pth)
+    with open(dst_pth, "w") as f:
+        for path in paths_to_add:
+            f.write(path + "\n")
+        f.write("import fme_env\n")
+
+    dst_py = os.path.join(site_packages_dir, "fme_env.py")
+    print("Writing " + dst_py)
+    src = Path(inspect.getfile(fme_packager)).parent / "fme_env.py"
+    shutil.copy(src, dst_py)
+
+    print("\nThis Python environment is now set up for access to FME and fmeobjects.")
+    print("If the FME install location changes, re-run this script to update paths.")
+
+
+if __name__ == "__main__":
+    cli()
```

## fme_packager/packager.py

```diff
@@ -1,518 +1,529 @@
-import csv
-import os
-import shutil
-import tempfile
-import warnings
-import zipfile
-from fnmatch import fnmatch
-from pathlib import Path
-
-import png
-import xmltodict
-from build import ProjectBuilder
-from jsonschema import validate
-from packaging import version
-
-from fme_packager.exception import (
-    TransformerPythonCompatError,
-    CustomTransformerPythonCompatError,
-)
-from fme_packager.help import HelpBuilder
-from fme_packager.metadata import load_fpkg_metadata, load_metadata_json_schema, TransformerMetadata
-from fme_packager.operations import (
-    build_fpkg_filename,
-    parse_formatinfo,
-    TREE_COPY_IGNORE_GLOBS,
-)
-from fme_packager.transformer import load_transformer, CustomTransformer
-
-
-def is_valid_python_compatibility(python_compat_version):
-    """
-    Checks for a valid python compatibility value.
-
-    :param str python_compat_version: Python compatibility version
-    :rtype: bool
-    """
-    minimum_requirement = "35"
-    is_python_3 = python_compat_version.startswith("3")
-    meets_minimum_requirements = False
-    if is_python_3:
-        meets_minimum_requirements = version.parse(python_compat_version) >= version.parse(
-            minimum_requirement
-        )
-    return is_python_3 and meets_minimum_requirements
-
-
-def check_exists_and_copy(src, dest):
-    """
-    Copy source contents to a source path.
-
-    :raises ValueError: If the source path does not exist.
-    :param src: The source path.
-    :param dest: The destination path.
-    """
-    if not os.path.exists(src):
-        raise ValueError("{} is required but does not exist".format(src))
-    shutil.copy(src, dest)
-
-
-def enforce_png(path, min_width=0, min_height=0, square=False):
-    """
-    Enforces the path is a valid PNG file and the PNG meets a minimum height and width requirement.
-
-    :raises ValueError: If the PNG is invalid or does not meet the minimum requirements.
-    :param path: Path to PNG file.
-    :param min_width: The minimum width of the image.
-    :param min_height: The minimum width of the image.
-    :param square: Whether the image should be square.
-    """
-    width, height, _, _ = png.Reader(filename=path).read()  # Raises if not PNG
-    if width < min_width or height < min_height:
-        raise ValueError(
-            "Min dimensions are {}x{}. {} is {}x{}".format(
-                min_width, min_height, path, width, height
-            )
-        )
-    if square and width != height:
-        raise ValueError("{} must be square".format(path))
-
-
-def fq_format_short_name(publisher_uid, package_uid, format_name):
-    """
-    Formats the publisher_uid, package_uid and format_name
-
-    :param publisher_uid: The Publisher unique identifier.
-    :param package_uid: The package unique identifier.
-    :param format_name: The format name.
-    :return: publisher_uid, package_uid, format_name dot delimited and upper case.
-    """
-    return "{}.{}.{}".format(publisher_uid, package_uid, format_name).upper()
-
-
-def check_fmf(package_metadata, format_metadata, fmf_path):
-    """
-    Checks the fmf file is consistent with the package and format metadata.
-
-    :raises ValueError: If the fmf fails the check.
-    :param package_metadata: The package metadata.
-    :param format_metadata: The format metadata.
-    :param fmf_path: The fmf file path.
-    """
-    with open(fmf_path) as inf:
-        contents = inf.read()
-
-    fqname = fq_format_short_name(
-        package_metadata.publisher_uid, package_metadata.uid, format_metadata.name
-    )
-
-    if (
-        "SOURCE_READER {}".format(fqname) not in contents
-        or "FORMAT_NAME {}".format(fqname) not in contents
-    ):
-        raise ValueError("SOURCE_READER and FORMAT_NAME must be '{}'".format(fqname))
-
-
-def check_formatinfo(package_metadata, format_metadata, db_path):
-    """
-    Checks formatinfo is consistent with the package and format metadata.
-
-    :param package_metadata: The package metadata.
-    :param format_metadata: The format metadata.
-    :param db_path: The path to the format file.
-    """
-    line = None
-    with open(db_path) as inf:
-        for line in inf:
-            if line.startswith(";"):
-                continue  # comment line.
-
-    if not line:
-        raise ValueError("{} empty".format(db_path))
-
-    fqname = fq_format_short_name(
-        package_metadata.publisher_uid, package_metadata.uid, format_metadata.name
-    )
-
-    formatinfo = parse_formatinfo(line)
-    if formatinfo.FORMAT_NAME != fqname:
-        raise ValueError("{} must have FORMAT_NAME of '{}'".format(db_path, fqname))
-
-
-class FMEPackager:
-    def __init__(self, src_dir):
-        self.src_dir = Path(src_dir)
-        self.build_dir = self.src_dir / "build"
-        self.dist_dir = self.src_dir / "dist"
-        self.src_python_dir = self.src_dir / "python"
-
-        self.metadata = load_fpkg_metadata(src_dir)
-
-        validate(self.metadata.dict, load_metadata_json_schema())
-
-    def apply_help(self, help_src):
-        """
-        Import an Safe TechPubs doc export into an FME Package directory.
-
-        :param help_src: Help source path.
-        """
-        tmp_doc_dir = tempfile.mkdtemp(prefix="fme-packager_")
-        try:
-            # If help source is a ZIP, extract it to a temporary folder.
-            if os.path.isfile(help_src):
-                with zipfile.ZipFile(help_src) as zipf:
-                    print("Extracting {} to {}".format(help_src, tmp_doc_dir))
-                    zipf.extractall(tmp_doc_dir)
-                root_contents = os.listdir(tmp_doc_dir)
-                # If help ZIP started with a single root level folder, then unnest.
-                if len(root_contents) == 1:
-                    nested_dir = os.path.join(tmp_doc_dir, root_contents[0])
-                    print("Flattening single top-level folder {}".format(nested_dir))
-                    for item in os.listdir(nested_dir):
-                        shutil.move(os.path.join(nested_dir, item), tmp_doc_dir)
-                    os.rmdir(nested_dir)
-                help_src = tmp_doc_dir
-
-            # Parse flali file ahead of anything else.
-            flali_path = os.path.join(help_src, "package_aliases.flali")
-            with open(flali_path, encoding="utf-8") as xmlin:
-                aliases_xml = xmltodict.parse(xmlin.read())
-
-            embedded_doc_dirs = list(filter(lambda x: x.startswith("!"), os.listdir(help_src)))
-            if embedded_doc_dirs:
-                warnings.warn(
-                    "{} embedded doc folders (starting with '!'). Avoid these if possible".format(
-                        len(embedded_doc_dirs)
-                    )
-                )
-
-            # (Re)create destination help folder and copy over the bulk of the doc files.
-            dest = os.path.join(self.src_dir, "help")
-            if os.path.exists(dest):
-                print("Deleting {}".format(dest))
-                shutil.rmtree(dest)
-            shutil.copytree(help_src, dest, ignore=shutil.ignore_patterns(*TREE_COPY_IGNORE_GLOBS))
-        finally:
-            shutil.rmtree(tmp_doc_dir)
-
-        # Convert flali to CSV and put it in the destination.
-        # Skip rows that refer to doc files that aren't present in the doc ZIP.
-        copied_rows = 0
-        with open(os.path.join(dest, "package_help.csv"), "w", newline="") as csvout:
-            writer = csv.writer(csvout)
-            rows = aliases_xml["CatapultAliasFile"]["Map"]
-            if not isinstance(rows, list):
-                rows = [rows]
-            for row in rows:
-                name = row["@Name"].replace(".", "_")
-                link = row["@Link"]
-                if link.startswith("/Content"):
-                    new_link = link.replace("/Content", "", 1)
-                    link = new_link
-                expected_doc_path = os.path.join(dest, link.lstrip("/"))
-                if os.path.exists(expected_doc_path):
-                    print("{} exists".format(expected_doc_path))
-                    writer.writerow([name, link])
-                    copied_rows += 1
-        print("Wrote {} of {} flali row(s) to package_help.csv".format(copied_rows, len(rows)))
-        if not copied_rows:
-            raise ValueError("flali doesn't reference any included doc")
-
-    def make_fpkg(self):
-        """
-        Create an .fpkg file from package build files.
-        """
-
-        if not self.dist_dir.exists():
-            self.dist_dir.mkdir(parents=True)
-
-        fpkg_filename = build_fpkg_filename(
-            self.metadata.publisher_uid, self.metadata.uid, self.metadata.version
-        )
-        fpkg_path = self.dist_dir / fpkg_filename
-        print(f"Saving fpkg to {fpkg_path}")
-
-        if fpkg_path.exists():
-            fpkg_path.unlink()
-
-        new_zip = shutil.make_archive(fpkg_path, "zip", root_dir=self.build_dir)
-        Path(new_zip).rename(fpkg_path)  # Strip zip extension
-        print("Done.")
-
-    def build(self):
-        """
-        Build and validate package files.
-        """
-        print("Collecting files into {}".format(self.build_dir))
-
-        # Clear out the build dir.
-        if os.path.exists(self.build_dir):
-            shutil.rmtree(self.build_dir)
-        self.build_dir.mkdir(parents=True)
-
-        for required_file in ["package.yml", "README.md", "CHANGES.md"]:
-            check_exists_and_copy(self.src_dir / required_file, self.build_dir)
-
-        self._copy_icon()
-
-        self._copy_transformers()
-        self._copy_web_services()
-        self._copy_web_filesystems()
-        self._copy_formats()
-        self._copy_localization()
-        self._copy_help()
-
-        self._build_wheels()
-        self._copy_wheels()
-        self._check_wheels()
-
-    def _copy_formats(self):
-        # First, copy all files we don't specifically care about.
-        # Ignore FMF and etc for formats not mentioned in metadata.
-        src = self.src_dir / "formats"
-        dst = self.build_dir / "formats"
-        if src.is_dir():
-            shutil.copytree(src, dst, ignore=shutil.ignore_patterns(*TREE_COPY_IGNORE_GLOBS))
-
-        for fmt in self.metadata.formats:
-            print(f"Working on format: {fmt.name}")
-
-            if not (dst / f"{fmt.name}.md").is_file():
-                raise ValueError(f"{fmt.name} is missing doc")
-
-            fms_path = src / f"{fmt.name}.fms"
-            if fms_path.is_file():
-                shutil.copy(fms_path, dst)
-
-            fmf_path = src / f"{fmt.name}.fmf"
-            if not fmf_path.is_file():
-                raise ValueError(f"{fmf_path} is in metadata, but was not found")
-            check_fmf(self.metadata, fmt, fmf_path)
-            shutil.copy(fmf_path, dst)
-
-            db_path = src / f"{fmt.name}.db"
-            if not db_path.is_file():
-                raise ValueError(f"{db_path} is in metadata, but was not found")
-            check_formatinfo(self.metadata, fmt, db_path)
-            shutil.copy(db_path, dst)
-
-    def validate_transformer(self, transformer_path, expected_metadata: TransformerMetadata):
-        print(f"Checking {transformer_path}")
-        transformer_file = load_transformer(transformer_path)
-
-        expected_fqname = "{}.{}.{}".format(
-            self.metadata.publisher_uid, self.metadata.uid, expected_metadata.name
-        )
-
-        transformer_versions = list(transformer_file.versions())
-        if not transformer_versions:
-            raise ValueError(f"{transformer_path} defines no versions")
-        # Validations below apply to all versions of the transformer
-        for transformer in transformer_versions:
-            if transformer.version < 1:
-                raise ValueError(f"Invalid transformer version {transformer.version}")
-            if transformer.name != expected_fqname:
-                raise ValueError(f"Name must be '{expected_fqname}', not '{transformer.name}'")
-            if isinstance(transformer, CustomTransformer):
-                if transformer.header.insert_mode != '"Linked Always"':
-                    raise ValueError(
-                        f'Custom transformer Insert Mode must be "Linked Always", not {transformer.header.insert_mode}'
-                    )
-                if transformer.header.build_num < self.metadata.minimum_fme_build:
-                    raise ValueError(
-                        "Custom transformer created with FME build older than fme_minimum_build in package.yml"
-                    )
-
-        # Validations below apply only to the latest version of the transformer
-        latest = transformer_versions[0]  # First definition in file
-        if latest.version != expected_metadata.version:
-            raise ValueError(f"Missing version {expected_metadata.version}")
-        if not latest.python_compatibility and self.metadata.minimum_fme_build < 23000:
-            raise ValueError("Python Compatibility setting required when minimum_fme_build < 23000")
-        elif latest.python_compatibility and not is_valid_python_compatibility(
-            latest.python_compatibility
-        ):
-            if not isinstance(latest, CustomTransformer):
-                raise TransformerPythonCompatError(expected_metadata.name)
-            elif isinstance(latest, CustomTransformer) and latest.python_compatibility != "2or3":
-                raise CustomTransformerPythonCompatError(expected_metadata.name)
-
-    def _copy_transformers(self):
-        # First, copy all files we don't specifically care about.
-        # Ignore FMX and FMS for transformers not mentioned in metadata.
-        src = self.src_dir / "transformers"
-        dst = self.build_dir / "transformers"
-        if src.is_dir():
-            shutil.copytree(src, dst, ignore=shutil.ignore_patterns(*TREE_COPY_IGNORE_GLOBS))
-
-        for transformer in self.metadata.transformers:
-            print(f"Working on transformer: {transformer.name}")
-
-            if transformer.version < 1:
-                raise ValueError(f"{transformer.name} version must be >= 1")
-
-            if not (dst / f"{transformer.name}.md").is_file():
-                raise ValueError(f"{transformer.name} is missing doc")
-
-            fms_path = src / f"{transformer.name}.fms"
-            if fms_path.is_file():
-                shutil.copy(fms_path, dst)
-
-            fmx_path = src / f"{transformer.name}.fmx"
-            fmxj_path = src / f"{transformer.name}.fmxj"
-            if fmx_path.is_file() and fmxj_path.is_file():
-                raise ValueError(f"{transformer.name} cannot have both FMX and FMXJ")
-            if not fmx_path.is_file() and not fmxj_path.is_file():
-                raise ValueError(f"{fmx_path} is in metadata, but was not found")
-            transformer_path = fmx_path if fmx_path.is_file() else fmxj_path
-            if transformer_path == fmxj_path and self.metadata.minimum_fme_build < 23146:
-                raise ValueError("FMXJ requires minimum_fme_build >= 23146")
-
-            # Copy file if it passed validation
-            self.validate_transformer(transformer_path, transformer)
-            shutil.copy(transformer_path, dst)
-
-    def _copy_web_services(self):
-        dest = self.build_dir / "web_services"
-        for web_service in self.metadata.web_services:
-            # fpkg spec says web service metadata entries must be full filename. Don't assume xml.
-            definition_path = self.src_dir / "web_services" / web_service.name
-            if not definition_path.exists():
-                raise ValueError(
-                    f"Web Service '{web_service.name}' is in metadata, but was not found"
-                )
-            if not dest.exists():
-                dest.mkdir(parents=True)
-
-            # TODO: Validate contents of XML.
-            print(f"Copying Web Service: {definition_path.name}")
-            shutil.copy(definition_path, dest)
-
-    def _copy_web_filesystems(self):
-        src = self.src_dir / "web_filesystems"
-        dest = self.build_dir / "web_filesystems"
-        for web_filesystem in self.metadata.web_filesystems:
-            definition_path = src / f"{web_filesystem.name}.fme"
-            if not definition_path.is_file():
-                raise ValueError(
-                    f"Web Filesystem '{web_filesystem.name}' is in metadata, but was not found"
-                )
-            if not dest.exists():
-                dest.mkdir(parents=True)
-
-            # TODO: Validate contents of .fme file.
-            print(f"Copying Web Filesystem: {definition_path.name}")
-            shutil.copy(definition_path, dest)
-
-            icon_path = src / f"{web_filesystem.name}.png"
-            if icon_path.is_file():
-                enforce_png(icon_path)
-                # Specification doesn't say anything about dimensions.
-                shutil.copy(icon_path, dest)
-
-    def _copy_icon(self):
-        path = self.src_dir / "icon.png"
-        if not path.is_file():
-            print("FME package has no icon")
-            return
-        enforce_png(path, min_width=200, min_height=200, square=True)
-        print("Icon is OK")
-        shutil.copy(path, self.build_dir)
-
-    def _build_wheels(self):
-        original_cwd = os.getcwd()
-
-        if not self.src_python_dir.exists():
-            return
-
-        for path in self.src_python_dir.iterdir():
-            if (path / "setup.py").is_file() or (path / "setup.cfg").is_file():
-                print(f"\nBuilding Python wheel: {path}")
-                os.chdir(path)
-                if os.path.exists("build"):
-                    shutil.rmtree("build")
-                # Simple solution to avoid needing to figure out which output is the one we want.
-                # The only wheel in the directory will be the one to include in the fpkg.
-                if os.path.exists("dist"):
-                    shutil.rmtree("dist")
-                try:
-                    ProjectBuilder(".").build("wheel", "dist")
-                finally:
-                    os.chdir(original_cwd)
-
-    def _copy_wheels(self):
-        if not self.src_python_dir.is_dir():
-            return
-
-        wheels_dest = self.build_dir / "python"
-        wheels_dest.mkdir(parents=True)
-
-        for path in self.src_python_dir.iterdir():
-            if os.path.isfile(path) and path.suffix == ".whl":
-                shutil.copy(path, wheels_dest)
-
-            built_wheels_dir = path / "dist"
-            if built_wheels_dir.is_dir():
-                built_wheels_for_lib = [
-                    name for name in built_wheels_dir.iterdir() if name.suffix == ".whl"
-                ]
-                assert len(built_wheels_for_lib) == 1
-                shutil.copy(built_wheels_for_lib[0], wheels_dest)
-
-    def _check_wheels(self):
-        wheels_path = self.build_dir / "python"
-
-        wheel_names = os.listdir(wheels_path) if wheels_path.is_dir() else []
-        for expected_py_package in self.metadata.python_packages:
-            lib_name = expected_py_package.name
-            if not any(
-                wheel_name.startswith(lib_name) or wheel_name.startswith(lib_name.replace("-", "_"))
-                for wheel_name in wheel_names
-            ):
-                raise ValueError(f"Python library '{lib_name}' is in metadata, but was not found")
-
-        if not wheels_path.is_dir():
-            return
-        for wheel_path in wheels_path.iterdir():
-            wheel_name = wheel_path.name
-            if "py3" not in wheel_name:
-                warnings.warn("{} is not a Python 3 wheel".format(wheel_name))
-            if not wheel_name.endswith("-none-any.whl"):
-                warnings.warn("{} is not a pure-Python wheel".format(wheel_name))
-
-    def _copy_localization(self):
-        # Copy any optional localization files. The only sanity check is a filename whitelist:
-        # guiprompts_??.txt, transformer-localized.??, FormatOrTransformerName_??.md
-        # ?? is a 2-letter language code.
-        # Contents of files aren't validated. It's up to Workbench to ignore anything malformed.
-        dest = self.build_dir / "localization"
-        src = self.src_dir / "localization"
-        if not src.is_dir():
-            return
-
-        keywords = [f.name for f in self.metadata.formats] + [
-            t.name for t in self.metadata.transformers
-        ]
-        localized_doc_globs = [keyword + "_??.md" for keyword in keywords]
-
-        for name in os.listdir(src):
-            path = src / name
-            if (
-                fnmatch(name, "guiprompts_??.txt")
-                or fnmatch(name, "transformer-localized.??")
-                or any(fnmatch(name, glob) for glob in localized_doc_globs)
-            ):
-                if not os.path.exists(dest):
-                    os.makedirs(dest)
-                print(f"Copying localization: {name}")
-                shutil.copy(path, dest)
-
-    def _copy_help(self):
-        src = self.src_dir / "help"
-        dest = self.build_dir / "help"
-        if not src.is_dir():
-            return
-
-        print("Copying help")
-        builder = HelpBuilder(self.metadata, src, dest)
-        builder.build()
+import csv
+import os
+import shutil
+import tempfile
+import warnings
+import zipfile
+from fnmatch import fnmatch
+from pathlib import Path
+
+import png
+import xmltodict
+from build import ProjectBuilder
+from jsonschema import validate
+from packaging import version
+
+from fme_packager.exception import (
+    TransformerPythonCompatError,
+    CustomTransformerPythonCompatError,
+)
+from fme_packager.help import HelpBuilder
+from fme_packager.metadata import load_fpkg_metadata, load_metadata_json_schema, TransformerMetadata
+from fme_packager.operations import (
+    build_fpkg_filename,
+    parse_formatinfo,
+    TREE_COPY_IGNORE_GLOBS,
+)
+from fme_packager.transformer import load_transformer, CustomTransformer
+
+
+def is_valid_python_compatibility(python_compat_version):
+    """
+    Checks for a valid python compatibility value.
+
+    :param str python_compat_version: Python compatibility version
+    :rtype: bool
+    """
+    minimum_requirement = "35"
+    is_python_3 = python_compat_version.startswith("3")
+    meets_minimum_requirements = False
+    if is_python_3:
+        meets_minimum_requirements = version.parse(python_compat_version) >= version.parse(
+            minimum_requirement
+        )
+    return is_python_3 and meets_minimum_requirements
+
+
+def check_exists_and_copy(src, dest):
+    """
+    Copy source contents to a source path.
+
+    :raises ValueError: If the source path does not exist.
+    :param src: The source path.
+    :param dest: The destination path.
+    """
+    if not os.path.exists(src):
+        raise ValueError("{} is required but does not exist".format(src))
+    shutil.copy(src, dest)
+
+
+def enforce_png(path, min_width=0, min_height=0, square=False):
+    """
+    Enforces the path is a valid PNG file and the PNG meets a minimum height and width requirement.
+
+    :raises ValueError: If the PNG is invalid or does not meet the minimum requirements.
+    :param path: Path to PNG file.
+    :param min_width: The minimum width of the image.
+    :param min_height: The minimum width of the image.
+    :param square: Whether the image should be square.
+    """
+    width, height, _, _ = png.Reader(filename=path).read()  # Raises if not PNG
+    if width < min_width or height < min_height:
+        raise ValueError(
+            "Min dimensions are {}x{}. {} is {}x{}".format(
+                min_width, min_height, path, width, height
+            )
+        )
+    if square and width != height:
+        raise ValueError("{} must be square".format(path))
+
+
+def fq_format_short_name(publisher_uid, package_uid, format_name):
+    """
+    Formats the publisher_uid, package_uid and format_name
+
+    :param publisher_uid: The Publisher unique identifier.
+    :param package_uid: The package unique identifier.
+    :param format_name: The format name.
+    :return: publisher_uid, package_uid, format_name dot delimited and upper case.
+    """
+    return "{}.{}.{}".format(publisher_uid, package_uid, format_name).upper()
+
+
+def check_fmf(package_metadata, format_metadata, fmf_path):
+    """
+    Checks the fmf file is consistent with the package and format metadata.
+
+    :raises ValueError: If the fmf fails the check.
+    :param package_metadata: The package metadata.
+    :param format_metadata: The format metadata.
+    :param fmf_path: The fmf file path.
+    """
+    with open(fmf_path) as inf:
+        contents = inf.read()
+
+    fqname = fq_format_short_name(
+        package_metadata.publisher_uid, package_metadata.uid, format_metadata.name
+    )
+
+    if (
+        "SOURCE_READER {}".format(fqname) not in contents
+        or "FORMAT_NAME {}".format(fqname) not in contents
+    ):
+        raise ValueError("SOURCE_READER and FORMAT_NAME must be '{}'".format(fqname))
+
+
+def check_formatinfo(package_metadata, format_metadata, db_path):
+    """
+    Checks formatinfo is consistent with the package and format metadata.
+
+    :param package_metadata: The package metadata.
+    :param format_metadata: The format metadata.
+    :param db_path: The path to the format file.
+    """
+    line = None
+    with open(db_path) as inf:
+        for line in inf:
+            if line.startswith(";"):
+                continue  # comment line.
+
+    if not line:
+        raise ValueError("{} empty".format(db_path))
+
+    fqname = fq_format_short_name(
+        package_metadata.publisher_uid, package_metadata.uid, format_metadata.name
+    )
+
+    formatinfo = parse_formatinfo(line)
+    if formatinfo.FORMAT_NAME != fqname:
+        raise ValueError("{} must have FORMAT_NAME of '{}'".format(db_path, fqname))
+
+
+class FMEPackager:
+    def __init__(self, src_dir, verbose=True):
+        """
+        :param src_dir: FME package directory
+        :param verbose: If true, print out build steps
+        """
+        self.src_dir = Path(src_dir)
+        self.build_dir = self.src_dir / "build"
+        self.dist_dir = self.src_dir / "dist"
+        self.src_python_dir = self.src_dir / "python"
+
+        self.metadata = load_fpkg_metadata(src_dir)
+        self.verbose = verbose
+
+        validate(self.metadata.dict, load_metadata_json_schema())
+
+    def apply_help(self, help_src):
+        """
+        Import an Safe TechPubs doc export into an FME Package directory.
+
+        :param help_src: Help source path.
+        """
+        tmp_doc_dir = tempfile.mkdtemp(prefix="fme-packager_")
+        try:
+            # If help source is a ZIP, extract it to a temporary folder.
+            if os.path.isfile(help_src):
+                with zipfile.ZipFile(help_src) as zipf:
+                    self._print("Extracting {} to {}".format(help_src, tmp_doc_dir))
+                    zipf.extractall(tmp_doc_dir)
+                root_contents = os.listdir(tmp_doc_dir)
+                # If help ZIP started with a single root level folder, then unnest.
+                if len(root_contents) == 1:
+                    nested_dir = os.path.join(tmp_doc_dir, root_contents[0])
+                    self._print("Flattening single top-level folder {}".format(nested_dir))
+                    for item in os.listdir(nested_dir):
+                        shutil.move(os.path.join(nested_dir, item), tmp_doc_dir)
+                    os.rmdir(nested_dir)
+                help_src = tmp_doc_dir
+
+            # Parse flali file ahead of anything else.
+            flali_path = os.path.join(help_src, "package_aliases.flali")
+            with open(flali_path, encoding="utf-8") as xmlin:
+                aliases_xml = xmltodict.parse(xmlin.read())
+
+            embedded_doc_dirs = list(filter(lambda x: x.startswith("!"), os.listdir(help_src)))
+            if embedded_doc_dirs:
+                warnings.warn(
+                    "{} embedded doc folders (starting with '!'). Avoid these if possible".format(
+                        len(embedded_doc_dirs)
+                    )
+                )
+
+            # (Re)create destination help folder and copy over the bulk of the doc files.
+            dest = os.path.join(self.src_dir, "help")
+            if os.path.exists(dest):
+                self._print("Deleting {}".format(dest))
+                shutil.rmtree(dest)
+            shutil.copytree(help_src, dest, ignore=shutil.ignore_patterns(*TREE_COPY_IGNORE_GLOBS))
+        finally:
+            shutil.rmtree(tmp_doc_dir)
+
+        # Convert flali to CSV and put it in the destination.
+        # Skip rows that refer to doc files that aren't present in the doc ZIP.
+        copied_rows = 0
+        with open(os.path.join(dest, "package_help.csv"), "w", newline="") as csvout:
+            writer = csv.writer(csvout)
+            rows = aliases_xml["CatapultAliasFile"]["Map"]
+            if not isinstance(rows, list):
+                rows = [rows]
+            for row in rows:
+                name = row["@Name"].replace(".", "_")
+                link = row["@Link"]
+                if link.startswith("/Content"):
+                    new_link = link.replace("/Content", "", 1)
+                    link = new_link
+                expected_doc_path = os.path.join(dest, link.lstrip("/"))
+                if os.path.exists(expected_doc_path):
+                    self._print("{} exists".format(expected_doc_path))
+                    writer.writerow([name, link])
+                    copied_rows += 1
+        self._print(
+            "Wrote {} of {} flali row(s) to package_help.csv".format(copied_rows, len(rows))
+        )
+        if not copied_rows:
+            raise ValueError("flali doesn't reference any included doc")
+
+    def make_fpkg(self):
+        """
+        Create an .fpkg file from package build files.
+        """
+
+        if not self.dist_dir.exists():
+            self.dist_dir.mkdir(parents=True)
+
+        fpkg_filename = build_fpkg_filename(
+            self.metadata.publisher_uid, self.metadata.uid, self.metadata.version
+        )
+        fpkg_path = self.dist_dir / fpkg_filename
+        self._print(f"Saving fpkg to {fpkg_path}")
+
+        if fpkg_path.exists():
+            fpkg_path.unlink()
+
+        new_zip = shutil.make_archive(fpkg_path, "zip", root_dir=self.build_dir)
+        Path(new_zip).rename(fpkg_path)  # Strip zip extension
+        self._print("Done.")
+
+    def build(self):
+        """
+        Build and validate package files.
+        """
+        self._print("Collecting files into {}".format(self.build_dir))
+
+        # Clear out the build dir.
+        if os.path.exists(self.build_dir):
+            shutil.rmtree(self.build_dir)
+        self.build_dir.mkdir(parents=True)
+
+        for required_file in ["package.yml", "README.md", "CHANGES.md"]:
+            check_exists_and_copy(self.src_dir / required_file, self.build_dir)
+
+        self._copy_icon()
+
+        self._copy_transformers()
+        self._copy_web_services()
+        self._copy_web_filesystems()
+        self._copy_formats()
+        self._copy_localization()
+        self._copy_help()
+
+        self._build_wheels()
+        self._copy_wheels()
+        self._check_wheels()
+
+    def _copy_formats(self):
+        # First, copy all files we don't specifically care about.
+        # Ignore FMF and etc for formats not mentioned in metadata.
+        src = self.src_dir / "formats"
+        dst = self.build_dir / "formats"
+        if src.is_dir():
+            shutil.copytree(src, dst, ignore=shutil.ignore_patterns(*TREE_COPY_IGNORE_GLOBS))
+
+        for fmt in self.metadata.formats:
+            self._print(f"Working on format: {fmt.name}")
+
+            if not (dst / f"{fmt.name}.md").is_file():
+                raise ValueError(f"{fmt.name} is missing doc")
+
+            fms_path = src / f"{fmt.name}.fms"
+            if fms_path.is_file():
+                shutil.copy(fms_path, dst)
+
+            fmf_path = src / f"{fmt.name}.fmf"
+            if not fmf_path.is_file():
+                raise ValueError(f"{fmf_path} is in metadata, but was not found")
+            check_fmf(self.metadata, fmt, fmf_path)
+            shutil.copy(fmf_path, dst)
+
+            db_path = src / f"{fmt.name}.db"
+            if not db_path.is_file():
+                raise ValueError(f"{db_path} is in metadata, but was not found")
+            check_formatinfo(self.metadata, fmt, db_path)
+            shutil.copy(db_path, dst)
+
+    def validate_transformer(self, transformer_path, expected_metadata: TransformerMetadata):
+        self._print(f"Checking {transformer_path}")
+        transformer_file = load_transformer(transformer_path)
+
+        expected_fqname = "{}.{}.{}".format(
+            self.metadata.publisher_uid, self.metadata.uid, expected_metadata.name
+        )
+
+        transformer_versions = list(transformer_file.versions())
+        if not transformer_versions:
+            raise ValueError(f"{transformer_path} defines no versions")
+        # Validations below apply to all versions of the transformer
+        for transformer in transformer_versions:
+            if transformer.version < 1:
+                raise ValueError(f"Invalid transformer version {transformer.version}")
+            if transformer.name != expected_fqname:
+                raise ValueError(f"Name must be '{expected_fqname}', not '{transformer.name}'")
+            if isinstance(transformer, CustomTransformer):
+                if transformer.header.insert_mode != '"Linked Always"':
+                    raise ValueError(
+                        f'Custom transformer Insert Mode must be "Linked Always", not {transformer.header.insert_mode}'
+                    )
+                if transformer.header.build_num < self.metadata.minimum_fme_build:
+                    raise ValueError(
+                        "Custom transformer created with FME build older than fme_minimum_build in package.yml"
+                    )
+
+        # Validations below apply only to the latest version of the transformer
+        latest = transformer_versions[0]  # First definition in file
+        if latest.version != expected_metadata.version:
+            raise ValueError(f"Missing version {expected_metadata.version}")
+        if not latest.python_compatibility and self.metadata.minimum_fme_build < 23000:
+            raise ValueError("Python Compatibility setting required when minimum_fme_build < 23000")
+        elif latest.python_compatibility and not is_valid_python_compatibility(
+            latest.python_compatibility
+        ):
+            if not isinstance(latest, CustomTransformer):
+                raise TransformerPythonCompatError(expected_metadata.name)
+            elif isinstance(latest, CustomTransformer) and latest.python_compatibility != "2or3":
+                raise CustomTransformerPythonCompatError(expected_metadata.name)
+
+    def _copy_transformers(self):
+        # First, copy all files we don't specifically care about.
+        # Ignore FMX and FMS for transformers not mentioned in metadata.
+        src = self.src_dir / "transformers"
+        dst = self.build_dir / "transformers"
+        if src.is_dir():
+            shutil.copytree(src, dst, ignore=shutil.ignore_patterns(*TREE_COPY_IGNORE_GLOBS))
+
+        for transformer in self.metadata.transformers:
+            self._print(f"Working on transformer: {transformer.name}")
+
+            if transformer.version < 1:
+                raise ValueError(f"{transformer.name} version must be >= 1")
+
+            if not (dst / f"{transformer.name}.md").is_file():
+                raise ValueError(f"{transformer.name} is missing doc")
+
+            fms_path = src / f"{transformer.name}.fms"
+            if fms_path.is_file():
+                shutil.copy(fms_path, dst)
+
+            fmx_path = src / f"{transformer.name}.fmx"
+            fmxj_path = src / f"{transformer.name}.fmxj"
+            if fmx_path.is_file() and fmxj_path.is_file():
+                raise ValueError(f"{transformer.name} cannot have both FMX and FMXJ")
+            if not fmx_path.is_file() and not fmxj_path.is_file():
+                raise ValueError(f"{fmx_path} is in metadata, but was not found")
+            transformer_path = fmx_path if fmx_path.is_file() else fmxj_path
+            if transformer_path == fmxj_path and self.metadata.minimum_fme_build < 23146:
+                raise ValueError("FMXJ requires minimum_fme_build >= 23146")
+
+            # Copy file if it passed validation
+            self.validate_transformer(transformer_path, transformer)
+            shutil.copy(transformer_path, dst)
+
+    def _copy_web_services(self):
+        dest = self.build_dir / "web_services"
+        for web_service in self.metadata.web_services:
+            # fpkg spec says web service metadata entries must be full filename. Don't assume xml.
+            definition_path = self.src_dir / "web_services" / web_service.name
+            if not definition_path.exists():
+                raise ValueError(
+                    f"Web Service '{web_service.name}' is in metadata, but was not found"
+                )
+            if not dest.exists():
+                dest.mkdir(parents=True)
+
+            # TODO: Validate contents of XML.
+            self._print(f"Copying Web Service: {definition_path.name}")
+            shutil.copy(definition_path, dest)
+
+    def _copy_web_filesystems(self):
+        src = self.src_dir / "web_filesystems"
+        dest = self.build_dir / "web_filesystems"
+        for web_filesystem in self.metadata.web_filesystems:
+            definition_path = src / f"{web_filesystem.name}.fme"
+            if not definition_path.is_file():
+                raise ValueError(
+                    f"Web Filesystem '{web_filesystem.name}' is in metadata, but was not found"
+                )
+            if not dest.exists():
+                dest.mkdir(parents=True)
+
+            # TODO: Validate contents of .fme file.
+            self._print(f"Copying Web Filesystem: {definition_path.name}")
+            shutil.copy(definition_path, dest)
+
+            icon_path = src / f"{web_filesystem.name}.png"
+            if icon_path.is_file():
+                enforce_png(icon_path)
+                # Specification doesn't say anything about dimensions.
+                shutil.copy(icon_path, dest)
+
+    def _copy_icon(self):
+        path = self.src_dir / "icon.png"
+        if not path.is_file():
+            self._print("FME package has no icon")
+            return
+        enforce_png(path, min_width=200, min_height=200, square=True)
+        self._print("Icon is OK")
+        shutil.copy(path, self.build_dir)
+
+    def _build_wheels(self):
+        original_cwd = os.getcwd()
+
+        if not self.src_python_dir.exists():
+            return
+
+        for path in self.src_python_dir.iterdir():
+            if (path / "setup.py").is_file() or (path / "setup.cfg").is_file():
+                self._print(f"\nBuilding Python wheel: {path}")
+                os.chdir(path)
+                if os.path.exists("build"):
+                    shutil.rmtree("build")
+                # Simple solution to avoid needing to figure out which output is the one we want.
+                # The only wheel in the directory will be the one to include in the fpkg.
+                if os.path.exists("dist"):
+                    shutil.rmtree("dist")
+                try:
+                    ProjectBuilder(".").build("wheel", "dist")
+                finally:
+                    os.chdir(original_cwd)
+
+    def _copy_wheels(self):
+        if not self.src_python_dir.is_dir():
+            return
+
+        wheels_dest = self.build_dir / "python"
+        wheels_dest.mkdir(parents=True)
+
+        for path in self.src_python_dir.iterdir():
+            if os.path.isfile(path) and path.suffix == ".whl":
+                shutil.copy(path, wheels_dest)
+
+            built_wheels_dir = path / "dist"
+            if built_wheels_dir.is_dir():
+                built_wheels_for_lib = [
+                    name for name in built_wheels_dir.iterdir() if name.suffix == ".whl"
+                ]
+                assert len(built_wheels_for_lib) == 1
+                shutil.copy(built_wheels_for_lib[0], wheels_dest)
+
+    def _check_wheels(self):
+        wheels_path = self.build_dir / "python"
+
+        wheel_names = os.listdir(wheels_path) if wheels_path.is_dir() else []
+        for expected_py_package in self.metadata.python_packages:
+            lib_name = expected_py_package.name
+            if not any(
+                wheel_name.startswith(lib_name) or wheel_name.startswith(lib_name.replace("-", "_"))
+                for wheel_name in wheel_names
+            ):
+                raise ValueError(f"Python library '{lib_name}' is in metadata, but was not found")
+
+        if not wheels_path.is_dir():
+            return
+        for wheel_path in wheels_path.iterdir():
+            wheel_name = wheel_path.name
+            if "py3" not in wheel_name:
+                warnings.warn("{} is not a Python 3 wheel".format(wheel_name))
+            if not wheel_name.endswith("-none-any.whl"):
+                warnings.warn("{} is not a pure-Python wheel".format(wheel_name))
+
+    def _copy_localization(self):
+        # Copy any optional localization files. The only sanity check is a filename whitelist:
+        # guiprompts_??.txt, transformer-localized.??, FormatOrTransformerName_??.md
+        # ?? is a 2-letter language code.
+        # Contents of files aren't validated. It's up to Workbench to ignore anything malformed.
+        dest = self.build_dir / "localization"
+        src = self.src_dir / "localization"
+        if not src.is_dir():
+            return
+
+        keywords = [f.name for f in self.metadata.formats] + [
+            t.name for t in self.metadata.transformers
+        ]
+        localized_doc_globs = [keyword + "_??.md" for keyword in keywords]
+
+        for name in os.listdir(src):
+            path = src / name
+            if (
+                fnmatch(name, "guiprompts_??.txt")
+                or fnmatch(name, "transformer-localized.??")
+                or any(fnmatch(name, glob) for glob in localized_doc_globs)
+            ):
+                if not os.path.exists(dest):
+                    os.makedirs(dest)
+                self._print(f"Copying localization: {name}")
+                shutil.copy(path, dest)
+
+    def _copy_help(self):
+        src = self.src_dir / "help"
+        dest = self.build_dir / "help"
+        if not src.is_dir():
+            return
+
+        self._print("Copying help")
+        builder = HelpBuilder(self.metadata, src, dest)
+        builder.build()
+
+    def _print(self, msg):
+        if self.verbose:
+            print(msg)
```

## Comparing `fme_packager-1.3.1.dist-info/LICENSE` & `fme_packager-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fme_packager-1.3.1.dist-info/METADATA` & `fme_packager-1.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fme-packager
-Version: 1.3.1
+Version: 1.4.0
 Summary: Tool for creating FME Packages.
 Home-page: https://github.com/safesoftware/fme-packager
 Author: Safe Software Inc.
 License: BSD
 Keywords: FME fmeobjects
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```


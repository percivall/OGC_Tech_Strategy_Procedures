# OGC Technology Strategy Procedures
This is a template proposed for Testbed-14 Engineering Reports.  The objective is for editors to check this out (Clone a version) and begin editing it with a tool such as e.g. Atom editor and Asciidoctor conversion tool.

Note that the files index.adoc, 0-preface.adoc, asciidoctor.css, and all files in folder _resources_ should not be modified. Please begin with file er.adoc. The file er.adoc has instructions in the form of comment. These don't need to be removed. Other files have helper texts that provide instructions.

It is very important that the names of the file er.adoc will not be changed, as the scripts to mass-convert all ERs fail! Ideally, you only name

* er.adoc
  * preface.adoc (don't change this)
  * 1-summary.adoc
  * 2-references.adoc
  * 3-terms.adoc
  * 4-overview.adoc
  * 5-example.adoc (some asciidoc syntax help. Use as many copies as you need sections in your document)

  * annex-a.adoc  --|
  * annex-b.adoc    |-- Use as needed
  * annex-c.adoc  --|

  * annex-history.adoc
  * annex-bibliography.adoc

=============
I have found the following User Guide very helpful:  http://www.methods.co.nz/asciidoc/userguide.html

# How to compile your raw files
Command for PDF output:
asciidoctor-pdf -a pdf-stylesdir=resources -a pdf-style=ogc -a pdf-fontsdir=resources/fonts cfp.adoc

Command for HTML output:
asciidoctor -a stylesheet=rocket-panda.css -a stylesdir=./resources/stylesheets cfp.adoc

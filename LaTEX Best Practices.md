LaTeX Best Practices
=======================

This document intends to serve as a list of best practices and guidance to write scientific papers (and my thesis) using LaTeX. The rules are gathered either by experience, online search and most importantly the wisdom of my PhD supervisor [@Raphael Troncy](https://twitter.com/rtroncy).

## General Organizations

- Create a structure to include your papers in an organized fashion. I keep spearate folders for `papers`, `posters`, `presentations`, `reports` and `thesis`. **Note**: Demo and reseach paper are included in the same folder, you can decide to have posters and demo in the same folder. It is up to you.
- To easily navigate through papers, it is good to have a separate folder for each conference (if you a large number of papers, and then from there you have another hierarchy with the year) but for me it is a flat strucutre inside each folder with a naming conveention that follows `<Conference>'<Year> - <Paper Name>`.
- Keep a `util` folder in the root. This will help misc files that you need globally. For me, i have a `LaTeX` folder inside that includes all the document classes that i use across my papers. I then reference the class using relative path. This way, you will need to maintain different copies of the same files in each paper's folder.

## Environment Setup

- I cannot stress enough on the importance of using a versioning system like `[git](http://git-scm.com/)` or `[svn](https://subversion.apache.org/)`. It is vital for collaborative authoring.
- My development machine is a Mac runnig OSX Yosemite. I use [MacTEX](https://tug.org/mactex/). MacTex is an all-in-one package installing the following:
    + GUI Applications: [TeXShop](http://www.uoregon.edu/~koch/texshop/texshop.html) , [BibDesk](http://bibdesk.sourceforge.net/), [LaTeXiT](http://ktd.club.fr/programmation/latexit_en.php), [TeX Live Utility](https://code.google.com/p/mactlmgr/), the spell checker [Excalibur](http://excalibur.sourceforge.net/), and some documentation
    + Ghostscript 9.10
    + TeX Live 2014, the actual TeX distribution

### Generating LaTeX Tables

-  A nice program that provides a GUI for various tasks is Lyx. I have not used it for Mac but it was useful when editing/creating tables on Windows. It can import data in `.csv` format and generate `.tex` code from it.
-  There is several online `.tex` generators. I use [the online LaTeX table generatorr](http://www.tablesgenerator.com/), and found it very useful for small/medium tables.
-  There is a handy Excel script to convert tables in Excel files to LaTeX. You can find it in `Util/Excel To LaTeX Table Converter.xla`

### Editing LaTeX with Sublime Text

I use [Sublime Text](https://www.sublimetext.com/) for nearly everything, so using it to write LaTeX was the logical choice for me. With the correct plugins it is a handy editor. You first need to make sure you have a valid TeX distribution (see above) and installed [Skim PDF Viewer](http://skim-app.sourceforge.net/). Skim is used to generate the result of the LaTeX build.

Assuming you already have [package control installed](https://packagecontrol.io/installation) install the `[LaTeX Tools](https://github.com/SublimeText/LaTeXTools)` package. Now, after editing a LaTeX document, simply hit `cmd+b` to build the file and launch it in Skim.

**Note** Make sure you have the build settings in Sublime Text set to automatic `[tools -> Build Systems]`.








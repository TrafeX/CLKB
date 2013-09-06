Command Line Knowledge Base
===========================
A command line app to manage knowledge base snippets, nifty one-liners and everything you simply want to store by using the command line.
When you create a new item your favorite CLI-editor pops up and lets you add the content. When you close the editor you'll be aked for a short description and optionally some tags to quickly find it back.

Master branch: [![Build Status](https://travis-ci.org/TrafeX/CLKB.png?branch=master)](https://travis-ci.org/TrafeX/CLKB)

Develop branch: [![Build Status](https://travis-ci.org/TrafeX/CLKB.png?branch=develop)](https://travis-ci.org/TrafeX/CLKB)

Install
=======
You want to use this app? You can!

Debian/Ubuntu
-------------
Follow these steps:

1. Make sure you have python and python-dateutil installed (apt-get install python python-dateutil)
2. Download the latest Debian package here: <http://www.trafex.nl/command-line-knowledge-base>
3. Install with dpkg -i clkb_*.deb
4. Type clkb --help or see below for how to use

Redhat/Fedora/CentOS:
-------------
Follow these steps:

1. Make sure you have python, python-dateutil and sqlite installed (yum install python python-dateutil sqlite)
2. Download the latest tag here <https://github.com/TrafeX/CLKB/tags>
3. Unpack the file and copy clkb to /usr/local/bin/
4. Type clkb --help or see below for how to use

Usage
=====

<pre>
Usage: clkb [options]

clkb - Command Line Knowledge Base

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -c, --create          create a new item
  -e ID, --edit=ID      edit a item
  -d ID, --delete=ID    delete a item
  -s QUERY, --search=QUERY
                        search items
  -i ID, --item=ID      show the item

  List/search options:
    These options can be used when searching or listing the items

    -l LIMIT, --limit=LIMIT
                        limit the listing to [LIMIT] items (default 50)
    --hide-content      hides the content in the listing
</pre>

Work in progress
================
This tool is still in progress. If you want a feature to be added, please let me know or send a pull request.

TODO
----
    [ ] Better error handling
    [X] Scale the width on tiny screens
    [X] Maybe a sort of syntax highlighting
    [ ] Add the option to store the DB on a other location
    [ ] Write a unit test
    
    
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/TrafeX/CLKB/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

Command Line Knowledge Base
===========================
A command line app to manage knowledge-base snippets, nifty one-liners and everything you simply want to store by using the command line.
When you create a new item your favorite CLI-editor pops up and lets you add the content. When you close the editor you'll be aked for a short description and optionally some tags to quickly find it back.


Copyright (c) 2012, Tim de Pater <code@trafex.nl>


Install
=======
You want to use this app? If you are on debian/ubuntu, you can!
Follow these steps:

1. Make sure you have python and python-dateutil installed (apt-get install python python-dateutil)
2. Download the latest version here: <https://github.com/downloads/TrafeX/CLKB/clkb_1.0.0-1_all.deb>
3. Install with dpkg -i clkb_*.deb
4. Typ clkb --help or see below for how to use

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
    [X] Fix the timezone for the add- and moddate
    [ ] Better error handling
    [ ] Scale the width on tiny screens
    [X] Cutoff long content
    [X] Add action to show detail
    [ ] Maybe a sort of syntax highlighting
    [X] Add argument to hide content in listing
    [X] Create a .deb package
    [ ] Add the option to store the DB on a other location

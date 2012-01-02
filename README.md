Command Line Knowledge Base
===========================
A command line app to manage knowledge-base snippets, nifty one-liners and everything you simply want to store by using the command line.
When you create a new item your favorite CLI-editor pops up and lets you add the content. When you close the editor you'll be aked for a short description and optionally some tags to quickly find it back.


Copyright (c) 2012, Tim de Pater <code@trafex.nl>


Install
=======
You want to use this app? Then follow these steps:

1. Download the latest version here: <https://github.com/TrafeX/CLKB/tags>
2. Copy the clkb file to /usr/local/bin
3. Typ clkb --help or see below for usage information


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
    [ ] Create a .deb package

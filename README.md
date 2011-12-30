Command Line Knowledge Base
====
A python app to simply create/edit/delete knowledge base snippets, nifty one-liners and all other stuff you want to store simply by using the command line.

Help
====
<pre>
Usage: clkb [options]

CLKB - Command Line Knowledge Base

Options:
    --version             show program's version number and exit
    -h, --help            show this help message and exit
    -c, --create          create a new item
    -e ID, --edit=ID      edit a item
    -d ID, --delete=ID    delete a item
    -s QUERY, --search=QUERY
                        search items
</pre>

Work in progress
====
This tool is still work in progress. If you want a feature to be added, please let me know or send a pull request.

TODO
======
    [ ] Fix the timezone for the add- and moddate
    [ ] Better error handling
    [ ] Scale the width on tiny screens
    [ ] Cutoff long content and implement a detail action

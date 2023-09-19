## TODO

1. make bkms2 app => a node.js app, in Typescript (i.e. bunch of TS scripts that can be run via npm) that:
   -- breaks the bookmarks into a set of classifications
   ---- removes any duplicates that currently exist (a duplicate is defined as the $BKMK_URL being the same for two or more bookmarks)
   -- renders README.md files in a folder structure that resembles the classifications
   ---- each classification README.md will essentially list all the bookmarks for that specific classification
   -- generates a bookmarks.html file that concatenates all the classifications allowing for easy import into a browser like Chrome, Edge, Brave Browser, or Firefox
   -- adds new bookmarks through a:
   ---- CLI command (i.e. npm add $CLASSIFICATION $BKMK_URL $BKMK_NAME)
   ---- JSON file
   ---- XML file
   ---- bookmarks.html file
   ---- CSV file
   ---- does a check to see if the bookmark already exists by comparing $BKMK_URL
   -- will utilize the emd-logger-typescript module

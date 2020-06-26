*Commands and tricks for Virtoso server*

## Nice iSQL commands\
When deleting large graphs, first change logging\
`log_enable(3,1);`
Then clear graph with\
`SPARQL CLEAR GRAPH  <graph-name>;`\

Always remember to run the loader and create checkpoint after insertion and deletion\
`rdf_loader_run ();`
`checkpoint;`


Insert graph\
Use the following format from iSQL\
`ld_dir ('/import', 'file-name.ttl', 'http://graph-name');`
where `/import` is the location of the file `file-name.ttl`. 
Remember to run loader and checkpoint after this.

## Tricks
Delete all graphs\
First stop Virtuoso, then enter /database and delete all files, except for the .ini file.
Now start Virtuoso again, and the all graphs are deleted.
Files in this folder:

## coherence-cluster-gc-profile.xml
A workspace for displaying coherence storage node GC profiles. Requries `hotspot-datatype.xml` and relies 
on storage enabled nodes having a role of 'cachenode', though this can easily be changed.

## hotspot-datatype.xml
A data type for intepretting hotspot GC logs.
the datatype relies on a naming convention of the gc logs. It expects gc logs to be named: `gc_<role>_.*`, 
where <role> is taken to be the role of the process within the application e.g. cachenode, app_server, etc.


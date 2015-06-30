Files in this folder:

## coherence-cluster-gc-profile.xml
A workspace for displaying coherence storage node GC profiles. Requries `hotspot-datatype.xml` and relies 
on storage enabled nodes having a role of 'cachenode', though this can easily be changed.

## hotspot-datatype.xml
A data type for intepretting hotspot GC logs.

The datatype relies on a naming convention of the gc logs:
* It expects gc log file name to match the regular expression `.*?_(.*?)_.*`, where the capture group is the role of the process within the application. The `coherence-clsuter-gc-profile.xml` workspace requires storage enabled cluster members to have the role 'cachenode', though this can of course be tweaked if needed.
* It expects the gc log to have a full path that matches the regular expression `.*/work/(.*?)/.*`, where the capture group is the 'engine name' - a unique name for the node. In the system this was written for this was the machine name plus a slot number, (as multiple processes are running on the same server). You will need to tweak this to match your own environment and setup.




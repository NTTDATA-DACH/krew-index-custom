# krew-index-custom

Plugin index for https://github.com/kubernetes-sigs/krew. This repo is for NTT DATA custom plugin maintainers.

## List of kubectl plugins listed in this index

* [viewnode](https://github.com/NTTDATA-DACH/viewnode)

## Using as custom krew-index

Adding this index as a custom one

```console
$ kubectl krew index add nttdata https://github.com/NTTDATA-DACH/krew-index-custom.git
WARNING: You have added a new index from "https://github.com/NTTDATA-DACH/krew-index-custom.git"
The plugins in this index are not audited for security by the Krew maintainers.
Install them at your own risk.
```

Listing indexes

```console
$ kubectl krew index list
default  https://github.com/kubernetes-sigs/krew-index.git
nttdata  https://github.com/NTTDATA-DACH/krew-index-custom.git
```

Adding a plugin from this index repository

```console
$ kubectl krew install nttdata/viewnode
Updated the local copy of plugin index.
Updated the local copy of plugin index "nttdata".
Installing plugin: viewnode
Installed plugin: viewnode
\
 | Use this plugin:
 | 	kubectl viewnode
 | Documentation:
 | 	https://github.com/NTTDATA-DACH/viewnode
/
```

# rsync

### Only copy new files

```
rsync -av --update source_dir dest_dir
```

Options:
* a - archive mode; equals -rlptgoD (no -H,-A,-X)
* v - increase verbosity
* update - skip files that are newer on the receiver

### Copy files with progress and log

```
rsync -arv source_dir dest_dir --progress | tee backup.log
```

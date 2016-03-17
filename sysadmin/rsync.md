# rsync

### Only copy new files

```
rsync -av --update source_dir dest_dir
```

Options:
* a - archive mode; equals -rlptgoD (no -H,-A,-X)
* v - increase verbosity
* update - skip files that are newer on the receiver

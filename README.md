# Workstation Housekeeping

Utilities for managing data on the local NGS workstation

## Reference
* [wscleaner](wscleaner/README.md)
* [backup_runfolder.py](backup_runfolder.py)
* [findfastqs.sh](findfastqs.sh)

<br>

---

## [wscleaner](wscleaner/README.md)

Clear NGS runfolders that are backed up in DNANexus.

```bash
wscleaner --set-key DNA_NEXUS_KEY # Cache dnanexus api key
wscleaner ROOT_DIRECTORY --logfile LOGFILE_PATH
```

---

## [backup_runfolder.py](backup_runfolder.py)

Upload a directory to a DNANexus project.

```bash
backup_runfolder.py [-h] -i RUNFOLDER [-a AUTH_TOKEN] [--ignore IGNORE] [-p PROJECT] [--logpath LOGPATH]
```

---

## [findfastqs.sh](findfastqs.sh)

Report the number of gzipped fastq files in an directory.

```bash
$ findfastqs.sh RUNFOLDER
>>> RUNFOLDER has 156 demultiplexed fastq files with 2 undetermined. Total: 158
```

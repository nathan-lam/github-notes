---
tags:
  - Guides/Workflows
---

# Goal
To copy my data from one drive to another using [[rsync]]


# Steps

## Overwriting
This process is slow and should only be done occasionally

1. cd into the harddrive
2. run the following command
	1. ```rsync -av --delete /home/user_name/DATAHOARD/ ./```


## Adding diffs
This is faster as it assumes the contents are the same but with some differences


# Notes

The command uses rsync to copy over an existing directory into the harddrive


## Command Breakdown

```
rsync
	The tool used to copy over files
-av
	a = archive
	v = verbose, print out processing text
--delete
	Delete files in favor of new files
	Otherwise files will only be added to
/home/user_name/DATAHOARD/
	The directory to copy data from
./
	The directory to copy data to
	Because we cd into the harddrive, we just say to use teh current directory
```



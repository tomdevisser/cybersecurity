# Commands

## Quick reference

`echo`, output any text
`whoami`, log the current user
`ls`, listing
`cd`, change directory
`cat`, concatenate (read files)
`pwd`, print working directory
`find`, find specific files
`grep`, search the contents of files
`touch`, create a file
`mkdir`, create a directory
`cp`, copy a file or folder
`mv`, move a file or folder
`rm`, remove a file or folder
`file`, determine the filetype
`su`, switch user
`wget`, download files via HTTP
`scp`, transfer files over SSH
`python3 -m http.server`, starting a web server module from Python


### `find`

- Find specific files by filename in every folder in the current directory using `find -name <filename>`
- Use a wildcard to search for anything with a specific extension, like .txt, using `find -name *.txt`

### `grep`

- Find all lines with a specific IP in a log using `grep "<ip>" access.log`

## Operators

`&`, allows you to run commands in the background
`&&`, allows to combine multiple commands
`>`, redirector to direct output of a command elsewhere
`>>`, redirector, but appends the output rather than replacing

## Flags and switches

A majority of commands allow for arguments to be provided, identified by a hyphen and a certain keyword, known as _flags_ or _switches_.

E.g. use `-h` with `ls -lh` to format longer listings in a human readable way.

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


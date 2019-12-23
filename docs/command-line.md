## Command Line

#### Basics
- pwd
  - get present working directory
- ls -Rale@
  - -R recursive
  - -a include dot files
  - -l long format
  - -e Access Control Lists
  - -@ extended attributes
- cd
- open .
  - open in Finder
- history
- clear

#### Files and Directories
- touch [filename]
  - create new file
- mkdir [directory-name]
  - create new directory 
- cp [existing-filename] [new-filename]
  - copy 
- rm [filename]
  - remove file
- rm -r [directory-name]
  - remove directory
- ln -s
  - create sym link

#### Backup
- rsync [source] [destination]
  - -r recursive into directories 
  - -v verbose 
  - -E copy extended attributes 

#### Permisions
- chmod
- chown
- chgrp

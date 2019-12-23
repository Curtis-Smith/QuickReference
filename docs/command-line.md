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
- rsync -avE [source] [destination]
  - -a archive mode; same as -rlptgoD (no -H)
    - -r recurse into directories
    - -l copy symlinks as symlinks
    - -p preserve permisions
    - -t preserve times
    - -g preserve group
    - -o preserve owner
    - -D preserve device files (super-user only), preserve special files
    - (no -H) do not preserve hard links
  - -v verbose 
  - -E copy extended attributes 

#### Permisions
- chmod
- chown
- chgrp

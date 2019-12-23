## git
#### Basics
- git init
  - initialize current directory as a repo
- git init [project-name]
  - create a local repository with directory named [project-name]
- git clone [url]
  - download repository and version history
- git add [file]
- git add .
  - stage file/files
- git commit -m "[commit message]"
  - commit with message
  - -m can be omitted which will open vim for longer message
- git push
- git push [remote] [branch]
  - upload local commits to remote
  - if [branch] does not exist in [remote], [branch] will be created
- git pull
  - download commits from remote
- git branch
  - list branches in repo
- git branch -a
  - list branches (local and remote)
- git branch [branch]
  - create new branch
- git branch -d [branch]
  - delete branch
- git checkout [branch]
  - checkout existing branch
- git checkout -b [branch]
  - create and checkout a new branch named [branch]
- git merge [branch]
  - merge [branch] into current branch
- git status
- git log
- git diff

#### Useful Variations
- git push --set-upstream origin [branch]
- git log --oneline --decorate --graph --all
- git diff <masterbranch_path> <remotebranch_path>
  - may need to fetch first
  - remember to remove "remotes/" from remotebranch

#### .gitignore
- git config --global core.excludesfile
  - look up global exclusion file
- git config --global core.excludesfile [filepath]
  - set global exclusion file
- [github repo](https://github.com/github/gitignore)

#### More Info/Cheat Sheets
- [git-scm](git-scm.com/doc)
- [github](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)
- [github](https://education.github.com/git-cheat-sheet-education.pdf)
- [atlassian](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

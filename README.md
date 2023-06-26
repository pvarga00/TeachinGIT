# Teachin' GIT
## Teaching GIT to peeps

This is a GIT repo showing peeps how to use GIT (remote repos, fetch/merge, etc.)

*Note: Original content by: Jan Kruger and Zack Rusin*


## Common GIT Commands (Cheat Sheet):
### Note: General GIT flow is: Create > Browse > Change (most used) > Revert > Update > Branch > Commit > Push

- **General**:
  - Use git help [command] if you're stuck
  - master/main : default development branch
    - PJV personal note: "master" is being deprecated for D&I reasons... stick to "main" for new repos/branch names going forward
  - origin : default upstream branch
  - HEAD : current branch
  - HEAD^ : parent of HEAD
  - HEAD ~4 : great-great grandparent of HEAD
  - foo..bar : from branch foo to branch bar
  - derp : I'm intentionally doing something silly

- **Create**:
  - From existing files:
    - git init
    - git add .   *(add all files changed)*
  - From existing repository:
    - git clone ~/old ~/new
    - git clone git://...
    - git clone ssh://...
   
- **View**:
  - git status
  - git diff [oldid newid]
  - git log [-p] [*file/dir*]
  - git blame *file*
  - git show *id*   *(metadata & diff)*
  - git branch   *(shows list. * = current)*
  - git tag -l   *(shows list)*
 
- **Revert**:
In GIT revert usually describes a new commit that undoes previous commits
  - git reset --hard **(NO UNDO)**   *(reset to last commit)
  - git revert branch
  - git commit -a --amend   *(replaces previous commit)*
  - git checkout *id file*
 
- **Publish**:
In GIT, commit only respects changes that have been marked explicitly with add.
  - git commit [-a]   *(-a: add changed files automatically)*
  - git format-patch origin
  - pit push *remote*
  - git tag *foo*     *(mark current version)*

- **Update**:
  - git fetch    *(from def. upstream)*
  - git fetch *remote* 
  - git pull   *(== fetch & merge -- basically "get latest")
  - git am -3 patch.mbox
  - git apply patch.diff

- **Branch**:
  - git checkout branch
  - git merge branch
  - git branch branch
  - git checkout -b *new* *other*   *(branch **new** from **other** and switch to it)*

- **Useful Tools**:
  - git archive  *(create release tarball)
  - git bisect  *(binary search for defects)
  - git cherry-pick   *(take a single commit from elsewhere)*
  - git fsck   *(check tree)*
  - git gc  *(compress metadata, for performance)*
  - git rebase
  - git remote add URL
  - git stash
  - git tag
  - gitk

- **Conflicts**:
  - git diff [--base]
  - git diff --ours
  - git diff --theirs
  - git log --merge
  - gitk --merge


- **Tracking Files**:
  - git add files
  - git mv *old new*
  - git rm *files*
  - git rm -- cached *files*   *(stop tracking but keep files in working dir)*




# TeachinGIT
Teaching GIT to peeps

This is a GIT repo showing peeps how to use GIT (remote repos, fetch/merge, etc.)

*Note: Original content by: Jan Kruger and Zack Rusin**


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
    - git add .
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
  - git reset
  - git revert branch
  - git commit -a --amend   *(replaces previous commit)*
  - git checkout *id file*
 
- **Publish**:
  - XXX

- **Update**:
  - XXX

- **Branch**:
  - XXX

- **Useful Tools**:
  - XXX

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






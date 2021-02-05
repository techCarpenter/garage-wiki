# Move Git Repos Script

## Commands

```sh
git remote set-url origin git://new.url.here
git remote remove origin
git push --mirror origin
git remote -v
chmod +x script_one.sh
```

## Script

```sh
#!/usr/bin/bash

curRepo=$1
newRepo=$2

# clone original repo
git clone git@gitlab.com:techCarpenter/$curRepo.git $newRepo

# cd into repo folder
cd $newRepo

# set new origin (gitlab -> github)
git remote set-url origin git@github.com:techCarpenter/$newRepo.git

# show remote repo values
# git remote -v

# push to new remote, (--mirror will keep commit history)
git push --mirror origin

# move up to parent directory
cd ..
```

```sh
# .bash_profile

alias transferrepo="$HOME/bin/transfer-repo.sh"
```

```sh
# example usage

transferrepo landingpage fcc-landing-page
```

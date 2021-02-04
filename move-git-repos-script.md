# Move Git Repos Script

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

```shell
# .bash_profile

alias transferrepo="$HOME/bin/transfer-repo.sh"
```

```shell
# example usage

transferrepo landingpage fcc-landing-page
```

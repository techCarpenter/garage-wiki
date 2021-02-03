# Move Git Repos Script

## Repo mapping

| Github                   | Gitlab                 |
| :----------------------- | :--------------------- |
| topple                   | Debt Paydown App       |
| techcarpenter.org-hugo   | techcarpenter          |
| `techcarpenter.org`      | techcarpenter-gridsome |
| stack-edit-pro-files     | Stack Edit Pro files   |
| `manpoweredtools.com`    | man-powered-tools      |
| leechblock-site-list     | Leechblock Site List   |
| devries-woodworking-site | devrieswoodworking     |
| debt-payment-planner     | Debt Payment Planner   |
| fcc-tribute-page         | tributepage            |
| fcc-technical-document   | technicaldocument      |
| fcc-survey-form          | surveyform             |
| fcc-random-quote-machine | randomquotemachine     |
| fcc-pomodoro-clock       | pomodoroclock          |
| fcc-personal-portfolio   | personalportfolio      |
| fcc-markdown-previewer   | markdownpreviewer      |
| fcc-landing-page         | landingpage            |
| fcc-js-calculator        | jscalculator           |
| fcc-drum-machine         | drummachine            |
| `same`                   | custom_bookmarks       |
| `same`                   | `brianjdevries.com`    |

```shell
git clone git@gitlab.com:techCarpenter/drummachine.git
git clone git@gitlab.com:techCarpenter/markdownpreviewer.git
```

```shell
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

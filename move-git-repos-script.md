# Move Git Repos Script

# Repo mapping

| Transferred | Github                   | Gitlab                 |
| :---------: | :----------------------- | :--------------------- |
|     Yes     | topple                   | Debt Paydown App       |
|     Yes     | techcarpenter.org-hugo   | techcarpenter          |
|     Yes     | techcarpenter.org        | techcarpenter-gridsome |
|     Yes     | stack-edit-pro-files     | Stack Edit Pro files   |
|     Yes     | manpoweredtools.com      | man-powered-tools      |
|     Yes     | leechblock-site-list     | Leechblock Site List   |
|     Yes     | devries-woodworking-site | devrieswoodworking     |
|     Yes     | debt-payment-planner     | Debt Payment Planner   |
|     Yes     | `same`                   | tributepage            |
|     Yes     | `same`                   | technicaldocument      |
|     Yes     | `same`                   | surveyform             |
|     Yes     | `same`                   | randomquotemachine     |
|     Yes     | `same`                   | pomodoroclock          |
|     Yes     | `same`                   | personalportfolio      |
|     Yes     | `same`                   | markdownpreviewer      |
|     Yes     | `same`                   | landingpage            |
|     Yes     | `same`                   | jscalculator           |
|     Yes     | `same`                   | drummachine            |
|     Yes     | `same`                   | custom_bookmarks       |
|     Yes     | `same`                   | brianjdevries.com      |

```shell
git remote set-url origin git@github.com:techCarpenter/fcc-d3-treemap.git
git remote set-url origin git@github.com:techCarpenter/fcc-d3-scatterplot.git
git remote set-url origin git@github.com:techCarpenter/fcc-d3-heatmap.git
git remote set-url origin git@github.com:techCarpenter/fcc-d3-choropleth.git
git remote set-url origin git@github.com:techCarpenter/fcc-d3-bar-chart.git

curRepo=surveyform && \
newRepo=fcc-survey-form && \
echo && \
echo "--- Clone repo ---" && \
echo && \
git clone git@gitlab.com:techCarpenter/$curRepo.git $newRepo && \
echo && \
echo "--- cd into new folder ---" && \
echo && \
cd $newRepo && \
echo "--- Set 'origin' ---" && \
echo && \
git remote set-url origin git@github.com:techCarpenter/$newRepo.git && \
echo "--- show remotes ---" && \
echo && \
git remote -v && \
echo && \
echo "--- Push to new origin ---" && \
echo && \
git push --mirror origin && \
echo && \
echo "--- cd .. ---" && \
cd ..




echo "--- Remove 'github' remote ---" && \
echo && \
git remote remove github && \
echo && \

git clone git@gitlab.com:techCarpenter/landingpage.git && \
git clone git@gitlab.com:techCarpenter/tributepage.git && \
git clone git@gitlab.com:techCarpenter/drummachine.git && \
git clone git@gitlab.com:techCarpenter/markdownpreviewer.git && \
```

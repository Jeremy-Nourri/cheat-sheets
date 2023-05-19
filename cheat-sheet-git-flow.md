## **Cheat sheet Git Flow**
---

Gitflow is an alternative Git branching model that involves the use of feature branches and multiple primary branches.

**The overall flow of Gitflow is:**

* A develop branch is created from main
* A release branch is created from develop
* Feature branches are created from develop
* When a feature is complete it is merged into the develop branch
* When the release branch is done it is merged into develop and main
* If an issue in main is detected a hotfix branch is created from main
* Once the hotfix is complete it is merged to both develop and main
  

| ***Git Flow***                         | ***Git commands***                                         |
|---------------------------------------|------------------------------------------------------|
| Initialize Git Flow                   | `` git flow init ``                                  |
| Create a new feature branch           | `` git flow feature start <feature-name> ``         |
| Finish a feature branch               | `` git flow feature finish <feature-name> ``        |
| Publish a feature branch              | `` git flow feature publish <feature-name> ``       |
| Get a feature branch                  | `` git flow feature pull origin <feature-name> ``   |
| Create a new release branch           | `` git flow release start <release-name> ``         |
| Finish a release branch               | `` git flow release finish <release-name> ``        |
| Publish a release branch              | `` git flow release publish <release-name> ``       |
| Get a release branch                  | `` git flow release pull origin <release-name> ``   |
| Create a new hotfix branch            | `` git flow hotfix start <hotfix-name> ``           |
| Finish a hotfix branch                | `` git flow hotfix finish <hotfix-name> ``          |
| Publish a hotfix branch               | `` git flow hotfix publish <hotfix-name> ``         |
| Get a hotfix branch                   | `` git flow hotfix pull origin <hotfix-name> ``     |


---

**For more explains:**
https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
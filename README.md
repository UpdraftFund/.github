# Git workflow and branching guide

* _[`dev`](#dev) is the branch you will mostly contribute to.  If you're new, please check out [`dev`](#dev) to start working, and make [pull requests](#pull-requests) to the [`dev`](#dev) branch._

## Permanent Branches

### `Master`

`Master` contains tested code that has been [released](#releases) or is about to be released. `master` branch will always reflect what's deployed and used by https://aura.brightid.org .

#### Pull requests

Commits to master should be done through a pull request from [`dev`](#dev) or a [hotfix branch](#hotfix-branches). `dev` branch represents the staging environment. Merging `dev` into `master` represents a release of the staging build to https://aura.brightid.org .

### `Dev`

`Dev` contains code that will probably be ready in time for the next [release](#releases). `Dev` is for testing integrations from feature branches to see if they're ready to be released.

* `Dev` merges into [`master`](#master).
* [`master`](#master) merges into `dev` after [hotfixes](#hotfix-branches).

Because all commits to master come through `dev` or through [hotfixes](#hotfix-branches) that are then merged into `dev`, `dev` should never be behind `master` for long.

## Temporary Branches 

### Feature Branches

Feature branches are created for every new feature. Because multiple features may be worked on at the same time, each feature gets its own temporary branch.

* Feature branches are merged into [`dev`](#dev) when they're ready for integration testing to be able to go out in the next [release](#releases).
* Changes to `dev` can be pulled into a feature branch periodically to make the final merge of the branch smoother.

### Large Update Branches

Large updates that may take longer than a single release cycle use temporary branches that eventually merge into dev. 

* Large Update branches merge into [`dev`](#dev) when they're ready for testing and integration into the next [release](#releases).
* Changes to `dev` can be pulled into a large update branch periodically to make the final merge of the branch smoother.

### Hotfix Branches

Hotfix branches are created as needed. Because multiple hotfixes may be worked on at the same time but finish at different times and need different releases, each hotfix gets its own temporary branch.

* Hotfix branches are merged into [`master`](#master) using a [pull request](#pull-requests).
* [`master`](#master) is then merged in [`dev`](#dev) to bring it up-to-date.
* Hotfix branches should be deleted after being merged.

#### Naming

The name of a hotfix branch should begin with `hotfix` .

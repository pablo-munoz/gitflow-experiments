# Gitflow

The purpose of this repo is so that I learn to use git flow.

# Feature Branches

Feature branches are branches where you do development. This branches
are eventually merged into `develop`. The goal is to accumulate a
number of features (although it could be only one) into a
"development" block to be considered as a candidate for release.

# Release branches

Once the appropiate number of feature branches have been merged onto
develop, a release branch can be created. The release branch is a copy
of the development code frozen at a given point in time. This gives
the ability to test a release (e.g. running on staging servers), while
allowing new features to continue being developed, although this
features will not become part of the release, and will have to wait
for a future release to be included in.

## Fixing mistakes on release branches

To fix a bug or mistake branch, simply correct the release
branch. Once the release branch has been deemed worthy, it is merged
both into master and develop, so both (the clients and the developers)
will get to use the most complete version of the code.

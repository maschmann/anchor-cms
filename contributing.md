# Contributing to Anchor
We're currently in the process of developing `v1.0` but there are still issues to iron out with the existing distro: `v0.9.x`. So we've compiled this short document to help you guys help *us*!

### First

1. Find an [issue](https://github.com/anchorcms/anchor-cms/issues) that needs fixing, or create one if you've got a bug, don't worry, simply making us aware of bugs is a big help!

### Getting Anchor set up locally (If you haven't already)

1. Fork anchor (use the button in the top right of the repo's page).
1. `git clone https://github.com/YOUR-USERNAME/anchor-cms` to get a local copy of your fork.
1. Run `git remote add upstream https://github.com/anchor/anchor-cms`. This will add another remote, named upstream, that points to the official Jeet repository. This will help with keeping your forks up to date with Anchor's master branch.

### Making changes

1. `git checkout -b YourInitials/feature-branch-name` (e.g. `cs/improve-this-feature`, `ma/fix-this-bug`). Make all your changes for the specific feature inside this branch.
1. Separate edits into [clean](https://github.com/erlang/otp/wiki/Writing-good-commit-messages), non-breaking, commits.

### Opening a pull request

1. Push your changes to your fork by running `git push origin your-branch-name`.
1. Open a [pull request](https://help.github.com/articles/creating-a-pull-request), give it a clear title and explain what your changes do. Even provide a code snippet if you can!
1. Be prepared to update your PR based on feedback. If you make updates, run `git push origin your-branch-name -f` on your branch to update the PR on Github.

### Keeping unmerged forks up to date with master

If your fork is taking a while to get merged, you might end up getting behind Anchor's master branch as other changes get added. Stay up to date in the following way:

1. `git fetch upstream master` This will give you all the latest updates from Anchor's master branch.
1. Run `git rebase upstream/master` while inside your feature branch. This will add all the new commits **before** yours, so it's as if you made the changes to the latest codebase.

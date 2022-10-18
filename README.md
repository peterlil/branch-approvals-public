# branch-approvals-public
This repo is created for me to test how it works with protected branches, pull requests and approvals.

## Tests

Testing to check in to main... 
_committing to main_
That worked well.


Adding these branch protection rules:
- pattern: main
- Require a pull request before merging
  - Require approvals
- Do not allow bypassing the above settings

_committing to main_
That didn't work well.
```
remote: error: GH006: Protected branch update failed for refs/heads/main.        
remote: error: At least 1 approving review is required by reviewers with write access.
```

Creating branch _b2_
_committing to b2 and publishing branch_
That worked well.

Creating pull request from _b2_ to _main_

Change in branch new-change-1. 09:07

Change in branch new-change-1. 09:22

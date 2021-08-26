# git-yolo

```
Commits and pushes changes. What could go wrong?

By default, this command runs the following git commands and then opens the
current branch on github.com:

    git add .
    git commit --amend --all --no-edit --no-verify
    git fetch
    git rebase origin/<default-branch>
    git push --force --set-upstream origin HEAD

To install, add this script to your PATH, then run one of the following:

    git config --global alias.yolo '!git-yolo' # All repos
    git config alias.yolo '!git-yolo'          # Current repo only

Usage: git yolo [options]

Options:
    -h                               Print this message (Don't use --help).
    -m, --message MESSAGE            Create a new commit rather than ammending.
    -e, --edit                       Edit commit message.
    -v, --verify                     Run verifications when committing.
    -b, --rebase-branch              Use this branch when rebasing rather than the repo's default branch.
        --no-add                     Don't add.
        --no-fetch                   Don't fetch.
        --no-rebase                  Don't rebase.
        --no-push                    Don't push.
        --no-force                   Don't force push.
        --no-open                    Don't open on GitHub.
```

# ticket-name-commit-msg
Git commit-msg hook to prepend a ticket number for each commit message. This expects a ticket name formatted like so `TIK-1234` in the branch name. If there is no ticket found in the branch name the script will not prepend anything to your commit message.

## Installation
1. update `commit_regex` to match your ticket letter prefix
2. save in a file called `.git/hooks/commit-msg`
3. `chmod 744 .git/hooks/commit-msg` to give it permission to run

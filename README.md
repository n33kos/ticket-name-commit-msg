# ticket-name-commit-msg
Git commit-msg hook to prepend a ticket number for each commit message.

This hook expects a ticket name formatted like so `TIK-1234` in the branch name. If it finds one, it will prepend it to your commit, so the command `git commit -m "Did the thing to the file"` would read `TIK-1234: Did the thing to the file`.

If there is no ticket found in the branch name the script will not prepend anything to your commit message.

## Installation
1. Clone and copy file to `.git/hooks/commit-msg` of your repository.
2. Customize `commit_regex` to match your ticket letter prefix
3. Customize `separator` if you want something instead of `:`
4. `chmod 744 .git/hooks/commit-msg` to give it permission to run

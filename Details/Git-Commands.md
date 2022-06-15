## Study notes of git command

> :eyes: Why we need branch ?
> 
> Branch allows many developers to work in parallel on the same projects simultaneously. 

### 1. Frequently used git commands


| Command | Description |
----------|-------------|
| `git init` | Create an empty Git repository(.git) or reinitialize an existing one. |
| `git clone [HTTPS]`  *(click "Code" button on GitHub to get) <br/> pros: no need to initialize git*| Download an identical copy of the latest version of a project from remote to local workspace.|
| `git add [file-name]` | Add file into index(to be tracked by .git). `-a`: all files; `*.html`: all html files| 
| `git status` | List all new or modified files that haven't yet been committed. |
| `git commit -m"message"` | Save changes ***locally***. |
| `git log` | Display complete details of all commits. `--online -n`: List recent n edit records in one line|
| `git push [remote-name][branch-name]` | Update remote repo with local changes.|
| `git pull [remote-name]` | Update local repo with remote changes. Relevant to git fetch(get updates from remote) + git merge(apply the latest changes to local).|
| `git branch [branch-name]` | Create a branch ***locally***. |
| `git branch --list` | View branches. |
| `git branch -d [branch-name]` | Delete a branch. |
| `git checkout [branch-name]` | Switch to another branch. `-b[branch-name]`: Switch to a new branch right after it has been created |
| `git merge` | Integrate the branch with the parent branch. |


*p.s. [branch-name] represents 7 digits of SHA hash*

*p.s. HEAD represents an indicator to current branch.*

*`-q`  deals with "No next tag (press RETURN)"*

> :eyes: When does conflict happen?
> 
> :eyes: How to fix conflicts?
> 

### 2. CMD
| Command Line | Description|
|--------------|------------|
| cd ../.. | Move up 2 directories |
| [directory path] dir/s | List all files and subdirectories in this directory |

### 3. Shortcuts
**Shift + command + >** &nbsp; -------- &nbsp; Toggle hidden directories(*.git*) or files in Mac OS system  
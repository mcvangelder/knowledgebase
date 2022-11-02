Git aliases offer a way to create short-hand notations or shortcuts to combining git (or any command line) commands


## Useful Aliases
```
co = checkout (checkout a branch)
br = branch (create a branch)
brc = checkout -b (create and checkout branch)
cim = commit -m (create a commit with message)
st = status (check the status of the git repository)
puf = push -f (force push changes to the server)
rbi = rebase -i (start an interactive rebase)
f = fetch (fetch latest details from server)
r = reset (soft reset the branch)
wip = "!git add . && git cim wip" (add all tracked files and create a wip commit)
wipp = "!git wip && git push" (add all tracked files, create a wip commit, and push)
aliases = "!git config --global --get-regexp ^alias.*$" (list global aliases)
```

## Configuration
To apply the aliases to all repository, add the aliases to global git configuration file. This is located in `<user home>/.gitconfig`. Add the following to the file:

```
[alias]
    co = checkout
    br = branch
    brc = checkout -b
    cim = commit -m
    st = status
    puf = push -f
    rbi = rebase -i
    f = fetch
    r = reset
    wip = "!git add . && git cim wip"
    wipp = "!git wip && git push"
    aliases = "!git config --global --get-regexp ^alias.*$"
```

## Usage
`git co <branch name>`
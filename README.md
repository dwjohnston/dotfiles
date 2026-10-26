# dotfiles



## Host Setup 

Add to `.zshrc`/etc   

```bash
PATH_TO_DOTFILES=/Users/davidjohnston/git-workspace/dotfiles
[ -f "$PATH_TO_DOTFILES/aliases" ] && . "$PATH_TO_DOTFILES/aliases"
[ -f "$PATH_TO_DOTFILES/aliases.host" ] && . "$PATH_TO_DOTFILES/aliases.host"
```


## The files 

- **aliases**
     - Shared aliases, whether in a container or not
- **aliases.host**
    - Aliases that only apply on the host
    - Also links `.vscode/*.code-snippets` into VS Code's user snippets folder, so
      snippets like `skill.code-snippets` load in every workspace, not just windows
      that include this repo (a no-op if the file or folder is missing) 


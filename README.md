# gitchecker

Utility to batch checking git repositories for uncommitted files or pending pushes.

It can be useful when switching between computers, to check that all the work has been uploaded.

Usage: gitchecker [-r][-q][-h] \<path\>

By default, gitchecker will check all the folders inside the given path. 

With the -r flag however, all the non-hidden subfolders will be checked. 

Use the -q flag to run quietly, so that only those repositories with uncommitted files or pending pushes will be shown.

For example, you can use 

```bash
gitchecker -rq ~
```

to check all of your repositories that are not inside a hidden folder.

## Installation

sudo wget -O /usr/local/bin/gitchecker https://raw.githubusercontent.com/Pauenmo/gitchecker/refs/heads/main/gitchecker && sudo chmod +x /usr/local/bin/gitchecker

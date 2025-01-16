# gitchecker

Utility for batch checking git repositories for uncommitted files or pending pushes.

It can be useful when switching between computers, to check that all the work has been uploaded.

Usage: gitchecker [-r][-q][-h] \<path\>

By default, only the non-hidden folders at depth 1 inside the given path will be checked. 

With the -r flag however, all the non-hidden subfolders will be checked. 

Use the -q flag to run quietly, so that only those repositories with uncommitted files or pending pushes will be shown.

For example, you can use "gitchecker -rq ~" to quickly check all of the repositories inside your user's home folder (except those that are inside a hidden folder).

## Installation

```bash
sudo wget -O /usr/local/bin/gitchecker https://raw.githubusercontent.com/Pauenmo/gitchecker/refs/heads/main/gitchecker && sudo chmod +x /usr/local/bin/gitchecker
```

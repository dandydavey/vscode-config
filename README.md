# VSCode Configuration files

## Installation instructions (for Linux)

_WARNING_: Following these instructions will overwrite any existing custom settings in your local VSCode installation with the ones in this repo. Copy any existing vscode configs that you want to maintain to this directory before running the commands below.

_Prerequisite_: Set the config directory of your VSCode installation `VSCODE_DIR` or similarly named environment variable. As of Visual Studio v1.52.1, this means:
```
# For Ubuntu
export VSCODE_DIR="$HOME/.config/Code/User/"
# For Mac
export VSCODE_DIR="$HOME/Library/Application\ Support/Code/User/"
```
1. Clone this repo
1. `rsync -a -v -r --ignore-existing $VSCODE_DIR .`
1. `rm -rf $VSCODE_DIR`
1. `ln -s -f -d $(pwd) $VSCODE_DIR`

## Project-specific configurations

Be wary of adding confidential information to this directory. In particular, do not add snippets containing confidential information. Use [Project snippet scope](https://code.visualstudio.com/docs/editor/userdefinedsnippets#_project-snippet-scope) instead.

## Extensions

Note that these settings do not store extensions, so when setting up a new machine, extensions will need to be reinstalled. Some useful extensions include:

- [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
- [Snippet Creator](https://marketplace.visualstudio.com/items?itemName=ryanolsonx.snippet-creator)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)

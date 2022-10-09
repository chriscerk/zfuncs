# zfuncs

my personal zsh functions autoloaded into `~/.zshrc` by adding the following:

```bash
fpath=( $ZFUNC_PATH "${fpath[@]}" )
autoload -U ${fpath[1]}/*(:t);
```

where `$ZFUNC_PATH` is an alias to this repo.

[source: zsh guide](https://zsh.sourceforge.io/Guide/zshguide03.html#l49)

## Current Template

Currently used as a [VS Code Snippet](//.vscode/new-zfunc.code-snippets)

```bash
# ~/zfuncs/my-function
# NAME
# DESCRIPTION
__my-function () {
    echo "NAME: DESCRIPTION";
    echo "-----------";

    # todo: script here

    echo "-----------";
    echo "NAME Complete";
}

__my-function

```
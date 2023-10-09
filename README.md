# Dotfiles

🏠 Personal dotfiles for \*NIX (macOS and Linux) systems.

## Installation

```bash
$ git clone --recursive https://github.com/ppeeou/dotfiles.git ~/.dotfiles
$ cd ~/.dotfiles && python install.py
```

<!--
Note: The option `-j8` (`--jobs 8`) works with Git >= 2.8 (parallel submodule fetching).
For older versions of Git, try without `-j` option.
-->

</p></details>

<br>

The installation script will clone the repository into `~/.dotfiles` and create symbolic links (e.g., `~/.vimrc`) for you.
If target files already exist (e.g. `~/.vim`, `~/.vimrc`), you will need to manually resolve the conflict (delete the old one or just ignore). See Troubleshooting below for details.

## `$ dotfiles`

**To update dotfiles** (pull changes from upstream and run [`install.py`][install.py] again):

```bash
$ dotfiles update
$ dotfiles update --fast          # fast update mode: skip updating {vim,zsh} plugins
```

## License

[The MIT License (MIT)](LICENSE)

Copyright (c) 2012-2023 Jongwook Choi (@wookayin)

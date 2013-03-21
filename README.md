# scottheaberlin’s dotfiles
_shamelessly cloned from [scottheaberlin](https://github.com/scottheaberlin/dotfiles)_
## Installation

### Using Git and the bootstrap script

clone the repository wherever you want.

```bash
git clone https://github.com/scottheaberlin/dotfiles.git && cd dotfiles && source bootstrap.sh
```

To update, `cd` into your local `dotfiles` repository and then:

```bash
source bootstrap.sh
```

Alternatively, to update while avoiding the confirmation prompt:

```bash
set -- -f; source bootstrap.sh
```

### Git-free install

To install these dotfiles without Git:
_TODO_
```bash
cd; curl -#L https://github.com/scottheaberlin/dotfiles/...
```

To update later on, just run that command again.

### Specify the `$PATH`

If `~/.path` exists, it will be sourced along with the other files, before any feature testing takes place.

Here’s an example `~/.path` file that adds `~/utils` to the `$PATH`:

```bash
export PATH="$HOME/utils:$PATH"
```

### Add custom commands without creating a new fork

If `~/.extra` exists, it will be sourced along with the other files. You can use this to add a few custom commands without the need to fork this entire repository, or to add commands you don’t want to commit to a public repository.

### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```
## Thanks to…

* [Mathias Bynens](https://github.com/mathiasbynens/dotfiles) for sharing his dotfiles and readme
* more

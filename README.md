# scottheaberlin’s dotfiles
_shamelessly forked from [mathiasbynens](https://github.com/mathiasbynens/dotfiles)_
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

### Git-free install, take 1

To install these dotfiles without Git:

```bash
cd; curl -#L https://github.com/scottheaberlin/dotfiles/tarball/master | tar -xzv --strip-components 1 --exclude={README.md,bootstrap.sh}
```

To update later on, just run that command again.

### Git-free install, take 2 (Z)

To install theze dotfiles without using Git:

```bash
wget https://github.com/scottheaberlin/dotfiles/tarball/master
mv master scottheaberlin-dotfiles.tgz
tar -zxf scottheaberlin-dotfiles.tgz
cd scottheaberlin-dotfiles<tab>
source bootstrap.sh
```

ignore git errors from the pull

TODO: rsync to multiple servers...

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

...

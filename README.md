# cygpath-for-linux

Lazy implementation of cygpath for linux, for the purpose of making cross-platform bash scripting easier

## downlaod

```
wget -O ~/bin/cygpath https://raw.githubusercontent.com/jstine35/cygpath-for-linux/refs/heads/main/cygpath
chmod +x ~/bin/cygpath
```

## usage

```
usage: cygpath [-a] [-f filename] [FILE]...
```

This tool echos filenames as-is, or converted to absolute pathnames if -a option is given.
Paths are always output as unix-style paths. Cygwin options such as `-w` and `-m` do nothing
since there is no point to convert to windows style paths on unix.

See 'winepath' if converting paths for use in wine.


# winemgr
Simple manager for WINE builds.

## Usage

```
Usage: winemgr <subcommand>

Subcommands:
list [<regex>]             List remote packages matching a regular
                           expression. If no regular expression provided,
                           all results will be listed.
install <package>          Install a package.
remove <package>           Remove a package.
create <prefix> <options>  Same as "prefix create".
run <prefix> <command>     Same as "prefix run".
tricks <prefix> <verbs>    Same as "prefix tricks".
clone <p1> <p2>            Same as "prefix clone".
help                       Display this help message.
```
```
Usage: winemgr prefix <subcommand>

Subcommands:
create <prefix> <options>    Create a WINE prefix using an installed
                             package.
list [<regex>] [<options>]   List prefixes matching regular expressions.
                             used. If no regular expressions provided,
                             all results will be listed.
run <prefix> [<cmd>...]      Run Windows program using a prefix.
tricks <prefix> [<verb>...]  Apply Winetricks on the prefix.
clone <prefix 1> <prefix 2>  Clone a prefix.
remove <prefix>              Remove a prefix.
uninstall <prefix>           Remove a prefix.
help                         Display this help message.

Options:
--package, --pkg, -p         Use a specific package to perform the
                             operation.
```


## Features

- **Manage WINE builds**: fetches WINE builds from [Kron4ek/Wine-Builds](https://github.com/Kron4ek/Wine-Builds).

- **Manage WINE prefixes**: manage WINE prefixes using the correct WINE build.

## Requirements

This script requires GNU bash (>= v4), `jq`, `perl` (including `Text::ASCIITable`) to run.

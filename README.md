cheatsheets-forensic
===========
This repository contains forensic cheatsheets to be used with
[cheat](https://github.com/cheat/cheat) and similar applications.

## How to
cheatsheets are simple text files that can be called and
displayed with the `cheat` command:

```sh
$ cheat mmls
# Display a device or image partition table / layout

mmls /dev/<device>
mmls <image>

# Display a  device or image partition table / layout with a
# column for size

mmls <image> -B
```

## Format 
Cheatsheets are plain-text files that begin with an optional "front matter"
header in YAML format. The header may be used to assign "tags" to a sheet, and
to specify the sheet's syntax (`bash`, `python`, `go`, etc).

When possible, cheatsheets should conform to this format:

```sh
---
syntax: bash
tags: [ sleuthkit ]
---
# To view a device or image partition table / layout

mmls /dev/<device>
mmls <image>

# To view a device or image partition table / layout with a
#    column for size

mmls <image> -B


```

For more information on cheatsheets, see the original project for
[community cheatsheets:](https://github.com/cheat/cheatsheets)



### License ###
Cheatsheets are licensed under [Creative Commons CC0 1.0][cc0]. See
[LICENSE.txt][] for the full license text.


[LICENSE.txt]: https://github.com/cheat/cheatsheets/blob/master/.github/LICENSE.txt
[cc0]: https://creativecommons.org/publicdomain/zero/1.0/legalcode
[cheat]:  https://github.com/cheat/cheat
[docopt]: http://docopt.org

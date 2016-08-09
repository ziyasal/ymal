YMal
============================

_**YMal —** The command line utility for modifiying **YAML** files_

[![Build Status](https://travis-ci.org/ziyasal/ymal.svg?branch=master)](https://travis-ci.org/ziyasal/ymal)
[![Coverage Status](https://coveralls.io/repos/github/ziyasal/ymal/badge.svg?branch=master)](https://coveralls.io/github/ziyasal/ymal?branch=master)
[![npm version](https://badge.fury.io/js/ymal.svg)](https://badge.fury.io/js/ymal)

## Usage

```
  Usage: ymal [options] [command]

  Commands:

    help  Display help

  Options:

    -C, --classes-to-remove          List of classes to remove
    -f, --file                       YAML file path
    -h, --help                       Output usage information
    -P, --pattern-to-remove-classes  Remove classes by pattern o_O!
    -s, --set-value                  Set property value form: `property=value`
    -v, --version                    Output the version number
```

## Sample
```sh
# Removes classes starts with `tst_` and 
# sets `classes.languages::list.perl` property value to `Silver`

# Short form
ymal -f sample.yaml  -s 'classes.languages::list.perl=Silver' -P '^tst_'

# Long form
ymal --file=sample.yaml  --set-value='classes.languages::list.perl=Silver' \
                         --pattern-to-remove-classes='^tst_'
```


## Contribute

[Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device

## Credits
- Licensed under MIT.

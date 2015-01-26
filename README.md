#lice

An open source license generator and license viewer.

[![NPM](https://nodei.co/npm/lice.png)](https://nodei.co/npm/lice/)

[![Build status](https://travis-ci.org/superkhau/lice.svg?branch=master)](https://travis-ci.org/superkhau/lice)

![](/data/lice.png)

##Installation
```
npm install -g lice
```

##Usage

```
lice
# follow the prompts
```

##CLI mode

```
Usage:
  lice [options]

Options:
  -h, --help     Display the help menu
  -g, --generate Generate a license [default `true`]
  -l, --license  The type of license to generate, [default `mit`]
  -n, --name     The name of the generated license, [default `LICENSE`]
  -p, --path     License generation file path, [default `current working dir`]
  -s, --show     Show the contents of a license
  -u, --user     The name to use in the generated license
  -v, --version  Display the version
  -y, --year     Year placeholder [default `current year`]

Available licenses:
  afl-3.0  Academic Free License 3.0 (AFL-3.0)
  agpl-3.0 GNU Affero General Public License 3.0 (AGPL-3.0)
  gpl-3.0  GNU General Public License 3.0 (GPL-3.0)
  isc      ISC License (ISC)
  mit      The MIT License (MIT) [default]
```

##Example

Let's say you want an MIT license for your project. Switch to the directory
where you want the license generated, run `lice` and follow the prompts:

```
cd /your/project/dir
lice
#follow the prompts, your license will be generated in /your/project/dir
```

Or if you prefer CLI mode:

```
lice -g -l mit -u 'John Doe' # see above for flag definitions or run `lice -h`
```

###Note
You can also provide a path to where you want the license generated via the `-p`
option.

##Contributing

Please help add more licenses! Submit a PR and I will get it merged ASAP.

1. Add a text file with your license content in the [licenses dir](/licenses).
2. Edit [licenses.js](/lib/licenses.js)
3. Update the `Available licenses` section in [README.md](/README.md)
4. Update the help file `Available licenses` section in [help.txt](/data/help.txt)

A good place to find licenses to add is the [Open Source Initiative license page](http://opensource.org/licenses/alphabetical)

##Thanks

[Open Source Initiative](http://opensource.org/) for providing the license
content.

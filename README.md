# npe 

A CLI for one-off inspection and editing of properties in package.json files.

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install npe --global
```

## Usage

```sh
cd some/node/project

# Get stuff from package.json
npe name
npe scripts
npe scripts.test
npe repository.url
open $(npe repository.url)

# Set stuff in package.json
npe name foo
npe scripts.start "node index.js"

# Use a file other than the current directory's package.json
npe name --package=some/other/package.json
npe name other --package=some/other/package.json

```

## Tests

```sh
npm install
npm test
```

## Dependencies

- [minimist](https://github.com/substack/minimist): parse argument options
- [steeltoe](https://github.com/jclem/steeltoe): Don&#39;t shoot yourself in the foot while traversing JavaScript objects.


## Dev Dependencies

- [mocha](https://github.com/visionmedia/mocha): simple, flexible, fun test framework
- [nixt](https://github.com/vesln/nixt): Simple and powerful testing for command-line apps


## License

MIT

## Colophon

- Homepage: https://github.com/zeke/npe
- Author: zeke
- README generated by
[package-json-to-readme](https://github.com/zeke/package-json-to-readme)

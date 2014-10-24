# faves

Audit your machine to generate a list of the npm packages you use most.

`faves` is a command line tool. Give it a directory and it will find every `package.json` file that is *not* inside a `node_modules` or `.git` directory. It inspects the `dependencies` property of each file and keeps a running tally of dependencies. When it's done, a list npm packages names is printed to stdout, sorted by count.

If you run `faves` without passing a directory argument, it will default to `~`. This will probably be a bit slow, but you'll get results for npm project on your machine!

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install faves --global
```

## Usage

```sh
# Audit all top-level package.json files in ~
# (ignoring node_modules directories)
audit

# Audit a specific directory
audit ~/projects
```

## What are npm's faves?

Here are the results of an audit of all the repos in the [github.com/npm](https://github.com/npm) organization:

- [request](https://npm.im/request) (34)
- [lodash](https://npm.im/lodash) (27)
- [underscore](https://npm.im/underscore) (24)
- [bluebird](https://npm.im/bluebird) (22)
- [mkdirp](https://npm.im/mkdirp) (17)
- [yargs](https://npm.im/yargs) (17)
- [async](https://npm.im/async) (17)
- [semver](https://npm.im/semver) (15)
- [restify](https://npm.im/restify) (13)
- [glob](https://npm.im/glob) (13)
- [optimist](https://npm.im/optimist) (11)
- [follow](https://npm.im/follow) (11)
- [rimraf](https://npm.im/rimraf) (10)
- [dashdash](https://npm.im/dashdash) (10)
- [once](https://npm.im/once) (9)
- [chalk](https://npm.im/chalk) (9)
- [moment](https://npm.im/moment) (9)
- [replify](https://npm.im/replify) (8)
- [inherits](https://npm.im/inherits) (8)
- [graceful-fs](https://npm.im/graceful-fs) (8)
- [slide](https://npm.im/slide) (7)
- [github-url-from-git](https://npm.im/github-url-from-git) (7)
- [redis](https://npm.im/redis) (7)
- [numbat-emitter](https://npm.im/numbat-emitter) (6)
- [read-package-json](https://npm.im/read-package-json) (6)
- [minimatch](https://npm.im/minimatch) (6)
- [bole](https://npm.im/bole) (6)
- [bistre](https://npm.im/bistre) (6)
- [joi](https://npm.im/joi) (6)
- [bunyan](https://npm.im/bunyan) (5)
- [nopt](https://npm.im/nopt) (5)
- [lru-cache](https://npm.im/lru-cache) (5)
- [inquirer](https://npm.im/inquirer) (5)
- [read](https://npm.im/read) (5)
- [seq-file](https://npm.im/seq-file) (5)
- [dezalgo](https://npm.im/dezalgo) (4)
- [github-url-from-username-repo](https://npm.im/github-url-from-username-repo) (4)
- [npm-user-validate](https://npm.im/npm-user-validate) (4)
- [fstream](https://npm.im/fstream) (4)
- [fastly](https://npm.im/fastly) (4)
- [manta](https://npm.im/manta) (4)
- [hapi](https://npm.im/hapi) (4)
- [aws-sdk](https://npm.im/aws-sdk) (4)
- [http-https](https://npm.im/http-https) (4)
- [wrappy](https://npm.im/wrappy) (4)
- [debuglog](https://npm.im/debuglog) (3)
- [http-proxy](https://npm.im/http-proxy) (3)

## Dependencies

- [findit](https://github.com/substack/node-findit): walk a directory tree recursively with events
- [lodash](https://github.com/lodash/lodash): A utility library delivering consistency, customization, performance, &amp; extras.


## License

MIT

_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_

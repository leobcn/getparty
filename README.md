# getparty [![Build Status](https://travis-ci.org/vbauerster/getparty.svg?branch=master)](https://travis-ci.org/vbauerster/getparty)

Console download manager

![showcase](showcase.gif)

## Installation
`getparty` requires Go 1.7 or later.
```
$ go get -u github.com/vbauerster/getparty
```
Or download [binary](https://github.com/vbauerster/getparty/releases/latest).

## Usage

```
Usage:
  getparty [OPTIONS] url

Application Options:
  -c, --continue=state.json    resume download from last saved json state
  -p, --parts=                 number of parts (default: 2)
  -t, --timeout=               download timeout in seconds
  -m, --best-mirror            pickup the fastest mirror. Will read from stdin
      --version                show version

Help Options:
  -h, --help                   Show this help message
```

#### Best mirror example:

`cat` [mirrors.txt](https://github.com/vbauerster/getparty/blob/master/cmd/getparty/mirrors.txt) `| getparty -p 8 -m`

## License

[MIT](https://github.com/vbauerster/getparty/blob/master/LICENSE)

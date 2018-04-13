# b32
> base32 command-line utlity

# Installation

```shell
$ go get github.com/picatz/b32
```

#### Updating Version

```shell
$ go get -u github.com/picatz/b32
```

# Usage

After installing, you can run the command `b32` to see the following help menu:

```
NAME:
   b32 - base32 encoder and decoder

USAGE:
   b32 [global options] command [command options] [arguments...]

VERSION:
   1.0.0

COMMANDS:
     encode   encode the given string(s) as base32
     decode   decode the given string(s) as base32
     help, h  Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --help, -h     show help
   --version, -v  print the version
```

To encode a given string with base32 encoding, you can use the `encode` flag:

```shell
$ b32 encode "Example String"
IV4GC3LQNRSSAU3UOJUW4ZY=
```

To decode a given string that been base32 encoded there's the `decode` flag:

```shell
$ b32 decode "IV4GC3LQNRSSAU3UOJUW4ZY="
Example String
```

Illustration of a potential [gopherjs](https://github.com/gopherjs/gopherjs) bug.

On my machine at least, this project builds using go 1.12, but fails to build with gopherjs:

```
$ unset GOPATH
$ go version
go version go1.12.5 darwin/amd64
$ go build
$ gopherjs version
GopherJS 1.12-2
$ gopherjs build
cannot find package "github.com/jancona/foo/bar" in any of:
	/usr/local/Cellar/go/1.12.5/libexec/src/github.com/jancona/foo/bar (from $GOROOT)
	/Users/jim/go/src/github.com/jancona/foo/bar (from $GOPATH)
```
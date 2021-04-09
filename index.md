## Steps to setup go and grpc

- Setup Go:
1. Download and install [golang](https://golang.org/doc/install)
2. run `go version` command in terminal to verify the installation.
3. Confirm that the command prints the installed version of Go.

- Setup Protoc:
1. [Download the windows archive](https://github.com/google/protobuf/releases)
2. Create a folder called _Proto3_ in _C_ Drive and extract the zip file into the folder.

Your directory structure should now be:
```markdown
C:\proto3\bin 
C:\proto3\include
```

- Setup grpc for Go [Go grpc github](https://github.com/grpc/grpc-go)

With Go module support (Go 1.11+), simply add the following import
`import "google.golang.org/grpc"`
to your code, and then `go [build|run|test]` will automatically fetch the necessary dependencies.

Otherwise, to install the grpc-go package, run the following command:

`$ go get -u google.golang.org/grpc`

- Setup protobuf [Protobuf github](https://github.com/golang/protobuf)

Old way: `$ go get -u github.com/golang/protobuf/protoc-gen-go`

New way: `$ go get -u google.golang.org/protobuf`

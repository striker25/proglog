# proglog

## Install Protobuf

```bash
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
```

## Compile Protobuf

```bash
protoc api/v1/*.proto \
    --go_out=. \
    --go_opt=paths=source_relative \
    --proto_path=.
```

## Install Make

```cmd
choco install make
```

With make installed and the Makefile properly configured in the root of the project, it is just required to run the "make" command to generate the structs from the proto3 files.

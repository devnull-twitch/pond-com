# Pond Communication

This repository contains the protobuf definitions and generated code to communicate with the pond backend.

## Build

You need:
* [protoc](https://github.com/protocolbuffers/protobuf/releases/latest)
* protoc-gen-go `go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.26`
* protoc-gen-go-grpc `go install go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.1`
* buf `go install github.com/bufbuild/buf/cmd/buf@latest`
* To run lint you also need protoc-gen-buf-lint `go install github.com/bufbuild/buf/cmd/protoc-gen-buf-lint@latest`

If everything is setup you can just run `buf generate` to update the geenrated code.

You should run `buf lint` to check changes do not validate any linting rules
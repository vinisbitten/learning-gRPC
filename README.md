# Tutorial on how to create a gRPC server and client in Go

## Install

go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28

go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2

apt install -y protobuf-compiler

## Initiated go module

go mod init github.com/vinisbitten/learning-gRPC

## Create proto file

protoc --go_out=. --go-grpc_out=. proto/course_category.proto

## Tidy up

go mod tidy

## See gRPC interface

--> proto/course_category.pb.go
(how to implement the interface)

## creating grpcServer
# grpc-go-example

## Regenerate gRPC code

```
$ protoc --go_out=. --go_opt=paths=source_relative \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    helloworld/helloworld.proto
```

## Run

```
$ go run server/server.go

$ go run client/client.go
2024/01/01 01:03:58 Greeting: Hello world
```

## References
- https://grpc.io/docs/languages/go/
- https://github.com/grpc/grpc-go/tree/master/examples/helloworld

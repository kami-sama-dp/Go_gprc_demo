# Go_gprc_demo

    一个微服务demo

    go mod init shippy 

生成protobuf  go

    protoc  --go_out=plugins=grpc:./pblib   proto/*.proto

可能需要修改相对import路径
```
sed -i -E 's/^\(import.*_pb2\)/from . \1/' pblib/proto/*.py
```

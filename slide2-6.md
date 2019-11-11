### しかしprotobufで定義すれば

```
syntax = "proto3"
package com.lt.proto

message Response{
  Human speaker = 1;
  Human listner = 2;
  Beer beer = 3;
}

message Human{
  int32 count = 1;
}

message Beer{
  int64 count = 1;
}
```

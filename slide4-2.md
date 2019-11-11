### Protocol BufferはGRPCに必須か？

Protocol BufferをRPCサービスとして<br />
手軽に使えるように定義されている<br />
つまり必須ではない。

---

### GRPCの

#### メリット

- 手軽なProtocolBuffer RPCサービスの実装
- ProtocolBuffer拡張ある言語は大概GRPCのモジュールもある
- HTTP/2対応

#### デメリット

- HTTP/2対応が必須なので、既存のHTTP/1.xで動いているサービスを乗せるのに検証・調査のコストが必要

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

- HTTP/2対応が必須。そのため既存HTTP/1.xのサービスでの利用は検証・調査のコストが必要

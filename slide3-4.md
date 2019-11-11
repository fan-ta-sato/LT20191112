### scalaPBでのcompile例

#### protocol buffer定義

```
message Person {
  string name = 1;
  int32 age = 2;

  repeated Address addresses = 3;
}

message Address {
  string street = 1;
  string city = 2;
}
```

---

#### Scalaオブジェクトへの変換

```scala
final case class Person(
  name: String = None,
  age: Int = None,
  addresses: Seq[Address] = Nil, ...) extends GeneratedMessage {

  def toByteArray: Array[Byte] = { ... }

  // more stuff...
}

object Person extends GeneratedMessageCompanion[Person] {
  def parseFrom(bytes: Array[Byte]): Person = { ... }

  // more stuff...
}

// similar stuff for Address...
```

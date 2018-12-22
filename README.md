# Buffer
```
package main

import "github.com/haiswork/hBuffer"

func main() {
     bf := hBuffer.NewBuffer()

     bf.WriteBool(true)
     bf.WriteInt32(123)
     bf.WriteInt64(124)
     bf.WriteUint32(125)
     bf.WriteUint64(126)
     bf.WriteFloat32(122.33)
     bf.WriteFloat64(122.44)
     bf.WriteString("test_abc")

     //read from position 0
     bf.SetPosition(0)

     bf.ReadBool()
     bf.ReadInt32()
     bf.ReadInt64()
     bf.ReadUint32()
     bf.ReadUint64()
     bf.ReadFloat32()
     bf.ReadFloat64()
     bf.ReadString()
}
```

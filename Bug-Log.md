# Bug Log

## Bug Fix Log: [Save System]

#### Status: $\color{green}{\text{Fixed}}$
#### System: Save System

### Discovered
#### Date: 12-11-2026

### Resolved
#### Date: 

---

### Problem
* The save system is not functioning as intended; error message noted below:
  - SerializationException: Type 'UnityEngine.MonoBehaviour' in Assembly 'UnityEngine.CoreModule, Version=0.0.0.0, Culture=neutral, PublicKeyToken=null' is not marked as serializable.
System.Runtime.Serialization.FormatterServices.InternalGetSerializableMembers (System.RuntimeType type) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.FormatterServices+<>c__DisplayClass9_0.<GetSerializableMembers>b__0 (System.Runtime.Serialization.MemberHolder _) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Collections.Concurrent.ConcurrentDictionary`2[TKey,TValue].GetOrAdd (TKey key, System.Func`2[T,TResult] valueFactory) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.FormatterServices.GetSerializableMembers (System.Type type, System.Runtime.Serialization.StreamingContext context) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.WriteObjectInfo.InitMemberInfo () (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.WriteObjectInfo.InitSerialize (System.Object obj, System.Runtime.Serialization.ISurrogateSelector surrogateSelector, System.Runtime.Serialization.StreamingContext context, System.Runtime.Serialization.Formatters.Binary.SerObjectInfoInit serObjectInfoInit, System.Runtime.Serialization.IFormatterConverter converter, System.Runtime.Serialization.Formatters.Binary.ObjectWriter objectWriter, System.Runtime.Serialization.SerializationBinder binder) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.WriteObjectInfo.Serialize (System.Object obj, System.Runtime.Serialization.ISurrogateSelector surrogateSelector, System.Runtime.Serialization.StreamingContext context, System.Runtime.Serialization.Formatters.Binary.SerObjectInfoInit serObjectInfoInit, System.Runtime.Serialization.IFormatterConverter converter, System.Runtime.Serialization.Formatters.Binary.ObjectWriter objectWriter, System.Runtime.Serialization.SerializationBinder binder) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.ObjectWriter.Serialize (System.Object graph, System.Runtime.Remoting.Messaging.Header[] inHeaders, System.Runtime.Serialization.Formatters.Binary.__BinaryWriter serWriter, System.Boolean fCheck) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.BinaryFormatter.Serialize (System.IO.Stream serializationStream, System.Object graph, System.Runtime.Remoting.Messaging.Header[] headers, System.Boolean fCheck) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.BinaryFormatter.Serialize (System.IO.Stream serializationStream, System.Object graph, System.Runtime.Remoting.Messaging.Header[] headers) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.Runtime.Serialization.Formatters.Binary.BinaryFormatter.Serialize (System.IO.Stream serializationStream, System.Object graph) (at <1071a2cb0cb3433aae80a793c277a048>:0)
SaveSystem.SaveGame (Data data) (at Assets/Scripts/SaveSystem.cs:18)
Data.savePlayerPos () (at Assets/Scripts/Data.cs:39)
Data.Update () (at Assets/Scripts/Data.cs:22)

  - IOException: Sharing violation on path D:\Unity\UnityProjects\Vaelith\Assets\SaveFile\save.file
System.IO.FileStream..ctor (System.String path, System.IO.FileMode mode, System.IO.FileAccess access, System.IO.FileShare share, System.Int32 bufferSize, System.Boolean anonymous, System.IO.FileOptions options) (at <1071a2cb0cb3433aae80a793c277a048>:0)
System.IO.FileStream..ctor (System.String path, System.IO.FileMode mode) (at <1071a2cb0cb3433aae80a793c277a048>:0)
(wrapper remoting-invoke-with-check) System.IO.FileStream..ctor(string,System.IO.FileMode)
SaveSystem.LoadGame () (at Assets/Scripts/SaveSystem.cs:28)
Data.loadPlayerPos () (at Assets/Scripts/Data.cs:45)
Data.Update () (at Assets/Scripts/Data.cs:27)

---

### Resolution

1. **:** 

---

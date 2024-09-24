# UE5-Protobuf
 
This is a prebuilt version v27.2 of [protobuf](https://github.com/protocolbuffers/protobuf/tree/v27.2) 
using c++ standard 20.

`ThirdParty` contains libs and headers
`bin` contains binary like `protoc`

config  your Build.cs 
```cs
// 1. Add include 
// 2. Add lib
// 3. Add extra definitions 
		PublicDefinitions.Add("PROTOBUF_ENABLE_DEBUG_LOGGING_MAY_LEAK_PII=0");
		PublicDefinitions.Add("PROTOBUF_BUILTIN_ATOMIC=0");

```

if you have security concerns and want to build from source,the following gist might help

https://gist.github.com/ibreathebsb/73ddba5e359b761d43bb9f15667c173f

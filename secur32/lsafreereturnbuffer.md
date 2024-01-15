# LsaFreeReturnBuffer

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaFreeReturnBuffer(void* Buffer);
```

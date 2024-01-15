# LsaConnectUntrusted

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaConnectUntrusted(HANDLE* LsaHandle);
```

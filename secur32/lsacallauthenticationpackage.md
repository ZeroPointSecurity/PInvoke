# LsaCallAuthenticationPackage

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaCallAuthenticationPackage(
    HANDLE LsaHandle,
    uint AuthenticationPackage,
    void* ProtocolSubmitBuffer,
    uint SubmitBufferLength,
    [Optional] void** ProtocolReturnBuffer,
    [Optional] uint* ReturnBufferLength,
    [Optional] int* ProtocolStatus);
```

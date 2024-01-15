# InitializeSecurityContext

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true, EntryPoint = "InitializeSecurityContextW")]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT InitializeSecurityContext(
    [Optional] SecHandle* phCredential,
    [Optional] SecHandle* phContext,
    [Optional] ushort* pszTargetName,
    ISC_REQ_FLAGS fContextReq,
    uint Reserved1,
    uint TargetDataRep,
    [Optional] SecBufferDesc* pInput,
    uint Reserved2,
    [Optional] SecHandle* phNewContext,
    [Optional] SecBufferDesc* pOutput,
    uint* pfContextAttr,
    [Optional] long* ptsExpiry);
```

# InitializeSecurityContextA

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT InitializeSecurityContextA(
    [Optional] SecHandle* phCredential,
    [Optional] SecHandle* phContext,
    [Optional] sbyte* pszTargetName,
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

[sechandle.md](../security/sechandle.md "mention")

[isc\_req\_flags.md](../authentication/isc\_req\_flags.md "mention")

[secbufferdesc.md](../authentication/secbufferdesc.md "mention")

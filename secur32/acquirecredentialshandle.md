# AcquireCredentialsHandle

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true, EntryPoint = "AcquireCredentialsHandleW")]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT AcquireCredentialsHandle(
    PWSTR pszPrincipal,
    PWSTR pszPackage,
    SECPKG_CRED fCredentialUse,
    [Optional] void* pvLogonId,
    [Optional] void* pAuthData,
    SEC_GET_KEY_FN pGetKeyFn,
    [Optional] void* pvGetKeyArgument,
    SecHandle* phCredential,
    [Optional] long* ptsExpiry);
```

[secpkg\_cred.md](../authentication/secpkg\_cred.md "mention")

[sec\_get\_key\_fn.md](../authentication/sec\_get\_key\_fn.md "mention")

[sechandle.md](../security/sechandle.md "mention")

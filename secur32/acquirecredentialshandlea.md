# AcquireCredentialsHandleA

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT AcquireCredentialsHandleA(
    PSTR pszPrincipal,
    PSTR pszPackage,
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

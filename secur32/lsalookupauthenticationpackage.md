# LsaLookupAuthenticationPackage

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaLookupAuthenticationPackage(
    HANDLE LsaHandle,
    LSA_STRING* PackageName,
    uint* AuthenticationPackage);
```

[lsa\_string.md](../authentication/lsa\_string.md "mention")

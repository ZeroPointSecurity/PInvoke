# LsaEnumerateTrustedDomains

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaEnumerateTrustedDomains(
    LSA_HANDLE PolicyHandle,
    uint* EnumerationContext,
    void** Buffer,
    uint PreferedMaximumLength,
    uint* CountReturned);
```

[ntstatus.md](../foundation/ntstatus.md "mention")

[lsa\_handle.md](../authentication/lsa\_handle.md "mention")

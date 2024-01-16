# GetSidSubAuthority

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe uint* GetSidSubAuthority(
    PSID pSid,
    uint nSubAuthority);
```

[psid.md](../foundation/psid.md "mention")

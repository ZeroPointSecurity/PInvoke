# OpenProcessToken

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL OpenProcessToken(
    HANDLE ProcessHandle,
    TOKEN_ACCESS_MASK DesiredAccess,
    HANDLE* TokenHandle);
```

[token\_access\_mask.md](../security/token\_access\_mask.md "mention")

# DuplicateTokenEx

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL DuplicateTokenEx(
    HANDLE hExistingToken,
    TOKEN_ACCESS_MASK dwDesiredAccess,
    [Optional] SECURITY_ATTRIBUTES* lpTokenAttributes,
    SECURITY_IMPERSONATION_LEVEL ImpersonationLevel,
    TOKEN_TYPE TokenType,
    HANDLE* phNewToken);
```

[token\_access\_mask.md](../security/token\_access\_mask.md "mention")

[security\_impersonation\_level.md](../security/security\_impersonation\_level.md "mention")

[token\_type.md](../security/token\_type.md "mention")

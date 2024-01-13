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

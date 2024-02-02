# NtDuplicateToken

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtDuplicateToken(
    HANDLE ExistingToken,
    uint DesiredAccess,
    [Optional] OBJECT_ATTRIBUTES*   ObjectAttributes,
    SECURITY_IMPERSONATION_LEVEL ImpersonationLevel,
    TOKEN_TYPE TokenType,
    HANDLE* NewToken);
```

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[security\_impersonation\_level.md](../security/security\_impersonation\_level.md "mention")

[token\_type.md](../security/token\_type.md "mention")

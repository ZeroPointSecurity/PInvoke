# NtAdjustPrivilegesToken

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtAdjustPrivilegesToken(
    HANDLE TokenHandle,
    BOOL DisableAllPrivileges,
    TOKEN_PRIVILEGES* NewState,
    uint BufferLength,
    [Optional] TOKEN_PRIVILEGES* PreviousState,
    [Optional] uint* ReturnLength);
```

[token\_privileges.md](../security/token\_privileges.md "mention")

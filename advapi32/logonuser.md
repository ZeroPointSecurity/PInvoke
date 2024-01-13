# LogonUser

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "LogonUserW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL LogonUser(
    PCWSTR lpszUsername,
    PCWSTR lpszDomain,
    PCWSTR lpszPassword,
    LOGON32_LOGON dwLogonType,
    LOGON32_PROVIDER dwLogonProvider,
    HANDLE* phToken);
```

[logon32\_logon.md](../security/logon32\_logon.md "mention")

[logon32\_provider.md](../security/logon32\_provider.md "mention")

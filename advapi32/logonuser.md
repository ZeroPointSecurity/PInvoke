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

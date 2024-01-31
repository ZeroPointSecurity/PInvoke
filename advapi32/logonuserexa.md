# LogonUserExA

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL LogonUserExA(
    PCSTR lpszUsername,
    PCSTR lpszDomain,
    PCSTR lpszPassword,
    LOGON32_LOGON dwLogonType,
    LOGON32_PROVIDER dwLogonProvider,
    [Optional] HANDLE* phToken,
    [Optional] PSID* ppLogonSid,
    [Optional] void** ppProfileBuffer,
    [Optional] uint* pdwProfileLength,
    [Optional] QUOTA_LIMITS* pQuotaLimits);
```

[logon32\_logon.md](../security/logon32\_logon.md "mention")

[logon32\_provider.md](../security/logon32\_provider.md "mention")

[quota\_limits.md](../security/quota\_limits.md "mention")

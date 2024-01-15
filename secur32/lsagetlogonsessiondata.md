# LsaGetLogonSessionData

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaGetLogonSessionData(
    LUID* LogonId,
    SECURITY_LOGON_SESSION_DATA** ppLogonSessionData);
```

[luid.md](../foundation/luid.md "mention")

[security\_logon\_session\_data.md](../authentication/security\_logon\_session\_data.md "mention")

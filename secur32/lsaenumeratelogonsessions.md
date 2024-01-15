# LsaEnumerateLogonSessions

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaEnumerateLogonSessions(
    uint* LogonSessionCount,
    LUID** LogonSessionList);
```

[luid.md](../foundation/luid.md "mention")

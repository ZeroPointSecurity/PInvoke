# CreateMailslotA

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateMailslotA(
    PCSTR lpName,
    uint nMaxMessageSize,
    uint lReadTimeout,
    [Optional] SECURITY_ATTRIBUTES* lpSecurityAttributes);
```

[security\_attributes.md](../security/security\_attributes.md "mention")

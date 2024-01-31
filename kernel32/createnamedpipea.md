# CreateNamedPipeA

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateNamedPipeA(
    PCSTR lpName,
    FILE_FLAGS_AND_ATTRIBUTES dwOpenMode,
    NAMED_PIPE_MODE dwPipeMode,
    uint nMaxInstances,
    uint nOutBufferSize,
    uint nInBufferSize,
    uint nDefaultTimeOut,
    [Optional] SECURITY_ATTRIBUTES* lpSecurityAttributes);
```

[file\_flags\_and\_attributes.md](../filesystem/file\_flags\_and\_attributes.md "mention")

[named\_pipe\_mode.md](../pipes/named\_pipe\_mode.md "mention")

[security\_attributes.md](../security/security\_attributes.md "mention")

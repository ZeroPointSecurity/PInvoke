# CreateNamedPipe

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, EntryPoint = "CreateNamedPipeW")]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateNamedPipe(
    PCWSTR lpName,
    FILE_FLAGS_AND_ATTRIBUTES dwOpenMode,
    NAMED_PIPE_MODE dwPipeMode,
    uint nMaxInstances,
    uint nOutBufferSize,
    uint nInBufferSize,
    uint nDefaultTimeOut,
    [Optional] SECURITY_ATTRIBUTES* lpSecurityAttributes);
```

# NtProtectVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtProtectVirtualMemory(
    HANDLE ProcessHandle,
    void* BaseAddress,
    uint* NumberOfBytesToProtect,
    uint NewAccessProtection,
    uint* OldAccessProtection);
```

[page\_protection\_flags.md](../memory/page\_protection\_flags.md "mention")

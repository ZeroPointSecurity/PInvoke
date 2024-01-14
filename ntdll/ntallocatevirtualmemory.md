# NtAllocateVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtAllocateVirtualMemory(
    HANDLE ProcessHandle,
    void* BaseAddress,
    uint ZeroBits,
    uint* RegionSize,
    uint AllocationType,
    uint Protect);
```

[virtual\_allocation\_type.md](../memory/virtual\_allocation\_type.md "mention")

[page\_protection\_flags.md](../memory/page\_protection\_flags.md "mention")

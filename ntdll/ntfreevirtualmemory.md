# NtFreeVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtFreeVirtualMemory(
    HANDLE ProcessHandle,
    void* BaseAddress,
    uint* RegionSize,
    uint FreeType);
```

[virtual\_free\_type.md](../memory/virtual\_free\_type.md "mention")

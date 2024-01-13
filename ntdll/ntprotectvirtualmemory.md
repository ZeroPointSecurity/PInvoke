# NtProtectVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtProtectVirtualMemory(
    HANDLE ProcessHandle,
    void* BaseAddress,
    nint* RegionSize,
    PAGE_PROTECTION_FLAGS NewProtect,
    PAGE_PROTECTION_FLAGS* OldProtect);
```

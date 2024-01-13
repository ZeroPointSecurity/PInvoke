# NtAllocateVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtAllocateVirtualMemory(
    HANDLE ProcessHandle,
    void* BaseAddress,
    nint ZeroBits,
    nint* RegionSize,
    VIRTUAL_ALLOCATION_TYPE AllocationType,
    PAGE_PROTECTION_FLAGS Protect);
```

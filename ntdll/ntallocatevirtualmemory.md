# NtAllocateVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtAllocateVirtualMemory(
    HANDLE processHandle,
    void* baseAddress,
    nint zeroBits,
    nint* regionSize,
    VIRTUAL_ALLOCATION_TYPE allocationType,
    PAGE_PROTECTION_FLAGS protect);
```

# VirtualAllocEx

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe void* VirtualAllocEx(
    HANDLE hProcess,
    [Optional] void* lpAddress,
    nuint dwSize,
    VIRTUAL_ALLOCATION_TYPE flAllocationType,
    PAGE_PROTECTION_FLAGS flProtect);
```
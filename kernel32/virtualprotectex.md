# VirtualProtectEx

````csharp
```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL VirtualProtectEx(
    HANDLE hProcess,
    void* lpAddress,
    nuint dwSize,
    PAGE_PROTECTION_FLAGS flNewProtect,
    PAGE_PROTECTION_FLAGS* lpflOldProtect);
```
````
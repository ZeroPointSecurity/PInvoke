# VirtualProtect

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL VirtualProtect(
    void* lpAddress,
    nuint dwSize,
    PAGE_PROTECTION_FLAGS flNewProtect,
    PAGE_PROTECTION_FLAGS* lpflOldProtect);
```

[page\_protection\_flags.md](../memory/page\_protection\_flags.md "mention")

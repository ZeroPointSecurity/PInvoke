# LoadLibraryExW

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern HMODULE LoadLibraryExW(
    PCWSTR lpLibFileName,
    HANDLE hFile,
    LOAD_LIBRARY_FLAGS dwFlags);
```

[load\_library\_flags.md](../library-loader/load\_library\_flags.md "mention")

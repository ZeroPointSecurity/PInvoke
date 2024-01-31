# LoadLibraryExA

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern HMODULE LoadLibraryExA(
    PCSTR lpLibFileName,
    HANDLE hFile,
    LOAD_LIBRARY_FLAGS dwFlags);
```

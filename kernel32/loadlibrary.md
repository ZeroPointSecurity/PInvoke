# LoadLibrary

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, EntryPoint = "LoadLibraryW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern HMODULE LoadLibrary(PCWSTR lpLibFileName);
```

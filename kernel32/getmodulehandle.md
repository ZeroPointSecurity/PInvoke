# GetModuleHandle

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, EntryPoint = "GetModuleHandleW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern HMODULE GetModuleHandle(PCWSTR lpModuleName);
```

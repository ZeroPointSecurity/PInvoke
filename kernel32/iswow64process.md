# IsWow64Process

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL IsWow64Process(
    HANDLE hProcess,
    BOOL* Wow64Process);
```

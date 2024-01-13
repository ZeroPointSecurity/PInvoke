# StartService

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "StartServiceW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL StartService(
    SC_HANDLE hService,
    uint dwNumServiceArgs,
    [Optional] PCWSTR* lpServiceArgVectors);
```

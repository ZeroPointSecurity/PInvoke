# StartServiceW

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL StartServiceW(
    SC_HANDLE hService,
    uint dwNumServiceArgs,
    [Optional] PCWSTR* lpServiceArgVectors);
```

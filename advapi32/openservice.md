# OpenService

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "OpenServiceW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern SC_HANDLE OpenService(
    SC_HANDLE hSCManager,
    PCWSTR lpServiceName,
    uint dwDesiredAccess);
```

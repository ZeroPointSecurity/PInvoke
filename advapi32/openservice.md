# OpenServiceW

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern SC_HANDLE OpenServiceW(
    SC_HANDLE hSCManager,
    PCWSTR lpServiceName,
    uint dwDesiredAccess);
```

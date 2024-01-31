# OpenServiceA

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern SC_HANDLE OpenServiceA(
    SC_HANDLE hSCManager,
    PCSTR lpServiceName,
    uint dwDesiredAccess);
```

# ControlService

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL ControlService(
    SC_HANDLE hService,
    uint dwControl,
    SERVICE_STATUS* lpServiceStatus);
```

[service\_status.md](../services/service\_status.md "mention")

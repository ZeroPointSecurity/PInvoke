# CreateService

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "CreateServiceW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe SC_HANDLE CreateService(
    SC_HANDLE hSCManager,
    PCWSTR lpServiceName,
    PCWSTR lpDisplayName,
    uint dwDesiredAccess,
    ENUM_SERVICE_TYPE dwServiceType,
    SERVICE_START_TYPE dwStartType,
    SERVICE_ERROR dwErrorControl,
    PCWSTR lpBinaryPathName,
    PCWSTR lpLoadOrderGroup,
    [Optional] uint* lpdwTagId,
    PCWSTR lpDependencies,
    PCWSTR lpServiceStartName,
    PCWSTR lpPassword);
```

[enum\_service\_type.md](../services/enum\_service\_type.md "mention")

[service\_start\_type.md](../services/service\_start\_type.md "mention")

[service\_error.md](../services/service\_error.md "mention")

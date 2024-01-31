# CreateServiceA

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe SC_HANDLE CreateServiceA(
    SC_HANDLE hSCManager,
    PCSTR lpServiceName,
    PCSTR lpDisplayName,
    uint dwDesiredAccess,
    ENUM_SERVICE_TYPE dwServiceType,
    SERVICE_START_TYPE dwStartType,
    SERVICE_ERROR dwErrorControl,
    PCSTR lpBinaryPathName,
    PCSTR lpLoadOrderGroup,
    [Optional] uint* lpdwTagId,
    PCSTR lpDependencies,
    PCSTR lpServiceStartName,
    PCSTR lpPassword);
```

[enum\_service\_type.md](../services/enum\_service\_type.md "mention")

[service\_start\_type.md](../services/service\_start\_type.md "mention")

[service\_error.md](../services/service\_error.md "mention")

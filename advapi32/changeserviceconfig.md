# ChangeServiceConfigW

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL ChangeServiceConfigW(
    SC_HANDLE hService,
    ENUM_SERVICE_TYPE dwServiceType,
    SERVICE_START_TYPE dwStartType,
    SERVICE_ERROR dwErrorControl,
    PCWSTR lpBinaryPathName,
    PCWSTR lpLoadOrderGroup,
    [Optional] uint* lpdwTagId,
    PCWSTR lpDependencies,
    PCWSTR lpServiceStartName,
    PCWSTR lpPassword,
    PCWSTR lpDisplayName);
```

[sc\_handle.md](../security/sc\_handle.md "mention")

[enum\_service\_type.md](../services/enum\_service\_type.md "mention")

[service\_start\_type.md](../services/service\_start\_type.md "mention")

[service\_error.md](../services/service\_error.md "mention")

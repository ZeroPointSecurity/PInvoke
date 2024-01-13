# ChangeServiceConfig

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "ChangeServiceConfigW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe winmdroot.Foundation.BOOL ChangeServiceConfig(
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

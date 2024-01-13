# OpenSCManager

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "OpenSCManagerW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern SC_HANDLE OpenSCManager(
    PCWSTR lpMachineName,
    PCWSTR lpDatabaseName,
    uint dwDesiredAccess);
```

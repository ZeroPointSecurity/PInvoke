# OpenSCManagerW

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern SC_HANDLE OpenSCManagerW(
    PCWSTR lpMachineName,
    PCWSTR lpDatabaseName,
    uint dwDesiredAccess);
```

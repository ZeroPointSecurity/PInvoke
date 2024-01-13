# CreateProcessWithToken

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "CreateProcessWithTokenW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CreateProcessWithToken(
    HANDLE hToken,
    CREATE_PROCESS_LOGON_FLAGS dwLogonFlags,
    PCWSTR lpApplicationName,
    PWSTR lpCommandLine,
    PROCESS_CREATION_FLAGS dwCreationFlags,
    [Optional] void* lpEnvironment,
    PCWSTR lpCurrentDirectory,
    STARTUPINFOW* lpStartupInfo,
    PROCESS_INFORMATION* lpProcessInformation);
```

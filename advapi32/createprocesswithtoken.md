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

[create\_process\_logon\_flags.md](../threading/create\_process\_logon\_flags.md "mention")

[process\_creation\_flags.md](../threading/process\_creation\_flags.md "mention")

[startupinfow.md](../threading/startupinfow.md "mention")

[process\_information.md](../threading/process\_information.md "mention")

# CreateProcessAsUser

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, EntryPoint = "CreateProcessAsUserW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CreateProcessAsUser(
    HANDLE hToken,
    PCWSTR lpApplicationName,
    PWSTR lpCommandLine,
    [Optional] SECURITY_ATTRIBUTES* lpProcessAttributes,
    [Optional] SECURITY_ATTRIBUTES* lpThreadAttributes,
    BOOL bInheritHandles,
    PROCESS_CREATION_FLAGS dwCreationFlags,
    [Optional] void* lpEnvironment,
    PCWSTR lpCurrentDirectory,
    STARTUPINFOW* lpStartupInfo,
    PROCESS_INFORMATION* lpProcessInformation);
```

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[process\_creation\_flags.md](../threading/process\_creation\_flags.md "mention")

[startupinfow.md](../threading/startupinfow.md "mention")

[process\_information.md](../threading/process\_information.md "mention")

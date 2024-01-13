# CreateProcess

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, EntryPoint = "CreateProcessW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CreateProcess(
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

[process\_creation\_flags.md](../threading/process\_creation\_flags.md "mention")

[startupinfow.md](../threading/startupinfow.md "mention")

[process\_information.md](../threading/process\_information.md "mention")

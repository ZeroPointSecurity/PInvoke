# CreateProcessAsUserA

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CreateProcessAsUserA(
    HANDLE hToken,
    PCSTR lpApplicationName,
    PSTR lpCommandLine,
    [Optional] SECURITY_ATTRIBUTES* lpProcessAttributes,
    [Optional] SECURITY_ATTRIBUTES* lpThreadAttributes,
    BOOL bInheritHandles,
    PROCESS_CREATION_FLAGS dwCreationFlags,
    [Optional] void* lpEnvironment,
    PCSTR lpCurrentDirectory,
    STARTUPINFOA* lpStartupInfo,
    PROCESS_INFORMATION* lpProcessInformation);
```

[security\_attributes.md](../security/security\_attributes.md "mention")

[process\_creation\_flags.md](../threading/process\_creation\_flags.md "mention")

[startupinfoa.md](../threading/startupinfoa.md "mention")

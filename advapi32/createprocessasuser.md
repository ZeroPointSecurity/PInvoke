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

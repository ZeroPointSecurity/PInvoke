# NtQueryInformationProcess

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtQueryInformationProcess(
    HANDLE processHandle,
    PROCESSINFOCLASS processInformationClass,
    void* processInformation,
    uint processInformationLength,
    uint* returnLength);
```

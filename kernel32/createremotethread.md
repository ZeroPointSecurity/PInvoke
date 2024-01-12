# CreateRemoteThread

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateRemoteThread(
    HANDLE hProcess,
    [Optional] SECURITY_ATTRIBUTES* lpThreadAttributes,
    nuint dwStackSize,
    LPTHREAD_START_ROUTINE lpStartAddress,
    [Optional] void* lpParameter,
    uint dwCreationFlags,
    [Optional] uint* lpThreadId);
```

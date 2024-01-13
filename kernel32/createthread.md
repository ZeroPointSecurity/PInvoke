# CreateThread

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateThread(
    [Optional] SECURITY_ATTRIBUTES* lpThreadAttributes,
    nuint dwStackSize,
    LPTHREAD_START_ROUTINE lpStartAddress,
    [Optional] void* lpParameter,
    THREAD_CREATION_FLAGS dwCreationFlags,
    [Optional] uint* lpThreadId);
```

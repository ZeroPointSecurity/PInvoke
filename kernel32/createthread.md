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

[lpthread\_start\_routine.md](../threading/lpthread\_start\_routine.md "mention")

[thread\_creation\_flags.md](../threading/thread\_creation\_flags.md "mention")

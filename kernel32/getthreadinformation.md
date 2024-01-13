# GetThreadInformation

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL GetThreadInformation(
    HANDLE hThread,
    THREAD_INFORMATION_CLASS ThreadInformationClass,
    void* ThreadInformation,
    uint ThreadInformationSize);
```

[thread\_information\_class.md](../threading/thread\_information\_class.md "mention")

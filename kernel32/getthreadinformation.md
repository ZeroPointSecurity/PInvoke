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

[Broken link](broken-reference "mention")

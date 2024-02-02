# NtSetInformationThread

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtSetInformationThread(
    HANDLE ThreadHandle,
    THREAD_INFORMATION_CLASS ThreadInformationClass,
    void* ThreadInformation,
    uint ThreadInformationLength);
```

[thread\_information\_class.md](../foundation/thread\_information\_class.md "mention")

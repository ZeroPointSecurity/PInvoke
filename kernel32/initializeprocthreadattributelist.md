# InitializeProcThreadAttributeList

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL InitializeProcThreadAttributeList(
    LPPROC_THREAD_ATTRIBUTE_LIST lpAttributeList,
    uint dwAttributeCount,
    uint dwFlags,
    nuint* lpSize);
```

[lpproc\_thread\_attribute\_list.md](../threading/lpproc\_thread\_attribute\_list.md "mention")

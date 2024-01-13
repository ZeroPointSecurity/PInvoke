# UpdateProcThreadAttribute

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL UpdateProcThreadAttribute(
    LPPROC_THREAD_ATTRIBUTE_LIST lpAttributeList,
    uint dwFlags,
    nuint Attribute,
    [Optional] void* lpValue,
    nuint cbSize,
    [Optional] void* lpPreviousValue,
    [Optional] nuint* lpReturnSize);
```

[lpproc\_thread\_attribute\_list.md](../threading/lpproc\_thread\_attribute\_list.md "mention")

[proc\_thread\_attribute.md](../threading/proc\_thread\_attribute.md "mention")

[process\_creation\_mitigation\_policy.md](../threading/process\_creation\_mitigation\_policy.md "mention")

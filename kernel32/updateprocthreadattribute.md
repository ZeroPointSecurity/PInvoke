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

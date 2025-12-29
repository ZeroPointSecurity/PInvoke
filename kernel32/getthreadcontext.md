# GetThreadContext

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL GetThreadContext(
    HANDLE hThread,
    CONTEXT* lpContext);
```

[context.md](../debug/context.md "mention")

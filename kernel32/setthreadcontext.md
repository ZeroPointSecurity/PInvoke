# SetThreadContext

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL SetThreadContext(
    HANDLE hThread,
    CONTEXT* lpContext);
```

[context.md](../debug/context.md "mention")

# HeapFree

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL HeapFree(
    HANDLE hHeap,
    HEAP_FLAGS dwFlags,
    [Optional] void* lpMem);
```

[heap\_flags.md](../memory/heap\_flags.md "mention")

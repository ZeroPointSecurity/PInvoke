# HeapAlloc

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe void* HeapAlloc(
    HANDLE hHeap,
    HEAP_FLAGS dwFlags,
    nuint dwBytes);
```

[heap\_flags.md](../memory/heap\_flags.md "mention")

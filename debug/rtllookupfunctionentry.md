# RtlLookupFunctionEntry

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe IMAGE_RUNTIME_FUNCTION_ENTRY* RtlLookupFunctionEntry(
    ulong ControlPc,
    ulong* ImageBase,
    [Optional] UNWIND_HISTORY_TABLE* HistoryTable);
```

[image_runtime_function_entry.md](image_runtime_function_entry.md "mention")

[unwind_history_table.md](unwind_history_table.md "mention")
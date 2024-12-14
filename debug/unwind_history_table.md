# UNWIND\_HISTORY\_TABLE

```csharp
public struct UNWIND_HISTORY_TABLE
{
	public uint Count;
	public byte LocalHint;
	public byte GlobalHint;
	public byte Search;
	public byte Once;
	public nuint LowAddress;
	public nuint HighAddress;
	public UNWIND_HISTORY_TABLE_ENTRY Entry;
}
```

[unwind_history_table_entry.md](unwind_history_table_entry.md "mention")
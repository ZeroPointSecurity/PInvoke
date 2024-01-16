# LDR\_DATA\_TABLE\_ENTRY

```csharp
public unsafe struct LDR_DATA_TABLE_ENTRY
{
    public void* Reserved1;
    public LIST_ENTRY InMemoryOrderLinks;
    public void* Reserved2;
    public void* DllBase;
    public void* Reserved3;
    public UNICODE_STRING FullDllName;
    public void* Reserved4;
    public void* Reserved5;
    public Anonymous Union;
    public uint TimeDateStamp;

    [StructLayout(LayoutKind.Explicit)]
    public struct Anonymous
    {
        [FieldOffset(0)]
        public uint CheckSum;

        [FieldOffset(0)]
        public void* Reserved6;
    }
}
```

[list\_entry.md](../kernel/list\_entry.md "mention")

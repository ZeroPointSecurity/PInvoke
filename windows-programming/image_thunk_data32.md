# IMAGE\_THUNK\_DATA32

```csharp
public struct IMAGE_THUNK_DATA32
{
    public Anonymous Union;

    [StructLayout(LayoutKind.Explicit)]
    public struct Anonymous
    {
        [FieldOffset(0)]
        public uint ForwarderString;

        [FieldOffset(0)]
        public uint Function;

        [FieldOffset(0)]
        public uint Ordinal;

        [FieldOffset(0)]
        public uint AddressOfData;
    }
}
```

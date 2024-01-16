# IMAGE\_THUNK\_DATA64

```csharp
public struct IMAGE_THUNK_DATA64
{
    public Anonymous Union;

    [StructLayout(LayoutKind.Explicit)]
    public struct Anonymous
    {
        [FieldOffset(0)]
        public ulong ForwarderString;

        [FieldOffset(0)]
        public ulong Function;

        [FieldOffset(0)]
        public ulong Ordinal;

        [FieldOffset(0)]
        public ulong AddressOfData;
    }
}
```

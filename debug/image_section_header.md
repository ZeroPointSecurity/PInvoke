# IMAGE\_SECTION\_HEADER

```csharp
public struct IMAGE_SECTION_HEADER
{
    [MarshalAs(UnmanagedType.LPUTF8Str, SizeConst = 8)]
    public string Name;

    public MiscUnion Misc;
    public uint VirtualAddress;
    public uint SizeOfRawData;
    public uint PointerToRawData;
    public uint PointerToRelocations;
    public uint PointerToLinenumbers;
    public ushort NumberOfRelocations;
    public ushort NumberOfLinenumbers;
    public IMAGE_SECTION_CHARACTERISTICS Characteristics;

    [StructLayout(LayoutKind.Explicit)]
    public struct MiscUnion
    {
        [FieldOffset(0)]
        public uint PhysicalAddress;

        [FieldOffset(0)]
        public uint VirtualSize;
    }
}
```

[image\_section\_characteristics.md](image\_section\_characteristics.md "mention")

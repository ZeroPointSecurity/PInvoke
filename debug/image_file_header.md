# IMAGE\_FILE\_HEADER

```csharp
public partial struct IMAGE_FILE_HEADER
{
    public IMAGE_FILE_MACHINE Machine;
    public ushort NumberOfSections;
    public uint TimeDateStamp;
    public uint PointerToSymbolTable;
    public uint NumberOfSymbols;
    public ushort SizeOfOptionalHeader;
    public IMAGE_FILE_CHARACTERISTICS Characteristics;
}
```

[image\_file\_machine.md](../system-information/image\_file\_machine.md "mention")

[image\_file\_characteristics.md](image\_file\_characteristics.md "mention")

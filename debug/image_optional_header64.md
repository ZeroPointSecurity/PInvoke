# IMAGE\_OPTIONAL\_HEADER64

```csharp
[StructLayout(LayoutKind.Sequential, Pack = 4)]
public struct IMAGE_OPTIONAL_HEADER64
{
    public IMAGE_OPTIONAL_HEADER_MAGIC Magic;
    public byte MajorLinkerVersion;
    public byte MinorLinkerVersion;
    public uint SizeOfCode;
    public uint SizeOfInitializedData;
    public uint SizeOfUninitializedData;
    public uint AddressOfEntryPoint;
    public uint BaseOfCode;
    public ulong ImageBase;
    public uint SectionAlignment;
    public uint FileAlignment;
    public ushort MajorOperatingSystemVersion;
    public ushort MinorOperatingSystemVersion;
    public ushort MajorImageVersion;
    public ushort MinorImageVersion;
    public ushort MajorSubsystemVersion;
    public ushort MinorSubsystemVersion;
    public uint Win32VersionValue;
    public uint SizeOfImage;
    public uint SizeOfHeaders;
    public uint CheckSum;
    public IMAGE_SUBSYSTEM Subsystem;
    public IMAGE_DLL_CHARACTERISTICS DllCharacteristics;
    public ulong SizeOfStackReserve;
    public ulong SizeOfStackCommit;
    public ulong SizeOfHeapReserve;
    public ulong SizeOfHeapCommit;

    [Obsolete]
    public uint LoaderFlags;

    public uint NumberOfRvaAndSizes;
    public IMAGE_DATA_DIRECTORY DataDirectory;
}
```

[image\_optional\_header\_magic.md](image\_optional\_header\_magic.md "mention")

[image\_subsystem.md](image\_subsystem.md "mention")

[image\_dll\_characteristics.md](image\_dll\_characteristics.md "mention")

[image\_data\_directory.md](image\_data\_directory.md "mention")

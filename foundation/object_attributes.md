# OBJECT\_ATTRIBUTES

```csharp
public unsafe struct OBJECT_ATTRIBUTES()
{
    public ulong Length = (ulong)Marshal.SizeOf<OBJECT_ATTRIBUTES>();
    public HANDLE RootDirectory;
    public UNICODE_STRING* ObjectName;
    public ulong Attributes;
    public void* SecurityDescriptor;
    public void* SecurityQualityOfService;
}
```

[unicode\_string.md](unicode\_string.md "mention")
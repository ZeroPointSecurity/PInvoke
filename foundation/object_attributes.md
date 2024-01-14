# OBJECT\_ATTRIBUTES

```csharp
public unsafe struct OBJECT_ATTRIBUTES
{
    public ulong Length;
    public HANDLE RootDirectory;
    public UNICODE_STRING* ObjectName;
    public ulong Attributes;
    public void* SecurityDescriptor;
    public void* SecurityQualityOfService;
}
```

[unicode\_string.md](unicode\_string.md "mention")

```csharp
//
// Valid values for the Attributes field
//
public const ulong OBJ_INHERIT = 0x00000002L;
public const ulong OBJ_PERMANENT = 0x00000010L;
public const ulong OBJ_EXCLUSIVE = 0x00000020L;
public const ulong OBJ_CASE_INSENSITIVE = 0x00000040L;
public const ulong OBJ_OPENIF = 0x00000080L;
public const ulong OBJ_OPENLINK = 0x00000100L;
public const ulong OBJ_KERNEL_HANDLE = 0x00000200L;
public const ulong OBJ_FORCE_ACCESS_CHECK = 0x00000400L;
public const ulong OBJ_IGNORE_IMPERSONATED_DEVICEMAP = 0x00000800L;
public const ulong OBJ_DONT_REPARSE = 0x00001000L;
public const ulong OBJ_VALID_ATTRIBUTES = 0x00001FF2L;
```

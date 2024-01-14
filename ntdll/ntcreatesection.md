# NtCreateSection

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtCreateSection(
    HANDLE* SectionHandle,
    uint DesiredAccess,
    [Optional] OBJECT_ATTRIBUTES* ObjectAttributes,
    [Optional] long* MaximumSize,
    uint SectionPageProtection,
    uint AllocationAttributes,
    [Optional] HANDLE FileHandle);
```

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[page\_protection\_flags.md](../memory/page\_protection\_flags.md "mention")

```csharp
// DesiredAccess
public const int SECTION_QUERY = 1;
public const int SECTION_MAP_WRITE = 2;
public const int SECTION_MAP_READ = 4;
public const int SECTION_MAP_EXECUTE = 8;
public const int SECTION_EXTEND_SIZE = 16;
public const int SECTION_MAP_EXECUTE_EXPLICIT = 32;

public const uint SECTION_ALL_ACCESS = STANDARD_RIGHTS_REQUIRED | SECTION_QUERY |
                                       SECTION_MAP_WRITE | SECTION_MAP_READ |
                                       SECTION_MAP_EXECUTE | SECTION_EXTEND_SIZE;
```

```csharp
// AllocationAttributes
public const uint SEC_COMMIT = 0x8000000;
public const uint SEC_IMAGE = 0x1000000;
public const uint SEC_IMAGE_NO_EXECUTE = 0x11000000;
public const uint SEC_LARGE_PAGES = 0x80000000;
public const uint SEC_NOCACHE = 0x10000000;
public const uint SEC_RESERVE = 0x4000000;
public const uint SEC_WRITECOMBINE = 0x40000000;
```

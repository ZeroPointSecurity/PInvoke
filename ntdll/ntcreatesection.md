# NtCreateSection

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtCreateSection(
    HANDLE* sectionHandle,
    ulong desiredAccess,
    [Optional] OBJECT_ATTRIBUTES* objectAttributes,
    [Optional] nuint* maximumSize,
    uint sectionPageProtection,
    uint allocationAttributes,
    [Optional] HANDLE fileHandle);
```

[access\_mask.md](../foundation/access\_mask.md "mention")

[object\_attributes.md](../foundation/object\_attributes.md "mention")

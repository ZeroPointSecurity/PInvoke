# NtCreateSection

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtCreateSection(
    HANDLE* sectionHandle,
    uint desiredAccess,
    [Optional] OBJECT_ATTRIBUTES* objectAttributes,
    [Optional] long* maximumSize,
    uint sectionPageProtection,
    uint allocationAttributes,
    [Optional] HANDLE fileHandle);
```

[object\_attributes.md](../foundation/object\_attributes.md "mention")

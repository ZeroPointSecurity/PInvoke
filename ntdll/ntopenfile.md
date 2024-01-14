# NtOpenFile

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtOpenFile(
    HANDLE* FileHandle,
    uint DesiredAccess,
    OBJECT_ATTRIBUTES* ObjectAttributes,
    IO_STATUS_BLOCK* IoStatusBlock,
    uint ShareAccess,
    uint OpenOptions);
```

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[io\_status\_block.md](../io/io\_status\_block.md "mention")

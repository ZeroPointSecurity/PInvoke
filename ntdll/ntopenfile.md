# NtOpenFile

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtOpenFile(
    HANDLE* FileHandle,
    ulong DesiredAccess,
    OBJECT_ATTRIBUTES* ObjectAttributes,
    IO_STATUS_BLOCK* IoStatusBlock,
    ulong ShareAccess,
    ulong OpenOptions);
```

[access\_mask.md](../foundation/access\_mask.md "mention")

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[io\_status\_block.md](../foundation/io\_status\_block.md "mention")

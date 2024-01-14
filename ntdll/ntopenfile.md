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

```csharp
// DesiredAccess
public const int FILE_READ_DATA = 1;
public const int FILE_WRITE_DATA = 2;
public const int FILE_APPEND_DATA = 4;
public const int FILE_READ_EA = 8;
public const int FILE_WRITE_EA = 16;
public const int FILE_EXECUTE = 32;
public const int FILE_READ_ATTRIBUTES = 128;
public const int FILE_WRITE_ATTRIBUTES = 256;
```

```csharp
// ShareAccess
public const int FILE_SHARE_READ = 1;
public const int FILE_SHARE_WRITE = 2;
public const int FILE_SHARE_DELETE = 4;
```

```csharp
// OpenOptions
public const int FILE_DIRECTORY_FILE = 1;
public const int FILE_WRITE_THROUGH = 2;
public const int FILE_SEQUENTIAL_ONLY = 4;
public const int FILE_NO_INTERMEDIATE_BUFFERING = 8;
public const int FILE_SYNCHRONOUS_IO_ALERT = 16;
public const int FILE_SYNCHRONOUS_IO_NONALERT = 32;
public const int FILE_NON_DIRECTORY_FILE = 64;
public const int FILE_CREATE_TREE_CONNECTION = 128;
public const int FILE_COMPLETE_IF_OPLOCKED = 256;
public const int FILE_NO_EA_KNOWLEDGE = 512;
public const int FILE_OPEN_REMOTE_INSTANCE = 1024;
public const int FILE_RANDOM_ACCESS = 2048;
public const int FILE_DELETE_ON_CLOSE = 4096;
public const int FILE_OPEN_BY_FILE_ID = 8192;
public const int FILE_OPEN_FOR_BACKUP_INTENT = 16384;
public const int FILE_NO_COMPRESSION = 32768;
public const int FILE_OPEN_REQUIRING_OPLOCK = 65536;
public const int FILE_DISALLOW_EXCLUSIVE = 131072;
public const int FILE_SESSION_AWARE = 262144;
public const int FILE_RESERVE_OPFILTER = 1048576;
public const int FILE_OPEN_REPARSE_POINT = 2097152;
public const int FILE_OPEN_NO_RECALL = 4194304;
public const int FILE_OPEN_FOR_FREE_SPACE_QUERY = 8388608;
public const int FILE_CONTAINS_EXTENDED_CREATE_INFORMATION = 268435456;
```

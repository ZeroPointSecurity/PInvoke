# ACCESS\_MASK

```csharp
public const ulong DELETE = 0x00010000L;
public const ulong READ_CONTROL = 0x00020000L;
public const ulong WRITE_DAC = 0x00040000L;
public const ulong WRITE_OWNER = 0x00080000L;
public const ulong SYNCHRONIZE = 0x00100000L;

public const ulong STANDARD_RIGHTS_REQUIRED = 0x000F0000L;
public const ulong STANDARD_RIGHTS_READ = READ_CONTROL;
public const ulong STANDARD_RIGHTS_WRITE = READ_CONTROL;
public const ulong STANDARD_RIGHTS_EXECUTE = READ_CONTROL;
public const ulong STANDARD_RIGHTS_ALL = 0x001F0000L;
public const ulong SPECIFIC_RIGHTS_ALL = 0x0000FFFFL;

public const ulong MAXIMUM_ALLOWED = 0x02000000L;

public const ulong GENERIC_READ = 0x80000000L;
public const ulong GENERIC_WRITE = 0x40000000L;
public const ulong GENERIC_EXECUTE = 0x20000000L;
public const ulong GENERIC_ALL = 0x10000000L;

public const uint PROCESS_TERMINATE = 0x0001;
public const uint PROCESS_CREATE_THREAD = 0x0002;
public const uint PROCESS_SET_SESSIONID = 0x0004;
public const uint PROCESS_VM_OPERATION = 0x0008;
public const uint PROCESS_VM_READ = 0x0010;
public const uint PROCESS_VM_WRITE = 0x0020;
public const uint PROCESS_DUP_HANDLE = 0x0040;
public const uint PROCESS_CREATE_PROCESS = 0x0080;
public const uint PROCESS_SET_QUOTA = 0x0100;
public const uint PROCESS_SET_INFORMATION = 0x0200;
public const uint PROCESS_QUERY_INFORMATION = 0x0400;
public const uint PROCESS_SUSPEND_RESUME = 0x0800;
public const uint PROCESS_QUERY_LIMITED_INFORMATION = 0x1000;
public const uint PROCESS_SET_LIMITED_INFORMATION = 0x2000;

public const ulong PROCESS_ALL_ACCESS = STANDARD_RIGHTS_REQUIRED |
                                        SYNCHRONIZE |
                                        0xFFFF;

public const uint SECTION_QUERY = 0x0001;
public const uint SECTION_MAP_WRITE = 0x0002;
public const uint SECTION_MAP_READ = 0x0004;
public const uint SECTION_MAP_EXECUTE = 0x0008;
public const uint SECTION_EXTEND_SIZE = 0x0010;
public const uint SECTION_MAP_EXECUTE_EXPLICIT = 0x0020;

public const ulong SECTION_ALL_ACCESS = STANDARD_RIGHTS_REQUIRED | 
                                        SECTION_QUERY |
                                        SECTION_MAP_WRITE |
                                        SECTION_MAP_READ |
                                        SECTION_MAP_EXECUTE | 
                                        SECTION_EXTEND_SIZE;

public const uint SEC_HUGE_PAGES = 0x00020000;
public const uint SEC_PARTITION_OWNER_HANDLE = 0x00040000;
public const uint SEC_64K_PAGES = 0x00080000;
public const uint SEC_FILE = 0x00800000;
public const uint SEC_IMAGE = 0x01000000;
public const uint SEC_PROTECTED_IMAGE = 0x02000000;
public const uint SEC_RESERVE = 0x04000000;
public const uint SEC_COMMIT = 0x08000000;
public const uint SEC_NOCACHE = 0x10000000;
public const uint SEC_WRITECOMBINE = 0x40000000;
public const uint SEC_LARGE_PAGES = 0x80000000;

public const uint SEC_IMAGE_NO_EXECUTE = SEC_IMAGE |
                                         SEC_NOCACHE;

public const uint FILE_READ_DATA = 0x0001;
public const uint FILE_LIST_DIRECTORY = 0x0001;
public const uint FILE_WRITE_DATA = 0x0002;
public const uint FILE_ADD_FILE = 0x0002;
public const uint FILE_APPEND_DATA = 0x0004;
public const uint FILE_ADD_SUBDIRECTORY = 0x0004;
public const uint FILE_CREATE_PIPE_INSTANCE = 0x0004;
public const uint FILE_READ_EA = 0x0008;
public const uint FILE_WRITE_EA = 0x0010;
public const uint FILE_EXECUTE = 0x0020;
public const uint FILE_TRAVERSE = 0x0020;
public const uint FILE_DELETE_CHILD = 0x0040;
public const uint FILE_READ_ATTRIBUTES = 0x0080;
public const uint FILE_WRITE_ATTRIBUTES = 0x0100;
public const ulong FILE_ALL_ACCESS = STANDARD_RIGHTS_REQUIRED |
                                     SYNCHRONIZE |
                                     0x1FF;

public const ulong FILE_GENERIC_READ = STANDARD_RIGHTS_READ |
                                       FILE_READ_DATA | 
                                       FILE_READ_ATTRIBUTES | 
                                       FILE_READ_EA |
                                       SYNCHRONIZE;

public const ulong FILE_GENERIC_WRITE = STANDARD_RIGHTS_WRITE |
                                        FILE_WRITE_DATA |
                                        FILE_WRITE_ATTRIBUTES |
                                        FILE_WRITE_EA |
                                        FILE_APPEND_DATA |
                                        SYNCHRONIZE;

public const ulong FILE_GENERIC_EXECUTE = STANDARD_RIGHTS_EXECUTE |
                                          FILE_READ_ATTRIBUTES |
                                          FILE_EXECUTE |
                                          SYNCHRONIZE;

public const uint FILE_SHARE_READ = 0x00000001;
public const uint FILE_SHARE_WRITE = 0x00000002;
public const uint FILE_SHARE_DELETE = 0x00000004;
public const uint FILE_ATTRIBUTE_READONLY = 0x00000001;
public const uint FILE_ATTRIBUTE_HIDDEN = 0x00000002;
public const uint FILE_ATTRIBUTE_SYSTEM = 0x00000004;
public const uint FILE_ATTRIBUTE_DIRECTORY = 0x00000010;
public const uint FILE_ATTRIBUTE_ARCHIVE = 0x00000020;
public const uint FILE_ATTRIBUTE_DEVICE = 0x00000040;
public const uint FILE_ATTRIBUTE_NORMAL = 0x00000080;
public const uint FILE_ATTRIBUTE_TEMPORARY = 0x00000100;
public const uint FILE_ATTRIBUTE_SPARSE_FILE = 0x00000200;
public const uint FILE_ATTRIBUTE_REPARSE_POINT = 0x00000400;
public const uint FILE_ATTRIBUTE_COMPRESSED = 0x00000800;
public const uint FILE_ATTRIBUTE_OFFLINE = 0x00001000;
public const uint FILE_ATTRIBUTE_NOT_CONTENT_INDEXED = 0x00002000;
public const uint FILE_ATTRIBUTE_ENCRYPTED = 0x00004000;
public const uint FILE_ATTRIBUTE_INTEGRITY_STREAM = 0x00008000;
public const uint FILE_ATTRIBUTE_VIRTUAL = 0x00010000;
public const uint FILE_ATTRIBUTE_NO_SCRUB_DATA = 0x00020000;
public const uint FILE_ATTRIBUTE_EA = 0x00040000;
public const uint FILE_ATTRIBUTE_PINNED = 0x00080000;
public const uint FILE_ATTRIBUTE_UNPINNED = 0x00100000;
public const uint FILE_ATTRIBUTE_RECALL_ON_OPEN = 0x00040000;
public const uint FILE_ATTRIBUTE_RECALL_ON_DATA_ACCESS = 0x00400000;
public const uint TREE_CONNECT_ATTRIBUTE_PRIVACY = 0x00004000;
public const uint TREE_CONNECT_ATTRIBUTE_INTEGRITY = 0x00008000;
public const uint TREE_CONNECT_ATTRIBUTE_GLOBAL = 0x00000004;
public const uint TREE_CONNECT_ATTRIBUTE_PINNED = 0x00000002;
public const uint FILE_ATTRIBUTE_STRICTLY_SEQUENTIAL = 0x20000000;
public const uint FILE_NOTIFY_CHANGE_FILE_NAME = 0x00000001;
public const uint FILE_NOTIFY_CHANGE_DIR_NAME = 0x00000002;
public const uint FILE_NOTIFY_CHANGE_ATTRIBUTES = 0x00000004;
public const uint FILE_NOTIFY_CHANGE_SIZE = 0x00000008;
public const uint FILE_NOTIFY_CHANGE_LAST_WRITE = 0x00000010;
public const uint FILE_NOTIFY_CHANGE_LAST_ACCESS = 0x00000020;
public const uint FILE_NOTIFY_CHANGE_CREATION = 0x00000040;
public const uint FILE_NOTIFY_CHANGE_SECURITY = 0x00000100;
public const uint FILE_ACTION_ADDED = 0x00000001;
public const uint FILE_ACTION_REMOVED = 0x00000002;
public const uint FILE_ACTION_MODIFIED = 0x00000003;
public const uint FILE_ACTION_RENAMED_OLD_NAME = 0x00000004;
public const uint FILE_ACTION_RENAMED_NEW_NAME = 0x00000005;
public const uint FILE_CASE_SENSITIVE_SEARCH = 0x00000001;
public const uint FILE_CASE_PRESERVED_NAMES = 0x00000002;
public const uint FILE_UNICODE_ON_DISK = 0x00000004;
public const uint FILE_PERSISTENT_ACLS = 0x00000008;
public const uint FILE_FILE_COMPRESSION = 0x00000010;
public const uint FILE_VOLUME_QUOTAS = 0x00000020;
public const uint FILE_SUPPORTS_SPARSE_FILES = 0x00000040;
public const uint FILE_SUPPORTS_REPARSE_POINTS = 0x00000080;
public const uint FILE_SUPPORTS_REMOTE_STORAGE = 0x00000100;
public const uint FILE_RETURNS_CLEANUP_RESULT_INFO = 0x00000200;
public const uint FILE_SUPPORTS_POSIX_UNLINK_RENAME = 0x00000400;
public const uint FILE_SUPPORTS_BYPASS_IO = 0x00000800;
public const uint FILE_SUPPORTS_STREAM_SNAPSHOTS = 0x00001000;
public const uint FILE_SUPPORTS_CASE_SENSITIVE_DIRS = 0x00002000;

public const uint FILE_VOLUME_IS_COMPRESSED = 0x00008000;
public const uint FILE_SUPPORTS_OBJECT_IDS = 0x00010000;
public const uint FILE_SUPPORTS_ENCRYPTION = 0x00020000;
public const uint FILE_NAMED_STREAMS = 0x00040000;
public const uint FILE_READ_ONLY_VOLUME = 0x00080000;
public const uint FILE_SEQUENTIAL_WRITE_ONCE = 0x00100000;
public const uint FILE_SUPPORTS_TRANSACTIONS = 0x00200000;
public const uint FILE_SUPPORTS_HARD_LINKS = 0x00400000;
public const uint FILE_SUPPORTS_EXTENDED_ATTRIBUTES = 0x00800000;
public const uint FILE_SUPPORTS_OPEN_BY_FILE_ID = 0x01000000;
public const uint FILE_SUPPORTS_USN_JOURNAL = 0x02000000;
public const uint FILE_SUPPORTS_INTEGRITY_STREAMS = 0x04000000;
public const uint FILE_SUPPORTS_BLOCK_REFCOUNTING = 0x08000000;
public const uint FILE_SUPPORTS_SPARSE_VDL = 0x10000000;
public const uint FILE_DAX_VOLUME = 0x20000000;
public const uint FILE_SUPPORTS_GHOSTING = 0x40000000;

public const uint FILE_DIRECTORY_FILE = 0x00000001;
public const uint FILE_WRITE_THROUGH = 0x00000002;
public const uint FILE_SEQUENTIAL_ONLY = 0x00000004;
public const uint FILE_NO_INTERMEDIATE_BUFFERING = 0x00000008;

public const uint FILE_SYNCHRONOUS_IO_ALERT = 0x00000010;
public const uint FILE_SYNCHRONOUS_IO_NONALERT = 0x00000020;
public const uint FILE_NON_DIRECTORY_FILE = 0x00000040;
public const uint FILE_CREATE_TREE_CONNECTION = 0x00000080;

public const uint FILE_COMPLETE_IF_OPLOCKED = 0x00000100;
public const uint FILE_NO_EA_KNOWLEDGE = 0x00000200;
public const uint FILE_OPEN_REMOTE_INSTANCE = 0x00000400;
public const uint FILE_RANDOM_ACCESS = 0x00000800;

public const uint FILE_DELETE_ON_CLOSE = 0x00001000;
public const uint FILE_OPEN_BY_FILE_ID = 0x00002000;
public const uint FILE_OPEN_FOR_BACKUP_INTENT = 0x00004000;
public const uint FILE_NO_COMPRESSION = 0x00008000;
```

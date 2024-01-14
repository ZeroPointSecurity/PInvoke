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
public const ulong FILE_ALL_ACCESS = STANDARD_RIGHTS_REQUIRED | SYNCHRONIZE | 0x1FF;

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
```

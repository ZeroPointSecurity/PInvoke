# OpenProcess

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern HANDLE OpenProcess(
    PROCESS_ACCESS_RIGHTS dwDesiredAccess, 
    BOOL bInheritHandle,
    uint dwProcessId);
```

[process\_access\_rights.md](../threading/process\_access\_rights.md "mention")

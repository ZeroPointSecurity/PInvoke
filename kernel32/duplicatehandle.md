# DuplicateHandle

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL DuplicateHandle(
    HANDLE hSourceProcessHandle,
    HANDLE hSourceHandle,
    HANDLE hTargetProcessHandle,
    HANDLE* lpTargetHandle,
    uint dwDesiredAccess,
    BOOL bInheritHandle,
    DUPLICATE_HANDLE_OPTIONS dwOptions);
```

[duplicate\_handle\_options.md](../foundation/duplicate\_handle\_options.md "mention")

# CreateFile

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, EntryPoint = "CreateFileW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateFile(
    PCWSTR lpFileName,
    uint dwDesiredAccess,
    FILE_SHARE_MODE dwShareMode,
    [Optional] SECURITY_ATTRIBUTES* lpSecurityAttributes,
    FILE_CREATION_DISPOSITION dwCreationDisposition,
    FILE_FLAGS_AND_ATTRIBUTES dwFlagsAndAttributes,
    HANDLE hTemplateFile);
```

[file\_share\_mode.md](../filesystem/file\_share\_mode.md "mention")

[file\_creation\_disposition.md](../filesystem/file\_creation\_disposition.md "mention")

[file\_flags\_and\_attributes.md](../filesystem/file\_flags\_and\_attributes.md "mention")

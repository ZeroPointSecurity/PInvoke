# NtOpenProcessToken

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtOpenProcessToken(
    HANDLE ProcessHandle,
    uint DesiredAccess,
    HANDLE* TokenHandle);
```

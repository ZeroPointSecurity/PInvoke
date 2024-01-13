# OpenProcessToken

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL OpenProcessToken(
    HANDLE ProcessHandle,
    TOKEN_ACCESS_MASK DesiredAccess,
    HANDLE* TokenHandle);
```

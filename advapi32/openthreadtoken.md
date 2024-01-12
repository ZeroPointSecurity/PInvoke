# OpenThreadToken

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL OpenThreadToken(
    HANDLE ThreadHandle,
    TOKEN_ACCESS_MASK DesiredAccess,
    BOOL OpenAsSelf,
    HANDLE* TokenHandle);
```

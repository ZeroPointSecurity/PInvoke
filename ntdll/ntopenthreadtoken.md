# NtOpenThreadToken

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtOpenThreadToken(
    HANDLE ThreadHandle,
    uint DesiredAccess,
    BOOL OpenAsSelf,
    HANDLE* TokenHandle);
```

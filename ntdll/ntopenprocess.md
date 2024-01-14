# NtOpenProcess

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtOpenProcess(
    HANDLE* ProcessHandle,
    uint DesiredAccess,
    OBJECT_ATTRIBUTES* ObjectAttributes,
    CLIENT_ID* ClientId);
```

[process\_access\_rights.md](../threading/process\_access\_rights.md "mention")

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[client\_id.md](../foundation/client\_id.md "mention")

# NtOpenProcess

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtOpenProcess(
    HANDLE* ProcessHandle,
    ACCESS_MASK DesiredAccess,
    OBJECT_ATTRIBUTES* ObjectAttributes,
    CLIENT_ID* ClientId);
```

[access\_mask.md](../foundation/access\_mask.md "mention")

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[client\_id.md](../foundation/client\_id.md "mention")

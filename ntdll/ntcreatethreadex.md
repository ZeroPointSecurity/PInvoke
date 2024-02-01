# NtCreateThreadEx



```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtCreateThreadEx(
    HANDLE* threadHandle,
    uint desiredAccess,
    [Optional] OBJECT_ATTRIBUTES* objectAttributes,
    HANDLE processHandle,
    USER_THREAD_START_ROUTINE startRoutine,
    [Optional] void* argument,
    uint createFlags,
    nuint zeroBits,
    nuint stackSize,
    nuint maximumStackSize,
    [Optional] PS_ATTRIBUTE_LIST* attributeList);
```

[object\_attributes.md](../foundation/object\_attributes.md "mention")

[user\_thread\_start\_routine.md](../foundation/user\_thread\_start\_routine.md "mention")

[ps\_attribute\_list.md](../foundation/ps\_attribute\_list.md "mention")

```csharp
// Desired Access
public const uint THREAD_CREATE_FLAGS_CREATE_SUSPENDED = 0x00000001;
public const uint THREAD_CREATE_FLAGS_SKIP_THREAD_ATTACH = 0x00000002;
public const uint THREAD_CREATE_FLAGS_HIDE_FROM_DEBUGGER = 0x00000004;
public const uint THREAD_CREATE_FLAGS_LOADER_WORKER = 0x00000010;
public const uint THREAD_CREATE_FLAGS_SKIP_LOADER_INIT = 0x00000020;
public const uint THREAD_CREATE_FLAGS_BYPASS_PROCESS_FREEZE = 0x00000040;
```

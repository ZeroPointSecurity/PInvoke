# AdjustTokenPrivileges

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL AdjustTokenPrivileges(
    HANDLE TokenHandle,
    BOOL DisableAllPrivileges,
    [Optional] TOKEN_PRIVILEGES* NewState,
    uint BufferLength,
    [Optional] TOKEN_PRIVILEGES* PreviousState,
    [Optional] uint* ReturnLength);
```

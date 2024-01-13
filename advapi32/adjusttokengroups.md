# AdjustTokenGroups

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL AdjustTokenGroups(
    HANDLE TokenHandle,
    BOOL ResetToDefault,
    [Optional] TOKEN_GROUPS* NewState,
    uint BufferLength,
    [Optional] TOKEN_GROUPS* PreviousState,
    [Optional] uint* ReturnLength);
```

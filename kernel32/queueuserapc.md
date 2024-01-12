# QueueUserAPC

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern uint QueueUserAPC(
    PAPCFUNC pfnAPC,
    HANDLE hThread,
    nuint dwData);
```

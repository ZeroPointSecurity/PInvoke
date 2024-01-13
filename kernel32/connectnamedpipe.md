# ConnectNamedPipe

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL ConnectNamedPipe(
    HANDLE hNamedPipe,
    [Optional] NativeOverlapped* lpOverlapped);
```

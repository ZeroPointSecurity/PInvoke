# CreatePipe

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CreatePipe(
    HANDLE* hReadPipe,
    HANDLE* hWritePipe,
    [Optional] SECURITY_ATTRIBUTES* lpPipeAttributes,
    uint nSize);
```

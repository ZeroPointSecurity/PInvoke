# PeekNamedPipe

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL PeekNamedPipe(
    HANDLE hNamedPipe,
    [Optional] void* lpBuffer,
    uint nBufferSize,
    [Optional] uint* lpBytesRead,
    [Optional] uint* lpTotalBytesAvail,
    [Optional] uint* lpBytesLeftThisMessage);
```

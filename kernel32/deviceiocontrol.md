# DeviceIoControl

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL DeviceIoControl(
    HANDLE hDevice,
    uint dwIoControlCode,
    [Optional] void* lpInBuffer,
    uint nInBufferSize,
    [Optional] void* lpOutBuffer,
    uint nOutBufferSize,
    [Optional] uint* lpBytesReturned,
    [Optional] NativeOverlapped* lpOverlapped);
```

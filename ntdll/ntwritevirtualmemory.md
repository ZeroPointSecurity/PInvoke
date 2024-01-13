# NtWriteVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtWriteVirtualMemory(
    HANDLE processHandle,
    void* baseAddress,
    void* buffer,
    nint bufferLength,
    nint* bytesWritten);
```

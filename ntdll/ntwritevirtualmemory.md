# NtWriteVirtualMemory

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS NtWriteVirtualMemory(
    HANDLE ProcessHandle,
    void* BaseAddress,
    void* Buffer,
    nint BufferLength,
    nint* BytesWritten);
```

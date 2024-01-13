# ReadProcessMemory

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL ReadProcessMemory(
    HANDLE hProcess,
    void* lpBaseAddress,
    void* lpBuffer,
    nuint nSize,
    [Optional] nuint* lpNumberOfBytesRead);
```

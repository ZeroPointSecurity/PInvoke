# LdrLoadDll

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LdrLoadDll(
    [Optional] char* PathToFile,
    [Optional] uint Flags,
    UNICODE_STRING* ModuleFileName,
    HANDLE* ModuleHandle);
```

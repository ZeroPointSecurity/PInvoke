# LdrUnloadDll

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LdrUnloadDll(
    HANDLE ModuleHandle);
```

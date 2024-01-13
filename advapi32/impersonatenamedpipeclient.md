# ImpersonateNamedPipeClient

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern BOOL ImpersonateNamedPipeClient(HANDLE hNamedPipe);
```

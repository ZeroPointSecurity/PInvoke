# DisconnectNamedPipe

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern BOOL DisconnectNamedPipe(HANDLE hNamedPipe);
```

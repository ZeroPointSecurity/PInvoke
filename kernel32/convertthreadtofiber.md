# ConvertThreadToFiber

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe void* ConvertThreadToFiber([Optional] void* lpParameter);
```

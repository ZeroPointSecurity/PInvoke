# CreateFiber

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe void* CreateFiber(
    nuint dwStackSize,
    LPFIBER_START_ROUTINE lpStartAddress,
    [Optional] void* lpParameter);
```

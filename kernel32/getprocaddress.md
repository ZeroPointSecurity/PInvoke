# GetProcAddress

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern FARPROC GetProcAddress(
    HMODULE hModule,
    PCSTR lpProcName);
```


# CreateMailslotW

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateMailslotW(
    PCWSTR lpName,
    uint nMaxMessageSize,
    uint lReadTimeout,
    [Optional] SECURITY_ATTRIBUTES* lpSecurityAttributes);
```

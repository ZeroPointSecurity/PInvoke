# CreateMailslot

```csharp
[DllImport("KERNEL32.dll", ExactSpelling = true, EntryPoint = "CreateMailslotW", SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HANDLE CreateMailslot(
    PCWSTR lpName,
    uint nMaxMessageSize,
    uint lReadTimeout,
    [Optional] SECURITY_ATTRIBUTES* lpSecurityAttributes);
```

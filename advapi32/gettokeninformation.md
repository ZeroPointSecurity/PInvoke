# GetTokenInformation

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL GetTokenInformation(
    HANDLE TokenHandle,
    TOKEN_INFORMATION_CLASS TokenInformationClass,
    [Optional] void* TokenInformation,
    uint TokenInformationLength,
    uint* ReturnLength);
```

[token\_information\_class.md](../security/token\_information\_class.md "mention")

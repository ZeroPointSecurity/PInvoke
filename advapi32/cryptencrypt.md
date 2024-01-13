# CryptEncrypt

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CryptEncrypt(
    nuint hKey,
    nuint hHash,
    BOOL Final,
    uint dwFlags,
    [Optional] byte* pbData,
    uint* pdwDataLen,
    uint dwBufLen);
```

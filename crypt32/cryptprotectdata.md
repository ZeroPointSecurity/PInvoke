# CryptProtectData

```csharp
[DllImport("CRYPT32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL CryptProtectData(
    CRYPT_INTEGER_BLOB* pDataIn,
    PCWSTR szDataDescr,
    [Optional] CRYPT_INTEGER_BLOB* pOptionalEntropy,
    [Optional] void* pvReserved,
    [Optional] CRYPTPROTECT_PROMPTSTRUCT* pPromptStruct,
    uint dwFlags,
    CRYPT_INTEGER_BLOB* pDataOut);

```

[crypt\_integer\_blob.md](../cryptography/crypt\_integer\_blob.md "mention")



Valid `dwFlags`:

```csharp
public const uint CRYPTPROTECT_LOCAL_MACHINE = 4U;
public const uint CRYPTPROTECT_UI_FORBIDDEN = 1U;
public const uint CRYPTPROTECT_AUDIT = 16U;
```

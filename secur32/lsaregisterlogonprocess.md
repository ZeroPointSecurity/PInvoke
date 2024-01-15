# LsaRegisterLogonProcess

```csharp
[DllImport("SECUR32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaRegisterLogonProcess(
    LSA_STRING* LogonProcessName,
    HANDLE* LsaHandle,
    uint* SecurityMode);
```

[lsa\_string.md](../authentication/lsa\_string.md "mention")

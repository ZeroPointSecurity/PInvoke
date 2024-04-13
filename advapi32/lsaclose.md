# LsaClose

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern NTSTATUS LsaClose(LSA_HANDLE ObjectHandle);
```

[ntstatus.md](../foundation/ntstatus.md "mention")

[lsa\_handle.md](../authentication/lsa\_handle.md "mention")

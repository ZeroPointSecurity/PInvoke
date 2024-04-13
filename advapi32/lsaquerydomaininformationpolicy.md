# LsaQueryDomainInformationPolicy

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS LsaQueryDomainInformationPolicy(
    LSA_HANDLE PolicyHandle,
    POLICY_DOMAIN_INFORMATION_CLASS InformationClass,
    void** Buffer);
```

[ntstatus.md](../foundation/ntstatus.md "mention")

[lsa\_handle.md](../authentication/lsa\_handle.md "mention")

[policy\_domain\_information\_class.md](../authentication/policy\_domain\_information\_class.md "mention")

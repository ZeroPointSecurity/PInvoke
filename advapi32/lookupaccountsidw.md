# LookupAccountSidW

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true, SetLastError = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe BOOL LookupAccountSidW(
    PCWSTR lpSystemName,
    PSID Sid,
    PWSTR Name,
    uint* cchName,
    PWSTR ReferencedDomainName,
    uint* cchReferencedDomainName,
    SID_NAME_USE* peUse);
```

{% content-ref url="../security/sid_name_use.md" %}
[sid\_name\_use.md](../security/sid_name_use.md)
{% endcontent-ref %}


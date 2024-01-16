# KERB\_TICKET\_CACHE\_INFO\_EX

```csharp
public struct KERB_TICKET_CACHE_INFO_EX
{
    public LSA_UNICODE_STRING ClientName;
    public LSA_UNICODE_STRING ClientRealm;
    public LSA_UNICODE_STRING ServerName;
    public LSA_UNICODE_STRING ServerRealm;
    public long StartTime;
    public long EndTime;
    public long RenewTime;
    public int EncryptionType;
    public uint TicketFlags;
}
```

[lsa\_unicode\_string.md](../authentication/lsa\_unicode\_string.md "mention")

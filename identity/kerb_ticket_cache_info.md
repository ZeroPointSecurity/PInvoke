# KERB\_TICKET\_CACHE\_INFO

```csharp
public struct KERB_TICKET_CACHE_INFO
{
    public LSA_UNICODE_STRING ServerName;
    public LSA_UNICODE_STRING RealmName;
    public long StartTime;
    public long EndTime;
    public long RenewTime;
    public int EncryptionType;
    public KERB_TICKET_FLAGS TicketFlags;
}
```

[lsa\_unicode\_string.md](../authentication/lsa\_unicode\_string.md "mention")

[kerb\_ticket\_flags.md](kerb\_ticket\_flags.md "mention")

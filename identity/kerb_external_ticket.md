# KERB\_EXTERNAL\_TICKET

```csharp
public partial struct KERB_EXTERNAL_TICKET
{
    public unsafe KERB_EXTERNAL_NAME* ServiceName;
    public unsafe KERB_EXTERNAL_NAME* TargetName;
    public unsafe KERB_EXTERNAL_NAME* ClientName;
    public LSA_UNICODE_STRING DomainName;
    public LSA_UNICODE_STRING TargetDomainName;
    public LSA_UNICODE_STRING AltTargetDomainName;
    public KERB_CRYPTO_KEY SessionKey;
    public KERB_TICKET_FLAGS TicketFlags;
    public uint Flags;
    public long KeyExpirationTime;
    public long StartTime;
    public long EndTime;
    public long RenewUntil;
    public long TimeSkew;
    public uint EncodedTicketSize;
    public unsafe byte* EncodedTicket;
}
```

[kerb\_external\_name.md](kerb\_external\_name.md "mention")

[lsa\_unicode\_string.md](../authentication/lsa\_unicode\_string.md "mention")

[kerb\_crypto\_key.md](kerb\_crypto\_key.md "mention")

[kerb\_ticket\_flags.md](kerb\_ticket\_flags.md "mention")

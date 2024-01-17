# KERB\_RETRIEVE\_TKT\_REQUEST

```csharp
public struct KERB_RETRIEVE_TKT_REQUEST
{
    public KERB_PROTOCOL_MESSAGE_TYPE MessageType;
    public LUID LogonId;
    public LSA_UNICODE_STRING TargetName;
    public uint TicketFlags;
    public uint CacheOptions;
    public KERB_CRYPTO_KEY_TYPE EncryptionType;
    public SecHandle CredentialsHandle;
}
```

[kerb\_protocol\_message\_type.md](kerb\_protocol\_message\_type.md "mention")

[luid.md](../foundation/luid.md "mention")

[lsa\_unicode\_string.md](../authentication/lsa\_unicode\_string.md "mention")

[kerb\_crypto\_key\_type.md](kerb\_crypto\_key\_type.md "mention")

[sechandle.md](../security/sechandle.md "mention")

```csharp
// CacheOptions
public const uint KERB_RETRIEVE_TICKET_DEFAULT = 0U;
public const uint KERB_RETRIEVE_TICKET_DONT_USE_CACHE = 1U;
public const uint KERB_RETRIEVE_TICKET_USE_CACHE_ONLY = 2U;
public const uint KERB_RETRIEVE_TICKET_USE_CREDHANDLE = 4U;
public const uint KERB_RETRIEVE_TICKET_AS_KERB_CRED = 8U;
public const uint KERB_RETRIEVE_TICKET_WITH_SEC_CRED = 16U;
public const uint KERB_RETRIEVE_TICKET_CACHE_TICKET = 32U;
public const uint KERB_RETRIEVE_TICKET_MAX_LIFETIME = 64U;
```

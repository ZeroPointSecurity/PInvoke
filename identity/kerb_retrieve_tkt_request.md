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

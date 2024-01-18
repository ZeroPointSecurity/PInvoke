# KERB\_SUBMIT\_TKT\_REQUEST

```csharp
public struct KERB_SUBMIT_TKT_REQUEST
{
    public KERB_PROTOCOL_MESSAGE_TYPE MessageType;
    public LUID LogonId;
    public uint Flags;
    public KERB_CRYPTO_KEY32 Key;
    public uint KerbCredSize;
    public uint KerbCredOffset;
}
```

[kerb\_protocol\_message\_type.md](kerb\_protocol\_message\_type.md "mention")

[kerb\_crypto\_key32.md](kerb\_crypto\_key32.md "mention")

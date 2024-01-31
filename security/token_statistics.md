# TOKEN\_STATISTICS

```csharp
public struct TOKEN_STATISTICS
{
    public LUID TokenId;
    public LUID AuthenticationId;
    public long ExpirationTime;
    public TOKEN_TYPE TokenType;
    public SECURITY_IMPERSONATION_LEVEL ImpersonationLevel;
    public uint DynamicCharged;
    public uint DynamicAvailable;
    public uint GroupCount;
    public uint PrivilegeCount;
    public LUID ModifiedId;
}
```

[token\_type.md](token\_type.md "mention")

[security\_impersonation\_level.md](security\_impersonation\_level.md "mention")

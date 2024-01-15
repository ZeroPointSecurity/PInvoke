# SECURITY\_LOGON\_SESSION\_DATA

```csharp
public partial struct SECURITY_LOGON_SESSION_DATA
{
    public uint Size;
    public LUID LogonId;
    public LSA_UNICODE_STRING UserName;
    public LSA_UNICODE_STRING LogonDomain;
    public LSA_UNICODE_STRING AuthenticationPackage;
    public uint LogonType;
    public uint Session;
    public PSID Sid;
    public long LogonTime;
    public LSA_UNICODE_STRING LogonServer;
    public LSA_UNICODE_STRING DnsDomainName;
    public LSA_UNICODE_STRING Upn;
    public uint UserFlags;
    public LSA_LAST_INTER_LOGON_INFO LastLogonInfo;
    public LSA_UNICODE_STRING LogonScript;
    public LSA_UNICODE_STRING ProfilePath;
    public LSA_UNICODE_STRING HomeDirectory;
    public LSA_UNICODE_STRING HomeDirectoryDrive;
    public long LogoffTime;
    public long KickOffTime;
    public long PasswordLastSet;
    public long PasswordCanChange;
    public long PasswordMustChange;
}
```

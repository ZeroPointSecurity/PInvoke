# NAMED\_PIPE\_MODE

```csharp
[Flags]
public enum NAMED_PIPE_MODE : uint
{
    PIPE_WAIT = 0x00000000,
    PIPE_NOWAIT = 0x00000001,
    PIPE_READMODE_BYTE = 0x00000000,
    PIPE_READMODE_MESSAGE = 0x00000002,
    PIPE_CLIENT_END = 0x00000000,
    PIPE_SERVER_END = 0x00000001,
    PIPE_TYPE_BYTE = 0x00000000,
    PIPE_TYPE_MESSAGE = 0x00000004,
    PIPE_ACCEPT_REMOTE_CLIENTS = 0x00000000,
    PIPE_REJECT_REMOTE_CLIENTS = 0x00000008,
}
```

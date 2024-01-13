# SERVICE\_STATUS

```csharp
public struct SERVICE_STATUS
{
    public ENUM_SERVICE_TYPE dwServiceType;
    public SERVICE_STATUS_CURRENT_STATE dwCurrentState;
    public uint dwControlsAccepted;
    public uint dwWin32ExitCode;
    public uint dwServiceSpecificExitCode;
    public uint dwCheckPoint;
    public uint dwWaitHint;
}
```

[enum\_service\_type.md](enum\_service\_type.md "mention")

[service\_status\_current\_state.md](service\_status\_current\_state.md "mention")

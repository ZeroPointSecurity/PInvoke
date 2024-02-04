# PROCESS\_BASIC\_INFORMATION

```csharp
public struct PROCESS_BASIC_INFORMATION
{
    public NTSTATUS ExitStatus;
    public unsafe void* PebBaseAddress;
    public nuint AffinityMask;
    public int BasePriority;
    public nuint UniqueProcessId;
    public nuint InheritedFromUniqueProcessId;
}
```

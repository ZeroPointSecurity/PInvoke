# SecBufferDesc

```csharp
public struct SecBufferDesc
{
    public uint ulVersion;
    public uint cBuffers;
    public unsafe SecBuffer* pBuffers;
}
```

[secbuffer.md](secbuffer.md "mention")

# PCSTR

```csharp
[DebuggerDisplay("{" + nameof(DebuggerDisplay) + "}")]
public readonly unsafe struct PCSTR : IEquatable<PCSTR>
{
    public readonly byte* Value;

    public PCSTR(byte* value) => Value = value;

    public static implicit operator byte*(PCSTR value) => value.Value;

    public static explicit operator PCSTR(byte* value) => new(value);

    public bool Equals(PCSTR other) => Value == other.Value;

    public override bool Equals(object obj) => obj is PCSTR other && Equals(other);

    public override int GetHashCode() => (int)Value;

    public int Length
    {
        get
        {
            var p = Value;
                
            if (p is null)
                return 0;
                
            while (*p != 0)
                p++;
                
            return checked((int)(p - Value));
        }
    }
        
    public override string ToString() => Value is null ? string.Empty : new string((sbyte*)Value, 0, Length, System.Text.Encoding.Default);

    public ReadOnlySpan<byte> AsSpan() => Value is null ? default : new ReadOnlySpan<byte>(Value, Length);

    private string DebuggerDisplay => ToString();
}
```

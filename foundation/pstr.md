# PSTR

```csharp
[DebuggerDisplay("{Value}")]
public readonly unsafe struct PSTR : IEquatable<PSTR>
{
    public readonly byte* Value;

    public PSTR(byte* value) => Value = value;

    public static implicit operator byte*(PSTR value) => value.Value;

    public static implicit operator PSTR(byte* value) => new(value);

    public static bool operator ==(PSTR left, PSTR right) => left.Value == right.Value;

    public static bool operator !=(PSTR left, PSTR right) => !(left == right);

    public bool Equals(PSTR other) => Value == other.Value;

    public override bool Equals(object obj) => obj is PSTR other && Equals(other);

    public override int GetHashCode() => (int)Value;
        
    public override string ToString() => new PCSTR(Value).ToString();

    public static implicit operator PCSTR(PSTR value) => new(value.Value);

    public int Length => new PCSTR(Value).Length;

    public Span<byte> AsSpan() => Value is null ? default : new Span<byte>(Value, Length);

    private string DebuggerDisplay => ToString();
}
```

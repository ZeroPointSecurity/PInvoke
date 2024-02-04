# BOOLEAN

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct BOOLEAN : IEquatable<BOOLEAN>
{
    public readonly byte Value;

    public BOOLEAN(byte value) => Value = value;

    public static implicit operator byte(BOOLEAN value) => value.Value;

    public static explicit operator BOOLEAN(byte value) => new(value);

    public static bool operator ==(BOOLEAN left, BOOLEAN right) => left.Value == right.Value;

    public static bool operator !=(BOOLEAN left, BOOLEAN right) => !(left == right);

    public bool Equals(BOOLEAN other) => Value == other.Value;

    public override bool Equals(object obj) => obj is BOOLEAN other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => $"0x{Value:x}";

    public BOOLEAN(bool value) => Value = value ? (byte)1 : (byte)0;

    public static implicit operator bool(BOOLEAN value) => value.Value != 0;

    public static implicit operator BOOLEAN(bool value) => new(value);
}
```

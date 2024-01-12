# BOOL

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct BOOL(int value) : IEquatable<BOOL>
{
    public readonly int Value = value;

    public static implicit operator int(BOOL value) => value.Value;

    public static explicit operator BOOL(int value) => new(value);

    public static bool operator ==(BOOL left, BOOL right) => left.Value == right.Value;

    public static bool operator !=(BOOL left, BOOL right) => !(left == right);

    public bool Equals(BOOL other) => Value == other.Value;

    public override bool Equals(object obj) => obj is BOOL other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => $"0x{Value:x}";

    public BOOL(bool value) : this(value ? 1 : 0) { }

    public static implicit operator bool(BOOL value) => value.Value != 0;

    public static implicit operator BOOL(bool value) => new(value);
}
```

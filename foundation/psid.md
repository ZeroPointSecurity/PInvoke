# PSID

```csharp
[DebuggerDisplay("{Value}")]
public readonly unsafe struct PSID : IEquatable<PSID>
{
    public readonly void* Value;

    public PSID(void* value) => Value = value;

    public static implicit operator void*(PSID value) => value.Value;

    public static explicit operator PSID(void* value) => new(value);

    public static bool operator ==(PSID left, PSID right) => left.Value == right.Value;

    public static bool operator !=(PSID left, PSID right) => !(left == right);

    public bool Equals(PSID other) => Value == other.Value;

    public override bool Equals(object obj) => obj is PSID other && Equals(other);

    public override int GetHashCode() => unchecked((int)Value);

    public override string ToString() => $"0x{(nuint)Value:x}";
}
```

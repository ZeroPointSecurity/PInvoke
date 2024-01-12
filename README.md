# Handle

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct Handle(IntPtr value) : IEquatable<Handle>
{
    public readonly IntPtr Value = value;

    public static Handle Null => default;

    public bool IsNull => Value == default;

    public static implicit operator IntPtr(Handle value) => value.Value;

    public static explicit operator Handle(IntPtr value) => new(value);

    public static bool operator == (Handle left, Handle right) => left.Value == right.Value;

    public static bool operator != (Handle left, Handle right) => !(left == right);

    public bool Equals(Handle other) => Value == other.Value;

    public override bool Equals(object obj) => obj is Handle other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => $"0x{Value:x}";
}
```

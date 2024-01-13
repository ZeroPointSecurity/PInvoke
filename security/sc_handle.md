# SC\_HANDLE

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct SC_HANDLE : IEquatable<SC_HANDLE>
{
    public readonly nint Value;

    public SC_HANDLE(nint value) => Value = value;

    public static implicit operator nint(SC_HANDLE value) => value.Value;

    public static explicit operator SC_HANDLE(nint value) => new(value);

    public static bool operator ==(SC_HANDLE left, SC_HANDLE right) => left.Value == right.Value;

    public static bool operator !=(SC_HANDLE left, SC_HANDLE right) => !(left == right);

    public bool Equals(SC_HANDLE other) => Value == other.Value;

    public override bool Equals(object obj) => obj is SC_HANDLE other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => $"0x{Value:x}";
}
```

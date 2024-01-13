# HMODULE

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct HMODULE : IEquatable<HMODULE>
{
    public readonly IntPtr Value;

    public HMODULE(IntPtr value) => Value = value;

    public static HMODULE Null => default;

    public bool IsNull => Value == default;

    public static implicit operator IntPtr(HMODULE value) => value.Value;

    public static explicit operator HMODULE(IntPtr value) => new(value);

    public static bool operator ==(HMODULE left, HMODULE right) => left.Value == right.Value;

    public static bool operator !=(HMODULE left, HMODULE right) => !(left == right);

    public bool Equals(HMODULE other) => Value == other.Value;

    public override bool Equals(object obj) => obj is HMODULE other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => $"0x{Value:x}";

    public static implicit operator HINSTANCE(HMODULE value) => new(value.Value);
}
```

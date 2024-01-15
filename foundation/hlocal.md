# HLOCAL

```csharp
[DebuggerDisplay("{Value}")]
public readonly unsafe struct HLOCAL : IEquatable<HLOCAL>
{
    public readonly void* Value;

    public HLOCAL(void* value) => Value = value;

    public static implicit operator void*(HLOCAL value) => value.Value;

    public static explicit operator HLOCAL(void* value) => new(value);

    public static bool operator ==(HLOCAL left, HLOCAL right) => left.Value == right.Value;

    public static bool operator !=(HLOCAL left, HLOCAL right) => !(left == right);

    public bool Equals(HLOCAL other) => Value == other.Value;

    public override bool Equals(object obj) => obj is HLOCAL other && Equals(other);

    public override int GetHashCode() => (int)Value;

    public override string ToString() => $"0x{(nuint)Value:x}";

    public static implicit operator IntPtr(HLOCAL value) => new(value.Value);

    public static explicit operator HLOCAL(IntPtr value) => new(value.ToPointer());

    public static explicit operator HLOCAL(UIntPtr value) => new(value.ToPointer());
}
```

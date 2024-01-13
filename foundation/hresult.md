## HRESULT

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct HRESULT : IEquatable<HRESULT>
{
    public readonly int Value;

    public HRESULT(int value) => Value = value;

    public static implicit operator int(HRESULT value) => value.Value;

    public static explicit operator HRESULT(int value) => new(value);

    public static bool operator ==(HRESULT left, HRESULT right) => left.Value == right.Value;

    public static bool operator !=(HRESULT left, HRESULT right) => !(left == right);

    public bool Equals(HRESULT other) => Value == other.Value;

    public override bool Equals(object obj) => obj is HRESULT other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => string.Format(System.Globalization.CultureInfo.InvariantCulture, "0x{0:X8}", Value);

    public static implicit operator uint(HRESULT value) => (uint)value.Value;

    public static explicit operator HRESULT(uint value) => new((int)value);

    [DebuggerBrowsable(DebuggerBrowsableState.Never)]
    public bool Succeeded => Value >= 0;

    [DebuggerBrowsable(DebuggerBrowsableState.Never)]
    public bool Failed => Value < 0;

    public HRESULT ThrowOnFailure(IntPtr errorInfo = default)
    {
        Marshal.ThrowExceptionForHR(Value, errorInfo);
        return this;
    }

    public string ToString(string format, IFormatProvider formatProvider) => ((uint)Value).ToString(format, formatProvider);
}
```

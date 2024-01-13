# PCWSTR

```csharp
[DebuggerDisplay("{" + nameof(DebuggerDisplay) + "}")]
public readonly unsafe struct PCWSTR : IEquatable<PCWSTR>
{
    public readonly char* Value;

    public PCWSTR(char* value) => Value = value;

    public static explicit operator char*(PCWSTR value) => value.Value;

    public static implicit operator PCWSTR(char* value) => new(value);

    public bool Equals(PCWSTR other) => Value == other.Value;

    public override bool Equals(object obj) => obj is PCWSTR other && Equals(other);

    public override int GetHashCode() => unchecked((int)Value);

    public int Length
    {
        get
        {
            var p = Value;
            
            if (p is null)
                return 0;
            
            while (*p != '\0')
                p++;
            
            return checked((int)(p - Value));
        }
    }

    public override string ToString() => Value is null ? null : new string(Value);

    public ReadOnlySpan<char> AsSpan() => Value is null ? default : new ReadOnlySpan<char>(Value, Length);

    private string DebuggerDisplay => ToString();
}
```

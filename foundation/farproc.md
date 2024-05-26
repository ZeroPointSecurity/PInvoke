# FARPROC

```csharp
public struct FARPROC
{
    public IntPtr Value;

    public FARPROC(IntPtr value) => Value = value;

    public static FARPROC Null => default;

    public bool IsNull => Value == default;

    public static implicit operator IntPtr(FARPROC value) => value.Value;

    public static explicit operator FARPROC(IntPtr value) => new(value);

    public static bool operator ==(FARPROC left, FARPROC right) => left.Value == right.Value;

    public static bool operator !=(FARPROC left, FARPROC right) => !(left == right);

    public bool Equals(FARPROC other) => Value == other.Value;

    public override bool Equals(object obj) => obj is FARPROC other && Equals(other);

    public override int GetHashCode() => Value.GetHashCode();

    public override string ToString() => $"0x{Value:x}";

    public TDelegate CreateDelegate<TDelegate>() where TDelegate : Delegate =>
        Marshal.GetDelegateForFunctionPointer<TDelegate>(Value);
}
```

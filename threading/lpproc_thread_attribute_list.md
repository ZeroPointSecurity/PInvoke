# LPPROC\_THREAD\_ATTRIBUTE\_LIST

```csharp
[DebuggerDisplay("{Value}")]
public readonly unsafe struct LPPROC_THREAD_ATTRIBUTE_LIST : IEquatable<LPPROC_THREAD_ATTRIBUTE_LIST>
{
    public readonly void* Value;

    public LPPROC_THREAD_ATTRIBUTE_LIST(void* value) => Value = value;

    public static implicit operator void*(LPPROC_THREAD_ATTRIBUTE_LIST value) => value.Value;

    public static explicit operator LPPROC_THREAD_ATTRIBUTE_LIST(void* value) => new(value);

    public static bool operator ==(LPPROC_THREAD_ATTRIBUTE_LIST left, LPPROC_THREAD_ATTRIBUTE_LIST right) => left.Value == right.Value;

    public static bool operator !=(LPPROC_THREAD_ATTRIBUTE_LIST left, LPPROC_THREAD_ATTRIBUTE_LIST right) => !(left == right);

    public bool Equals(LPPROC_THREAD_ATTRIBUTE_LIST other) => Value == other.Value;

    public override bool Equals(object obj) => obj is LPPROC_THREAD_ATTRIBUTE_LIST other && Equals(other);

    public override int GetHashCode() => (int)Value;

    public override string ToString() => $"0x{(nuint)Value:x}";
}
```

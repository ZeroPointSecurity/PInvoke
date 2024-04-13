# LSA\_HANDLE

```csharp
[DebuggerDisplay("{Value}")]
public readonly partial struct LSA_HANDLE: IEquatable<LSA_HANDLE>
{
	public readonly IntPtr Value;
	public LSA_HANDLE(IntPtr value) => this.Value = value;
	public static LSA_HANDLE Null => default;
	public bool IsNull => Value == default;
	public static implicit operator IntPtr(LSA_HANDLE value) => value.Value;
	public static explicit operator LSA_HANDLE(IntPtr value) => new LSA_HANDLE(value);
	public static bool operator ==(LSA_HANDLE left, LSA_HANDLE right) => left.Value == right.Value;
	public static bool operator !=(LSA_HANDLE left, LSA_HANDLE right) => !(left == right);
	public bool Equals(LSA_HANDLE other) => this.Value == other.Value;
	public override bool Equals(object obj) => obj is LSA_HANDLE other && this.Equals(other);
	public override int GetHashCode() => this.Value.GetHashCode();
	public override string ToString() => $"0x{thisalue:x}";
}
```

# HWND

```csharp
[DebuggerDisplay("{Value}")]
public readonly struct HWND : IEquatable<HWND>
{
    public readonly IntPtr Value;
    
    public HWND(IntPtr value) => this.Value = value;
    
    public static HWND Null => default;
    
    public bool IsNull => Value == default;
    
    public static implicit operator IntPtr(HWND value) => value.Value;
    
    public static explicit operator HWND(IntPtr value) => new HWND(value);
    
    public static bool operator ==(HWND left, HWND right) => left.Value == right.Value;
    
    public static bool operator !=(HWND left, HWND right) => !(left == right);
    
    public bool Equals(HWND other) => this.Value == other.Value;
    
    public override bool Equals(object obj) => obj is HWND other && this.Equals(other);
    
    public override int GetHashCode() => this.Value.GetHashCode();
    
    public override string ToString() => $"0x{this.Value:x}";
    
    public static implicit operator HANDLE(HWND value) => new HANDLE(value.Value);
}
```

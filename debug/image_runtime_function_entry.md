# IMAGE\_RUNTIME\_FUNCTION\_ENTRY

```csharp
public struct IMAGE_RUNTIME_FUNCTION_ENTRY
{
	public uint BeginAddress;
	public uint EndAddress;
	public Anonymous Anonymous;

	[StructLayout(LayoutKind.Explicit)]
	public struct Anonymous
	{
		[FieldOffset(0)]
		public uint UnwindInfoAddress;

		[FieldOffset(0)]
		public uint UnwindData;
	}
}
```
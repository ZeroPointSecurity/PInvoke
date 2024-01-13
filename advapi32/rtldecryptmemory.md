# RtlDecryptMemory

```csharp
[DllImport("ADVAPI32.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe NTSTATUS RtlDecryptMemory(
    void* Memory,
    uint MemorySize,
    uint OptionFlags);
```

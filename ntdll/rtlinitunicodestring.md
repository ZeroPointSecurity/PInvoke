# RtlInitUnicodeString

```csharp
[DllImport("ntdll.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe void RtlInitUnicodeString(
    UNICODE_STRING* DestinationString,
    PCWSTR SourceString);
```

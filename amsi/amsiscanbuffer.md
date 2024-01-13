## AmsiScanBuffer

```csharp
[DllImport("Amsi.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT AmsiScanBuffer(
    HAMSICONTEXT amsiContext,
    void* buffer,
    uint length,
    PCWSTR contentName,
    HAMSISESSION amsiSession,
    AMSI_RESULT* result);
```

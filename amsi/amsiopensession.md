## AmsiOpenSession

```csharp
[DllImport("Amsi.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT AmsiOpenSession(
    HAMSICONTEXT amsiContext,
    HAMSISESSION* amsiSession);
```

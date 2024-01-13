## AmsiCloseSession

```csharp
[DllImport("Amsi.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern void AmsiCloseSession(
    HAMSICONTEXT amsiContext,
    HAMSISESSION amsiSession);
```

# AmsiInitialize

```csharp
[DllImport("Amsi.dll", ExactSpelling = true)]
[DefaultDllImportSearchPaths(DllImportSearchPath.System32)]
public static extern unsafe HRESULT AmsiInitialize(
    PCWSTR appName,
    HAMSICONTEXT* amsiContext);
```

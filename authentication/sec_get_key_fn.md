# SEC\_GET\_KEY\_FN

```csharp
[UnmanagedFunctionPointerAttribute(CallingConvention.Winapi)]
public unsafe delegate void SEC_GET_KEY_FN(
    void* Arg,
    void* Principal,
    uint KeyVer,
    void** Key,
    HRESULT* Status);
```

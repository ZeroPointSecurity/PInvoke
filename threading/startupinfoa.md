# STARTUPINFOA

```csharp
public struct STARTUPINFOA
{
    public uint cb;
    public PSTR lpReserved;
    public PSTR lpDesktop;
    public PSTR lpTitle;
    public uint dwX;
    public uint dwY;
    public uint dwXSize;
    public uint dwYSize;
    public uint dwXCountChars;
    public uint dwYCountChars;
    public uint dwFillAttribute;
    public STARTUPINFO_FLAGS dwFlags;
    public ushort wShowWindow;
    public ushort cbReserved2;
    public unsafe byte* lpReserved2;
    public HANDLE hStdInput;
    public HANDLE hStdOutput;
    public HANDLE hStdError;
}
```

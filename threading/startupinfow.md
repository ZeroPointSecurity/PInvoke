# STARTUPINFOW

```csharp
public struct STARTUPINFOW
{
    public uint cb;
    public PWSTR lpReserved;
    public PWSTR lpDesktop;
    public PWSTR lpTitle;
    public uint dwX;
    public uint dwY;
    public uint dwXSize;
    public uint dwYSize;
    public uint dwXCountChars;
    public uint dwYCountChars;
    public uint dwFillAttribute;
    public STARTUPINFOW_FLAGS dwFlags;
    public ushort wShowWindow;
    public ushort cbReserved2;
    public unsafe byte* lpReserved2;
    public HANDLE hStdInput;
    public HANDLE hStdOutput;
    public HANDLE hStdError;
}
```

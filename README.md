# Iscsicpl UAC Bypass

When a 32bit Microsoft binary is launched on a 64bit system through SysWOW64, a DLL Order hijacking vulnerability affecting the `iscsicpl.exe` binary.


The 32-bit binary will look for the DLL iscsiexe.dll in `user/%Path%`.


As autoelevate is enabled, this can be abused by utilizing a proxy DLL to execute code through `iscsicpl.exe`.

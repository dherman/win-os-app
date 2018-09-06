# minimal demonstration of os_info link error

this demo app fails to build with 32-bit msvc; it has a linker error that looks like:

```
  = note: libos_info-4d3a0afa4b4f8187.rlib(os_info-4d3a0afa4b4f8187.os_info3.rcgu.o) : error LNK2019: unresolved external symbol __imp__RtlGetVersion referenced in function __ZN7os_info3imp6winapi16get_version_info17hec01399a17427c2bE
            C:\Users\dherman\Sources\Bash\win-os-app\target\debug\deps\win_os_app-e0e18894295fc8cd.exe : fatal error LNK1120: 1 unresolved externals
```

you should also be able to see this in appveyor


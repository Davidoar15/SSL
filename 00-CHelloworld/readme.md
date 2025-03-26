## Compilador
`gcc --version`
gcc.exe (Rev2, Built by MSYS2 project) 14.2.0

## Versión de C
`gcc -dM -E -x c /dev/null | findstr __STDC_VERSION__`
#define __STDC_VERSION__ 201710L (C17, también llamado C18 o C1x, formalmente ISO/IEC 9899:2018)

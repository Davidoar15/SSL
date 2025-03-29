# Compilador
`gcc --version`

gcc.exe (Rev2, Built by MSYS2 project) 14.2.0

# Versión de C
`gcc -dM -E -x c /dev/null | findstr __STDC_VERSION__`

#define __STDC_VERSION__ 201710L (C17, también llamado C18 o C1x, formalmente ISO/IEC 9899:2018)

`gcc -std=c2x -E -dM -x c nul | findstr __STDC_VERSION__` #define __STDC_VERSION__ 202000L

`gcc -std=c23 -E -dM -x c nul | findstr __STDC_VERSION__` #define __STDC_VERSION__ 202000L

(Soporta C23)

# Secuencia realizada:

1. Se crea el archivo "hello.c" y se escribe un código que imprime `Hello World!`.
2. Se compila el archivo "hello.c" y se genera "hello.exe" ejecutando `gcc hello.c -o hello.exe`.
3. Se ejecuta `./hello.exe` e imprime "Hello World!" en consola.
4. Se ejecuta `./hello.exe > output.txt` redireccionando la salida.
5. Se comprueba lo hecho en el paso 4 ejecutando `cat output.txt`.

## Fin
# Net2Fox
Librería NET que expone funciones útiles para consumir desde Visual FoxPro 9.0

## Requisitos
. [Net Framework 4 o Superior](https://www.microsoft.com/es-ES/download/details.aspx?id=17718)

## Instalación

1. Copiar `Net2Fox.dll` en la carpeta deseada.
2. Abrir la terminal de windows (cmd) con permisos de administrador y navegar hasta la carpeta donde está `Net2Fox.dll`
3. Ejecutar lo siguiente:

```Console
$> C:\Windows\Microsoft.NET\Framework\v2.0.50727\RegAsm.exe -tlb -codebase Net2Fox.dll
```

**NOTA: Si tienes una versión distinta entonces cambia `\v2.0.50727\` por la versión que tienes instalada.**

## Ejemplo de uso
```xBase
loNet2Fox = CreateObject("Net2Fox.Security")
? loNet2Fox.VERSION
? loNet2Fox.MD5("Net for Fox")
```

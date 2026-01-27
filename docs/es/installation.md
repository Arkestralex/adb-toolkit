# ADB Toolkit - Documentación inicial

## ¿Qué es ADB?
  ADB (Android Debug Bridge) es una herramienta de línea de comandos incluída en el Android SDK Platform Tools que permite comunicarte con un dispositivo Android desde una computadora. Se usa para depuración, transferencia de archivos, instalación de apps, control del sistema y más.

## Requisitos previos
  - Un dispositivo Android con:
    - Opciones de desarrollador habilitadas
    - Depuración USB activada
  - Un cable USB funcional (preferiblemente de datos)
  - Una PC con windows, Linux o macOS

## Activar opciones de desarrollador en Android
  1. Ve a Ajustes > Acerca del teléfono
  2. Pulsa 7 veces sobre el Número de compilación
  3. Vuelve a Ajustes y entra a Opciones de desarrollador
  4. Activa Depuración USB

## Instalación en GNU/Linux (Ubuntu/Debian y derivados)
  En Terminal:
  - sudo apt update
  - sudo apt install android-tools-adb android-tools-fastboot
  - verifica la instalación: adb version

## Instalación en Windows
  1. Descarga Platform Tools desde la página oficial de desarrolladores de Android
  2. Extrae el archivo ZIP en una carpeta (por ejemplo: C:\adb)
  3. Abre esa carpeta, mantén Shift+clic derecho y selecciona "Abrir Powershell aquí"
  4. Ejecuta: adb version

## Instalación en macOS
  - Usando Homebrew: brew install android-platform-tools

## Primer Uso
  - Conecta el dispositivo por USB y ejecuta:
    - adb devices
  En el teléfono aparecerá un mensaje solicitando autorización. Acepta la clave RSA.
  Si todo está correcto verás algo como:
    List of devices attached
    ABC1234567 device
  

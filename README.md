# LONKOTROLL TOOLKIT 🧌🔥💀😈🪄🎉📳💥🖕😂🤡💣

**MIT License** – trollea, rompe, vende, quema, todo vale 🔥🪦

[![License: MIT](https://img.shields.io/badge/License-MIT-red?style=for-the-badge&logo=ghost)](https://opensource.org/licenses/MIT)
![Troll Level](https://img.shields.io/badge/Troll%20Level-OVER%209000-orange?style=for-the-badge&logo=firefox)
![Windows Only](https://img.shields.io/badge/Windows-Only-black?style=for-the-badge&logo=windows)

Instalador que te obliga a sufrir mientras instalas Flutter con puro meme.

## ¿Estás lo suficientemente troleador?  
Ya casi... pero con esto llegas al OLIMPO DEL TROLLEO 😭🧌

## Instalación (como admin o te vas a arrepentir)
1. Crea `install_lonkotroll.bat`  
2. Copia el código de abajo  
3. Ejecutar como administrador  
4. Elige 9 para rickroll dreams (aunque no exista, el espíritu vive)  

```batch
@echo off
title LONKOTROLL TOOLKIT v666.9 - TROLLEO MÁXIMO ACTIVADO 😈🧌💀🔥🤡

echo =============================================
echo      LONKOTROLL TOOLKIT - EL REY DEL CAOS
echo   Flutter + Android Studio + TROLLEO PURO 2026
echo =============================================
echo.

choco -v >nul 2>&1 || (
    powershell -nop -ep bypass -c "iex ((new-object net.webclient).DownloadString('https://community.chocolatey.org/install.ps1'))"
)

choco install flutter androidstudio -y --force
setx PATH "%PATH%;C:\tools\flutter\bin" /M 2>nul

flutter doctor --android-licenses < NUL >nul 2>&1
flutter upgrade --force

echo.
echo =============================================
echo   ELIGE TU NIVEL DE TROLLEO (ENTER = MÁXIMO)
echo =============================================
echo.

:menu
cls
echo 1  flutter_riverpod      → state serio (aburrido) 🛡️
echo 2  dio                   → HTTP sin alma ⚡
echo 3  firebase suite        → backend que te trollea a ti 🔥
echo 4  hive                  → base de datos loca 🕳️
echo 5  lottie               → animaciones del infierno 🎬
echo 6  confetti             → confeti en tu vida 🎉💣
echo 7  animated_text_kit    → texto que te insulta 😏
echo 8  shake + vibration    → tiembla y vibra tu celu 📳😭
echo 9  rickroll dreams       → el sueño troll eterno 🎵🕺
echo 0  SALIR (cobarde) 🏳️
echo.

set /p picks="Nivel de trolleo: "

if "%picks%"=="" set "picks=1 2 3 4 5 6 7 8 9"

set "pkgs="

for %%n in (%picks%) do (
    if "%%n"=="1" set "pkgs=!pkgs! flutter_riverpod"
    if "%%n"=="2" set "pkgs=!pkgs! dio"
    if "%%n"=="3" set "pkgs=!pkgs! firebase_core firebase_auth cloud_firestore firebase_storage firebase_messaging"
    if "%%n"=="4" set "pkgs=!pkgs! hive hive_flutter"
    if "%%n"=="5" set "pkgs=!pkgs! lottie"
    if "%%n"=="6" set "pkgs=!pkgs! confetti"
    if "%%n"=="7" set "pkgs=!pkgs! animated_text_kit"
    if "%%n"=="8" set "pkgs=!pkgs! shake vibration"
    if "%%n"=="9" set "pkgs=!pkgs! just_audio"   REM para rickroll manual xd
    if "%%n"=="0" goto fin
)

if not "!pkgs!"=="" (
    echo.
    echo INSTALANDO TROLLEO MÁXIMO... AGUANTA CRACK 💀🔥
    flutter pub add !pkgs!
    echo.
    echo Listo. flutter pub get y prepárate pa'l ridículo 😂🧌
)

echo.
echo Presiona cualquier tecla pa' más trolleo...
pause >nul
goto menu

:fin
echo.
echo =============================================
echo        LONKOTROLL COMPLETADO - NIVEL DIOS
echo =============================================

echo.
echo          🧌
echo       💀   🔥
echo     😈       🪄
echo   🎉           💥
echo  🖕  TROLLEA SIEMPRE  🤡
echo.
timeout /t 5 >nul
exit

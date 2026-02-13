# LONKOTROLL TOOLKIT 🧌🔥💀😈🪄🎉📳💥🖕😂

**LONKOTROLL MODE FULL ACTIVADO FOREVER**  
Instalador caótico de Flutter + Android Studio + paquetes meme/troll para Windows  
Porque el desarrollo serio ya nos tiene hasta la coronilla 😤🪦

MIT License – haz lo que quieras, trollea sin culpa, vende el alma si te da la gana 🔥

## 🚀 ¿QUÉ HACE ESTE DEMONIO?  
- Instala Chocolatey si no existe ☠️  
- Baja Flutter SDK + Android Studio con choco en modo --force 😈  
- Acepta licencias Android sin preguntar ni joder ⚡  
- Menú interactivo para elegir paquetes serios o PURO CAOS TROLL 🧨  
- Paquetes que hacen explotar confeti, vibrar el celu, animaciones satánicas y más 💣🎊  

## 🛠 Requisitos (sin excusas)  
- Windows 10/11  
- **Ejecutar como administrador** (obligatorio o no funciona nada)  
- Internet (obvio weon) 🌐  

## 🔥 Instalación ultra-rápida  
1. Crea archivo `install_lonkotroll.bat`  
2. Copia y pega TODO el código de abajo  
3. Clic derecho → **Ejecutar como administrador**  
4. Dale ENTER para máximo caos o elige tus números de trolleo 🧌  


@echo off
title LONKOTROLL TOOLKIT v666 - NO MERCY MODE ACTIVADO 😈🧌💀🔥

echo =============================================
echo      LONKOTROLL TOOLKIT - EL CAOS ES LEY
echo   Flutter + Android Studio + PAQUETES TROLL 2026
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
echo   ELIGE TUS ARMAS TROLL (separados por espacio)
echo   ENTER = TODOS LOS PAQUETES CAÓTICOS + MEMES 💥🧨
echo =============================================
echo.

:menu
cls
echo 1  flutter_riverpod      → state a prueba de balazos 🛡️
echo 2  dio                   → HTTP sin piedad ni misericordia ⚡
echo 3  firebase suite        → backend que te quema el orto 🔥
echo 4  hive + hive_flutter   → base de datos loca y rápida 🕳️
echo 5  lottie               → animaciones satánicas nivel dios 🎬
echo 6  confetti             → explota confeti en cada build 🎉💣
echo 7  animated_text_kit    → texto que se burla de tu existencia 😏
echo 8  shake                → app vibra si la sacudes fuerte 📳😭
echo 9  rickroll             → rickroll random (sueño eterno) 🎵🕺
echo 0  SALIR / ME RINDO 🏳️
echo.

set /p picks="Lonkotroll manda: "

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
    if "%%n"=="8" set "pkgs=!pkgs! shake"
    if "%%n"=="9" set "pkgs=!pkgs! rickroll"
    if "%%n"=="0" goto fin
)

if not "!pkgs!"=="" (
    echo.
    echo LONKOTROLL INSTALANDO... PREPÁRATE PARA EL CAOS 💀🔥
    flutter pub add !pkgs!
    echo.
    echo Listo weon. Corre "flutter pub get" y sufre con estilo 😂🧌
)

echo.
echo Presiona cualquier tecla pa' seguir trolleando sin parar...
pause >nul
goto menu

:fin
echo.
echo =============================================
echo   LONKOTROLL TOOLKIT COMPLETADO 🧌💀🔥😈
echo   Que el espíritu troll te acompañe siempre 🪄🖕
echo =============================================
timeout /t 5 >nul
exit

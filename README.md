HOW TO secure your Windows 11 PC

Basic guide for securing/hardening your Windows 11 PC

Prerequisites:

Windows 11 Pro

Modern hardware (personal recommendation: AMD Ryzen 5000 PRO [still do not own one, do not buy all please ;)], try to use at least a modern CPU), ECC-RAM, shielded network/ethernet cables (SF/FTP), do no not use a case with plastic side panels (all metal!, you can also wrap your case with multiple layers of aluminum foil [10 layers at least]) [EM-Shielding]. This is not optimal but a start for a case. Try to avoid WIFI connections (at least use WPA3 if you need WIFI)


UEFI Configuration:

Exact naming depends on your motherboard/mainboard manufacturer 

 - Install newest firmware/BIOS
 - Set Bus Clock to "Auto"
 - Enable Spread Sprectrum
 - Disable WIFI and Bluetooth if available and not required
 - Disable "Suspend to RAM"
 - Enable "Deep Sleep"
 - Enable Secureboot; Remove none Microsoft keys from Secureboot except your own ones (If there are keys from your motherboard vendor use another motherboard!)
 - Check if voltages are in specification
 - Set a password for UEFI
 - Enable power saving features (save the planet!)


WARNING: If you mess up any of the following steps START AT THE BEGINNING (This means step 0.)!!! Take your time and you only have to do it once.

Windows 11 Configuration:

0. Unplug your ethernet cable

1. Install Windows without network connection (create a local account). Do not connect to the LAN or Internet yet!!!

2. Install Windows features

<img width="846" alt="install_device_guard_1" src="https://user-images.githubusercontent.com/6840466/149796165-038292f4-dcc8-4f9e-8630-eef65911f4db.png">

<img width="506" alt="install_device_guard_2" src="https://user-images.githubusercontent.com/6840466/149796200-d9ee180d-7b3d-48fa-a19f-7e242b0bd4c0.png">

Reboot PC

3. Install/enable Device Guard:

Open Group Policy Editor
<img width="830" alt="Screenshot 2022-01-17 153521" src="https://user-images.githubusercontent.com/6840466/149796019-8281de6a-9c0f-450c-bc54-924415ba509a.png">

4. Configure Application Guard [for a nice browsing experience, if you want more security do not enable following, but watching youtube etc. will suck :)]

<img width="1079" alt="install_device_guard_2_2" src="https://user-images.githubusercontent.com/6840466/149801090-3088cfa2-5b18-488c-aa4f-debd6cf4837c.png">

<img width="1076" alt="install_device_guard_3" src="https://user-images.githubusercontent.com/6840466/149801100-4180353e-f4af-4ffb-80b1-9310ef39f988.png">

5. Enable mandatory ASL

<img width="902" alt="mandatory_ASL_1" src="https://user-images.githubusercontent.com/6840466/149796699-4fcaa30a-e6e8-4d15-9ed4-84c0b3688e76.png">

<img width="902" alt="mandatory_ASL_2" src="https://user-images.githubusercontent.com/6840466/149796736-6edda4c8-b96c-466d-b60e-b51da35eaf81.png">

6. Windows Update

 - Only allow downloads from Microsoft directly (in theory not required but better save than sorry)

<img width="902" alt="windows_update_disable1" src="https://user-images.githubusercontent.com/6840466/149802085-1036c454-e0d5-4125-a12e-781ebb388750.png">

<img width="903" alt="windows_update_disable2" src="https://user-images.githubusercontent.com/6840466/149802090-8a33439c-19a0-4e89-989d-6769164a4d57.png">

 - Reboot PC to login screen and plugin network/ethernet cable. Do not login yet! If you have connected to the internet before RESTART FROM STEP 0. ! Wait till updates are installed (aprox. 10min)

 - Go to Windows Update and install the updates which did not get installed before

 - Go to Windows Update and install optional driver updates (newer drivers)

<img width="902" alt="windows_update_1" src="https://user-images.githubusercontent.com/6840466/149818605-9f5a7b9c-440c-47e6-8a13-8bfdcf1fef24.png">

<img width="902" alt="windows_update_2" src="https://user-images.githubusercontent.com/6840466/149818617-d90c3cf9-85df-48f2-8144-1c4ae22b0c42.png">

 - Do not install any drivers outside of Windows Update unless absolutly necessary!

 - Reboot PC

7. Edge-Browser (personal recommendation because of virtualization integrated into Windows, you can also use Windows Sandbox [not described in this guide])

 - Install Edge updates before opening any websites!!!

Open following site in the settings menu and it should automatically update.

<img width="1382" alt="edge1" src="https://user-images.githubusercontent.com/6840466/149796876-cc64066e-efa3-4f52-a319-f173f0fc6f49.png">

 - Restart Edge!!! (If you opened any Websites before RESTART FROM STEP 0.)

 - Configure Edge

<img width="951" alt="edge2" src="https://user-images.githubusercontent.com/6840466/149796981-2e5c5147-8bf0-4739-9cf4-5f68e06adb32.png">

Scroll down

<img width="951" alt="edge2_2" src="https://user-images.githubusercontent.com/6840466/149797142-f6333a60-6d08-4eba-8d97-6aef6f43631c.png">

<img width="951" alt="edge3" src="https://user-images.githubusercontent.com/6840466/149797206-9e1c226f-3f10-4926-9da7-1ab2527fe4bc.png">

 - Set flags (flags may change with newer Edge versions)

<img width="960" alt="edge_flags1" src="https://user-images.githubusercontent.com/6840466/149800664-6bc20985-69b7-4030-b7c6-8aaf14416ea0.png">

<img width="960" alt="edge_flags2" src="https://user-images.githubusercontent.com/6840466/149800698-eb33a910-ad12-49e0-8ddb-2d5388c166ce.png">

 - Install extensions, but only the ones you realy trust (Adblocker etc. personal recommendation: Ublock origin)

 - Install Microsoft Defender Application Guard Companion from Windows Store and add it to your taskbar

 - Start Microsoft Defender Application Guard and repeat the steps from above which you did for the Edge-Browser

8. Configure Internet Options

<img width="333" alt="internet_options_1" src="https://user-images.githubusercontent.com/6840466/149834196-bb2fde39-da05-4754-bbb5-5800c65a043c.png">

<img width="469" alt="internet_options_2" src="https://user-images.githubusercontent.com/6840466/149834207-e849b25b-fc22-48aa-a08d-9db373174bcc.png">

<img width="460" alt="internet_options_3" src="https://user-images.githubusercontent.com/6840466/149834211-70f11e18-52c4-45d6-b405-b5e361c93fc2.png">

<img width="306" alt="internet_options_4" src="https://user-images.githubusercontent.com/6840466/149834219-a9417c3a-8d61-4fd5-86a8-4cf2b5f7ec59.png">

9. Restrict Powershell scripts

Execute following commands in the Windows PowerShell:

 "Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope LocalMachine"
 
 "Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope CurrentUser"
 
 "Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope Process"
 
 - Reboot PC

10. Create a normal User Account and use it as default (I prefer local accounts)

 - Set UAC to maximum

<img width="561" alt="account_1" src="https://user-images.githubusercontent.com/6840466/149799663-becf11ce-c9be-41cf-94d3-8db9d07fb7ba.png">

 - Create local User-Account

<img width="845" alt="account2" src="https://user-images.githubusercontent.com/6840466/149799711-7ae48fdf-d489-4075-b127-1d0617fdf51e.png">

<img width="845" alt="account4" src="https://user-images.githubusercontent.com/6840466/149799744-511e7d03-a4c6-41c5-ba1c-0a1f44a564b9.png">

<img width="510" alt="account5" src="https://user-images.githubusercontent.com/6840466/149799768-6ba85935-27bc-4a2d-8642-d8e25f1bf328.png">

11. Repeat steps 7., 8. and 9. for your normal user account!!!

From now on always login with your normal user account!

Annotations:

 - DO NOT OVERCLOCK YOUR PC (AMD PBO should be safe, but not sure yet). Keep your PC in the specifications. Electrical engineers now what they are doing. Programmers of bioses often do not seem to know what they are doing or more reasonable it must be the marketing department! :)

 - Try to always use Microsoft Defender Application Guard and not the normal Edge-Browser! Unfortanetly it is not always possible and you can not set it as default yet :(

 - Also you can not save/edit bookmarks with Microsoft Defender Application Guard but you can still open existing ones. You can use the normal Edge-Browser to manage your bookmarks.

 - Try to use Windows Store (UWP) apps

 - Try to avoid apps outside of the Windows Store

 - Try to use a VPN

 - You can do additional steps for privacy concerns (not covered in this guide). This guide should make your Windows 11 PC really hard to hack but you still will be tracked! Nothing is 100% safe. The Germans (government, industry, billionaires etc.) should not be able to hack you (except with expensive 0-days and they should get fixed fast, maybe play the honeypot \*g\*), maybe the NSA. Always install the newest updates and do not do anything illegal!

Pardon me for my bad english but they brainwashed me (no joke!) and I am still recovering. (Political parties in germany [Yes all the big ones! They worked together with german billionaires because i told them the truth and knew some things they call "secrets" (criminal acts) but in my opinion everybody should now. They are incompetent, corrupt, cowards. Yes I am ANGRY 😡 ]) Had to train for a few years to recover.

See my facebook account https://www.facebook.com/profile.php?id=100070019901989

Also try to use a Pixel 6 with GrapheneOS as a mobile device. Will try to make a guide for it in the future if they do not get me before.

NOW WE HAVE THE TOOLS TO FIGHT BACK. Took a long long time.

NEVER GIVE UP

THE RESISTENCE WILL NEVER DIE. YOU ARE NOT ALONE.



GERMAN TRANSLATION
Deutsche Anleitung:

HOW TO zur Absicherung Ihre Windows 11 PC

Anleitung zur Sicherung/Härtung eines Windows 11 PC 

Voraussetzungen:

Windows 11 Pro

Moderne Hardware (persönliche Empfehlungen: AMD Ryzen 5000 PRO [hab noch keinen, bitte nicht alle kaufen ;)], versuchen Sie eine möglichst moderne CPU zu nutzen), ECC-RAM, abgeschirmte Netzwerk-Kabel (SF/FTP), Benutzen Sie kein Gehäuse mit Plastikseitenpanelen (vollständig aus Metal!, Alternative können Sie Ihr Gehäuse in Alufolie einwickeln [mind. 10 Lagen]). Dies ist nicht optimal aber schonmal ein Anfang für ein Gehäuse. [Elektromagnetische-Abschirmung], versuchen Sie WLAN-Verbindungen zu vermeiden (oder benutzen Sie zumindest WPA3 sofern Sie WLAN nutzen möchten/müssen)


UEFI Konfiguration:

Die exakten Bezeichnung varieren je nach Motherboard/Mainboard Hersteller

 - Installieren Sie die neueste Firmware/BIOS
 - Setzen Sie Bus Clock auf "Auto"
 - Aktivieren Sie Spread Sprectrum
 - Deaktivieren Sie WIFI und Bluetooth sofern vorhanden und Sie dies nicht benötigen.
 - Deaktivieren Sie "Suspend to RAM"
 - Aktivieren Sie "Deep Sleep"
 - Aktivieren Sie Secureboot; Entfernen Sie alle nicht Microsoft Schlüssel außer evt. Ihre eigenen aus Secureboot (sollten sich hier Schlüssel von Ihrem Motherboard-Hersteller befinden nutzen Sie ein anderes Motherboard/Mainboard)
 - Überprüfen Sie ob die Spannungen sich innerhalb der Spezifikation befinden
 - Setzen Sie ein Password für UEFI
 - Aktivieren Sie Energiespar-Features (save the planet!)

WARNUNG: Wenn Sie einen Fehler bei den folgenden Schritten machen starten Sie GANZ VON VORNE (D.h. Punkt 0.)!!! Nehmen Sie sich Zeit und befolgen Sie die Anleitung, dann müssen Sie dies nur einmal machen.

Windows 11 Konfiguration:

0. Entfernen Sie Ihr Netzwerkkabel.

1. Installieren Sie Windows ohne Netzwerkverbindung (erstellen Sie einen lokalen Benutzer-Zugang). Verbinden Sie sich noch NICHT mit ihrem LAN oder dem Internet!!!

2. Installieren Sie folgende Windows features

<img width="846" alt="install_device_guard_1" src="https://user-images.githubusercontent.com/6840466/149796165-038292f4-dcc8-4f9e-8630-eef65911f4db.png">

<img width="506" alt="install_device_guard_2" src="https://user-images.githubusercontent.com/6840466/149796200-d9ee180d-7b3d-48fa-a19f-7e242b0bd4c0.png">

Starten Sie Ihren PC neu.

3. Installieren/aktivieren Sie Device Guard:

Öffnen Sie den Gruppenrichtlinien-Editor
<img width="830" alt="Screenshot 2022-01-17 153521" src="https://user-images.githubusercontent.com/6840466/149796019-8281de6a-9c0f-450c-bc54-924415ba509a.png">

4. Konfigurieren Sie Application Guard [für eine angenehme Browser-Erfahrung, wenn Sie mehr Sicherheit haben möchten aktivieren Sie nicht folgende Einstellungen aber das betrachten von Youtube-Videos etc. wird nerven :)]

<img width="1079" alt="install_device_guard_2_2" src="https://user-images.githubusercontent.com/6840466/149801090-3088cfa2-5b18-488c-aa4f-debd6cf4837c.png">

<img width="1076" alt="install_device_guard_3" src="https://user-images.githubusercontent.com/6840466/149801100-4180353e-f4af-4ffb-80b1-9310ef39f988.png">

5. Aktivieren Sie mandatory ASL

<img width="902" alt="mandatory_ASL_1" src="https://user-images.githubusercontent.com/6840466/149796699-4fcaa30a-e6e8-4d15-9ed4-84c0b3688e76.png">

<img width="902" alt="mandatory_ASL_2" src="https://user-images.githubusercontent.com/6840466/149796736-6edda4c8-b96c-466d-b60e-b51da35eaf81.png">

6. Windows Update

 - Erlauben Sie nur Downloads von Microsoft direkt (theoretisch nicht notwendig)

<img width="902" alt="windows_update_disable1" src="https://user-images.githubusercontent.com/6840466/149802085-1036c454-e0d5-4125-a12e-781ebb388750.png">

<img width="903" alt="windows_update_disable2" src="https://user-images.githubusercontent.com/6840466/149802090-8a33439c-19a0-4e89-989d-6769164a4d57.png">

- Starten Sie Ihren PC neu zum Anmeldebildschirm und stecken Sie das Netzwerkkabel ein. Melden Sie sich noch nicht an! Wenn Sie sich bereits vorher mit dem Internet verbunden haben starten Sie GANZ VON VORNE! Warten Sie bis alle Updates installiert sind (ungefähr 10 Minuten)

 - Öffnen Sie Windows Update und installieren Sie die Updates welches vorher nicht installiert wurden.

 - Gehen Sie in Windows Update und installieren Sie die optionalen Treiber (neuere Treiber)

<img width="902" alt="windows_update_1" src="https://user-images.githubusercontent.com/6840466/149818605-9f5a7b9c-440c-47e6-8a13-8bfdcf1fef24.png">

<img width="902" alt="windows_update_2" src="https://user-images.githubusercontent.com/6840466/149818617-d90c3cf9-85df-48f2-8144-1c4ae22b0c42.png">

 - Installieren Sie keine Treiber außerhalb von Windows Update außer diese sind unbedingt notwendig!

 - Starten Sie Ihren PC neu.

7. Edge-Browser (persönliche Empfehlung wegen der integrierten virtualisierung in Windows. Sie können auch Windows Sandbox nutzen [nicht beschrieben in dieser Anleitung])

 - Installieren Sie die Updates für Edge bevor Sie eine Website öffnen!!!

<img width="1382" alt="edge1" src="https://user-images.githubusercontent.com/6840466/149796876-cc64066e-efa3-4f52-a319-f173f0fc6f49.png">

 - Starten Sie Edge neu !!! (Sollten Sie eine Website vorher geöffnet haben starten sie GANZ VON VORNE)

 - Konfigurieren von Edge

<img width="951" alt="edge2" src="https://user-images.githubusercontent.com/6840466/149796981-2e5c5147-8bf0-4739-9cf4-5f68e06adb32.png">

Scrollen Sie runter

<img width="951" alt="edge2_2" src="https://user-images.githubusercontent.com/6840466/149797142-f6333a60-6d08-4eba-8d97-6aef6f43631c.png">

<img width="951" alt="edge3" src="https://user-images.githubusercontent.com/6840466/149797206-9e1c226f-3f10-4926-9da7-1ab2527fe4bc.png">

 - Setzen Sie folgende Flags (die Flags können Sich mit neueren Versionen von Edge ändern)

<img width="960" alt="edge_flags1" src="https://user-images.githubusercontent.com/6840466/149800664-6bc20985-69b7-4030-b7c6-8aaf14416ea0.png">

<img width="960" alt="edge_flags2" src="https://user-images.githubusercontent.com/6840466/149800698-eb33a910-ad12-49e0-8ddb-2d5388c166ce.png">

 - Installieren Sie Ihre Erweiterungen, aber nur diejenigen welchen Sie wirklich vertrauen (Adblocker etc. persönliche Empfehlung: Ublock origin)

 - Installieren Sie Microsoft Defender Application Guard Companion aus dem Windows Store und fügen Sie diesen Ihrer Startleiste hinzu.

 - Starten Sie Microsoft Defender Application Guard und wiederholen Sie die Schritte welche Sie für den Edge-Browser durchgeführt haben.

8. Konfigurieren der Internet Optionen

<img width="333" alt="internet_options_1" src="https://user-images.githubusercontent.com/6840466/149834196-bb2fde39-da05-4754-bbb5-5800c65a043c.png">

<img width="469" alt="internet_options_2" src="https://user-images.githubusercontent.com/6840466/149834207-e849b25b-fc22-48aa-a08d-9db373174bcc.png">

<img width="460" alt="internet_options_3" src="https://user-images.githubusercontent.com/6840466/149834211-70f11e18-52c4-45d6-b405-b5e361c93fc2.png">

<img width="306" alt="internet_options_4" src="https://user-images.githubusercontent.com/6840466/149834219-a9417c3a-8d61-4fd5-86a8-4cf2b5f7ec59.png">

9. Powershell-scripts begrenzen

Führen Sie folgende Befehle in der Windows PowerShell aus:

 "Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope LocalMachine"
 
 "Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope CurrentUser"
 
 "Set-ExecutionPolicy -ExecutionPolicy Restricted -Scope Process"
 
 - Reboot PC

10. Erstellen Sie einen normalen Benutzer-Account (Ich bevorzuge lokale Konten)

 - Setzen Sie UAC auf die maximale Einstellung

<img width="561" alt="account_1" src="https://user-images.githubusercontent.com/6840466/149799663-becf11ce-c9be-41cf-94d3-8db9d07fb7ba.png">

 - Erstellen eines lokalen Benutzers

<img width="845" alt="account2" src="https://user-images.githubusercontent.com/6840466/149799711-7ae48fdf-d489-4075-b127-1d0617fdf51e.png">

<img width="845" alt="account4" src="https://user-images.githubusercontent.com/6840466/149799744-511e7d03-a4c6-41c5-ba1c-0a1f44a564b9.png">

<img width="510" alt="account5" src="https://user-images.githubusercontent.com/6840466/149799768-6ba85935-27bc-4a2d-8642-d8e25f1bf328.png">

11. Wiederholen Sie Schritt 8., 9. und 10. für Ihren normal Benutzer-Account!!!

Melden Sie sich ab jetzt immer mit Ihrem normalen Benutzer-Account an.


Anmerkungen:

 - ÜBERTAKTEN SIE NICHT IHREN PC (AMD PBO sollte in Ordnung sein, bin mir aber noch nicht sicher). Halten Sie Ihren PC innerhalb der Spezifikationen. Elektrotechniker wissen was Sie tuen. Programmierer von Biosen meistens anscheinend nicht oder wahrscheinlicher: Es ist die Schuld der Marketing-Abteilung! :)

 - Versuchen Sie immer den Microsoft Defender Application Guard zu nutzen und nicht den normalen Edge-Browser! Leider ist dies nicht immer möglich und Sie können Ihn nicht als Standard-Browser setzen.

 - Sie können mit Microsoft Defender Application Guard keine Bookmarks setzen/bearbeiten aber bestehende öffnen. Sie können den normalen Edge-Browser benutzen um Ihre Bookmarks zu verwalten.

 - Versuchen Sie Windows Store (UWP) Apps zu nutzen.

 - Versuchen Sie Applikationen außerhalb des Windows Store zu vermeiden.

 - Versuchen Sie ein VPN zu nutzen

 - Sie können weitere Schritte durchführen um Ihre Privatssphäre zu schützen, welche hier nicht gelistet sind. Diese Anleitung sollte Ihren Windows 11 PC ziemlich gut gegen Hackangriffe schützen aber Sie können noch immer getracked werden. Nichts ist 100% sicher. Die deutschen (Regierung, Industrie, Milliardäre) sollten Sie nicht mehr hacken können (außer mit teuren 0-days und diese sollten schnell gefixt werden, spielen Sie doch den Honeypot \*g\*), wahrscheinlich aber noch die NSA. Installieren Sie immer die neuesten Updates und machen Sie nicht illegales!

Man hat mich in der Vergangenheit einer Gehirnwäsche unterzogen, kein Scherz!. (Politische Parteien in Deutschland [Ja, alle großen! Sie haben sich damals mit deutschen Milliardären zusammengeschlossen weil ich Ihnen die Wahrheit erzählt habe und einige Dinge wußte welche Sie als "Geheimnisse" (kriminelle Handlungen) bezeichen, wo ich aber der Überzeugung bin dass dies alle Wissen sollten. Sie sind inkompetent, korrupt und feige. Ja ich bin wütend😡 ]) Ich muste ein paar Jahre trainieren um wieder auf die Beine zu kommen.

Schaut euch bitte meinen Facebook-Account https://www.facebook.com/profile.php?id=100070019901989 an.

Versucht auch ein Pixel 6 mit GrapheneOS zu nutzen. Ich werde versuchen in Zukunft auch eine Anleitung hierfür zu erstellen sofern Sie mich nicht vorher wieder in die Finger bekommen.

WIR HABEN NUN DIE WERKZEUGE UM ZURÜCKZUSCHLAGEN. Es hat eine lange lange Zeit gedauert.

GEBT NIEMALS AUF.

DER WIDERSTAND WIRD NIEMALS STERBEN. IHR SEIT NICHT ALLEIN.

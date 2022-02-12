# $Dedsec
 @echo off
 color 0a
 title $Skizm Prompt$
 echo $dedsec$ [Version v.1]
 echo (c) SKIZM. All rights reserved.
:typecmd
set c=
set /P c="$dedsec>"

if /I "%c%" EQU "$wait" (
 color 0a
 timeout 5
 goto typecmd
)

if /I "%c%" EQU "$checkup" (
 start https://discord.gg/dkQBKTDT
 goto typecmd
)

if /I "%c%" EQU "$clear" (
 cls
 goto typecmd
)

if /I "%c%" EQU "$KeyFlood" (
 :start
 color 0a
 :start
 echo %random% %random% %random% %random% %random% %random% %random% %random% %random% %random%.
 goto start
 goto typecmd
)

if /I "%c%" EQU "$CheckFiles" (
 tree
 goto typecmd
)

if /I "%c%" EQU "$DDoS" (
 echo Click on the "Add" button and then type in the persons IP address, then fill out the rest of the stuff.
 shutdown -i
 goto typecmd
)

if /I "%c%" EQU "$ping" (
 ping google.com
 goto typecmd
)

if /I "%c%" EQU "$ping2" (
 ping discord.com
 goto typecmd
)

if /I "%c%" EQU "$EncStatus" (
 Cipher
 goto typecmd
)

if /I "%c%" EQU "$dir" (
 Dir
 goto typecmd
)



if /I "%c%" EQU "" (
 goto typecmd
) ELSE (
 echo Unknown command "%c%"!
 goto typecmd
)

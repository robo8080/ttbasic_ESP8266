TOYOSHIKI Tiny BASIC for Arduino(ESP8266/ESP-WROOM-02)

オリジナルのArduino版からの変更点<br>
1.ESP8266/ESP-WROOM-02だとSoft WDTに引っかかってしまう問題を対策<br>
2.LOAD/SAVEコマンドを追加（LOAD/SAVEできるプログラムは１つのみ）

The code tested in ESP-WROOM-02.<br>
Use UART terminal, or temporarily use Arduino IDE serial monitor.

Operation example

&gt; list<br>
10 FOR I=2 TO -2 STEP -1; GOSUB 100; NEXT I<br>
20 STOP<br>
100 REM Subroutine<br>
110 PRINT ABS(I); RETURN

OK<br>
&gt;run<br>
2<br>
1<br>
0<br>
1<br>
2

OK<br>
&gt;

The grammar is the same as<br>
PALO ALTO TinyBASIC by Li-Chen Wang<br>
Except 3 point to show below.

(1)The contracted form of the description is invalid.

(2)Force abort key<br>
PALO ALTO TinyBASIC -> [Ctrl]+[C]<br>
TOYOSHIKI TinyBASIC -> [ESC]<br>
NOTE: Probably, there is no input means in serial monitor.

(3)Other some beyond my expectations.

(C)2012 Tetsuya Suzuki<br>
GNU General Public License

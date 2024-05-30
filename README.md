Aufgabe 1.4 simpleBlink (40%)
Wir wollen in den weiteren Übungen für das EduArdu-Board eine Art Roboter, den DiBS▪E, implementieren. In dieser Aufgabe wollen wir die Grundlage dafür schaffen.
Erstellen Sie die Dateien dibse.h und dibse.cpp und implementieren Sie dort die Klasse DibsE. Aktuell sollen darin die folgenden Methoden umgesetzt werden:
	• void setup(): wird in der setup-Funktion eines Arduino Programms aufgerufen. Diese Funktion macht derzeit noch nichts ;-)
	• void loop(): wird in der loop-Funktion eines Arduino Programms aufgerufen.
	• void simpleBlinkOn(int duration, int red, int green, int blue): Diese Funktion soll das RGB-LED von DiBS▪E abwechselnd für die Dauer von int duration leuchten lassen bzw. ausschalten. Die Farbe wird dabei durch einen RGB-Wert (int red, int green & int blue) bestimmt.
	• void simpleBlinkOff(): stoppt das Blinken.
Implementierung
Das eigentliche Blinken, soll in der Funktion DibsE::loop() stattfinden. In den Funktionen DibsE::simpleBlinkOn(...) und DibsE::simpleBlinkOff() werden nur entsprechende Objektvariablen gesetzt, welche dann von DibsE::loop() verwendet werden, um das eigentliche "Blinken" umzusetzen.
Hauptprogramm
Implementieren Sie ein Programm (in der Datei main.cpp), das die Verwendung Ihrer Klasse demonstriert:
	• Erzeugen Sie eine Instanz der Klasse DibsE dibse ausserhalb von setup und loop.
	• Innerhalb von setup wird dibse.setup() aufgerufen.
	• Danach wird dibse.simpleBlinkOn(...) ausgeführt.
	• Innerhalb von loop wird dibse.loop() aufgerufen.

![image](https://github.com/claner2804/Embedded-Systems-hw01-04/assets/131294860/717c7beb-7e7e-4e9a-8586-034aa6d8f4e3)

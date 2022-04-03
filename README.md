# Ender-2-Pro-BLTouch-und-Autoleveling
Marlin V2.0.X mit BL Touch und Autoleveling

Montage des BL Touch wie vom Hersteller empfohlen.
BL Touch an das Motherboard Creality V 4.2.3 anschließen.
Dabei den original Z- Stopp entfernen und durch BL Touch Anschluss ersetzen ( siehe Foto ) 

- MB ------ BL Touch
- G ------- GND   (grün)
- V ------- +5 V  (rot)
- IN ------ Servo (gelb)

- Z- ------ GND   (schwarz)
- Z- ------ OUT   (weiß)


![BL Toch](https://user-images.githubusercontent.com/7778580/161447623-86126328-9e7d-4d9e-9ef0-4941bb0801f5.jpg)

Danach: 
- die .bin auf eine SD Karte kopiere
- Drucker ausschalten
- SD Karte einführen
- Drucker einschalten
- Firmware installiert sich selbtsändig

Z-Offset einstellen(!!!!) 

Erst wenn das Z-Offset richtig eingestellt ist, weiter machen!!

Empfohlen wird, jetzt das Bett mit Konsolen Befehlen zu nivellieren und die Daten im Eprom zu speichern. 
- G28   für Home Position
- G29   für leveling
- M500  um die Messdaten im Eprom zu speichern

Im Slicer den Startcode mit 
- M501    // lädt die gespeicherten Daten
- M420 S1 // schaltet das Leveling ein

... ergänzen


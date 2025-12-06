# ICM20948 9-Achsen Bewegungssensormodul

## Beschreibung
Ein GSM/GPRS-Modul ist ein Mobilfunk-Modem für [2G-Netz](https://www.pcwelt.de/article/2251322/wann-2g-abschaltung-folgen.html), um SMS, Telefonie und mobile Daten zu nutzen.
GSM = Global System for Mobile Communications
klassischer 2G-Mobilfunkstandard
GPRS = General Packet Radio Service
Erweiterung von GSM zur mobilen Datenübertragung via Internet
Die Steuerung läuft über AT-Befehle (serial/UART)

Merkmale:
Der serielle Port ist ein TTL-Port, der direkt mit einem Mikrocontroller verbunden werden kann.
Automatischer Start beim Einschalten des Moduls, automatische Netzwerksuche
On-Board-Anzeige für alle Signale (Signal langsam blinken, kein Signal schnell blinken)
Mini-GSM/GPRS-Breakout-Board basiert auf SIM-Modul, unterstützt Quad-Band-GSM/GPRS-Netzwerk, verfügbar für GPRS und SMS-Datenfernübertragung.
Das Board zeichnet sich durch kompakte Größe und niedrigen Stromverbrauch aus. Dank der Energiespartechnik liegt der Stromverbrauch im Sleep-Modus bei nur 1 mA.
Es kommuniziert mit dem Mikrocontroller über den UART-Port und unterstützt Befehle wie 3GPP TS 27.007, 27.005 und SIMCOM enhanced AT Commands.
Betriebsspannung: 3,5~4,2V
Quad-Band 850/900/1800/1900MHz
Anschluss an jedes globale GSM-Netz mit jeder 2G-SIM
Tätigen und empfangen Sie Sprachanrufe über ein Headset oder einen externen Lautsprecher und ein Elektretmikrofon.
Senden und Empfangen von SMS-Nachrichten.
Senden und Empfangen von GPRS-Daten (TCP/IP, HTTP, usw.).
Scannen und Empfangen von FM-Radioübertragungen.
Anschluss zur Steuerung von Summer und Vibrationsmotor.
AT-Befehlsschnittstelle mit "Auto-Baud"-Erkennung.

## Technische Daten

Die Stromversorgung des SIM800L ist anscheinend nicht ganz unkritisch,
daher wird empfohlen parallel zur Stromversorgung einen 2.2 mF Kondensator (z.B.: [Amazon Produktseite]([https://www.amazon.de/dp/B0CM9HGCKX](https://www.amazon.de/dp/B01MUEBGT8))) zum Puffern von Stromspitzen,
welche anscheinend bis zu 2 A betragen können, einzubauen

## Bezugsquelle
[Amazon Produktseite](https://www.amazon.de/dp/B0CM9HGCKX)

## Foto
<img src="[https://wolles-elektronikkiste.de/wp-content/uploads/2021/07/ICM20948_module_small.jpg](https://wolles-elektronikkiste.de/wp-content/uploads/2021/11/SIM800L_pinout-1536x883.png)" width="200">
<img src="[[https://wolles-elektronikkiste.de/wp-content/uploads/2021/07/ICM20948_module_small.jpg](https://wolles-elektronikkiste.de/wp-content/uploads/2021/11/SIM800L_pinout-1536x883.png](https://wolles-elektronikkiste.de/wp-content/uploads/2021/10/SIM800L_Sim_Karte-741x1024.jpg)" width="200">


## Weiterführende Quellen
[SIM800L Modul](https://wolles-elektronikkiste.de/sim800l-modul)
[Raspberry Pi Pico With SIM800L Module](https://www.theelectronics.co.in/2021/09/raspberry-pi-pico-with-sim800l-module.html)
[Send Receive SMS & Call with SIM800L GSM Module & Arduino][(https://www.circuits-diy.com/send-receive-sms-call-with-sim800l-gsm-module-arduino/)
[Raspberry Pi Pico Relay Control With SMS Sim800L Arduino IDE](https://www.youtube.com/watch?v=8HVxT5M7FmI)
[Liste mit AT-Befehlen](https://github.com/anothermist/LIBRARIES/blob/master/TinyGSM/extras/AT%20Command%20Manuals/SIM800%20Series%20AT%20Command%20Manual%20V1.10.pdf)


###Trouble shooting:
[Probleme mit dem einwählen in ein Mobilfunknetz mittel SIM 800L Modem](https://www.mikrocontroller.net/topic/430187)
[Spannungsversorgung des SIM800L Mobilfunkmoduls](https://cbrell.de/blog/spannungsversorgung-des-sim800l-mobilfunkmoduls/)
[Solutions of SIM800L Network Problem | 4 Methods](https://www.youtube.com/watch?v=j2mM4ssH8nk (siehe Videobeschreibung))
[SIM800L SIM Karte Provider](https://forum.arduino.cc/t/sim800l-sim-karte-provider/508736)
[MicroPython libraries for the SIM800 module](https://community.hiveeyes.org/t/micropython-libraries-for-the-sim800-module/1492)



## Fritzing Part
missing

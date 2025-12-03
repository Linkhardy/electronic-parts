# RTC Real Time Clock DS3231

## Beschreibung
Das AZDelivery RTC-Modul mit DS3231 Chipsatz zeichnet sich nicht nur durch seinen hochpräzisen Uhrenquarz aus,
es findet auch jede Minute eine Messung der Temperatur statt, um den Oszillator zu Korrekturzwecken anzupassen.
Dank mitgelieferter Knopfzelle und integrierten EEPROM bleibt die Uhrzeit auch bei einem Ausfall der Spannung erhalten.
Die Verkabelung ist durch den verwendeten I2C-Bus sehr einfach und die IIC-Adresse kann selbstverständlich geändert werden.
Ein zusätzlicher Ausgang für das 32kHz-Signal ist ebenfalls vorhanden und kann über ein Register aktiviert werden.
Die RTC ist abwärtskompatibel und kann auch mit der Library für die DS1302 verwendet werden.
Die Real-Time-Uhr bietet programmierbare Tageszeitalarme und ein Kalender, das auf einen Rechteckwellenausgang eingestellt werden kann.
Adresse und Daten werden seriell über einen bidirektionalen I2C-Bus übertragen.

## Technische Daten
Abmessungen	34mm x 23mm x 18mm	43 mm x 23 mm x 20 mm
Speicherchip	AT24C32
Uhrenchip	DS3231 RTC
Digitaler Temperatursensor	±3°C Genauigkeit
Speicherkapazität	32 kB
Tageszeitalarm	2
Schnittstelle	I2C
Betriebstemperatur	0 to +70 ℃ ℃
Stromverbrauch	weniger als 1mA
Versorgungsspannung	3,3V
Knopfzelle	CR2032

## Bezugsquelle
[Amazon Produktseite](https://www.amazon.de/dp/B076GP5B94)


## Foto
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.giganepal.com%2Fwp-content%2Fuploads%2F2023%2F04%2F71eUOEnI04L._AC_SX679_.jpg&f=1&nofb=1&ipt=b34ed51cd8782542d0817f332fa500ac944ffcb3f64feb54f9a8c8a7411cce7e"  width="400">


## 24C32 EEPROM
A 32-byte Atmel 24C32 EEPROM chip with unlimited read-write cycles is also included with the DS3231 RTC module.
The three A0, A1, and A2 solder jumpers on the back make modifying the EEPROM’s I2C address simple. The addresses are hardcoded into each of these. Soldering a jumper short establishes the address.
[Electronic Smith](https://electronicsmith.com/interfacing-ds3231-real-time-clock-rtc-module-with-arduino/)
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse4.mm.bing.net%2Fth%2Fid%2FOIP.QpaxdA75WG7N5Xt_m9OFLAHaDt%3Fpid%3DApi&f=1&ipt=b922d6d5529dce14e34243436f440d88874ead1a960012b3c4907774c0053549&ipo=images" width="400">


## Battery
1. if you power the module with 3.3V or 5V (both is OK) and use a CR2032 battery you HAVE to desolder the resistor "201".
The battery will not be charged but will work fine as a backup battery when there is no Vcc
2. if you power the module with 3.3V or 5V (both is OK) and use a LIR2032 battery, you DONT have to desolder anything, but you'll have limited battery life
Advisable is option 1.
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Feurope1.discourse-cdn.com%2Farduino%2Foptimized%2F4X%2Fa%2F0%2F7%2Fa07d64c6d6c3713b93bd2923ef705428735398e8_2_790x750.jpeg&f=1&nofb=1&ipt=a92e0de5ff00d0f00ca348592ddac6e4056a023e4891f54b50366d641393f20f" width="400">
[Arduino Forum](https://forum.arduino.cc/t/zs-042-ds3231-rtc-module/268862/69?page=4)


## Datenblatt
[AZ-Delivery](https://cdn.shopify.com/s/files/1/1509/1638/files/DS3231_RTC_Real_Time_Clock_DE_2a4d775e-b341-4982-a91d-0b543af02304.pdf?v=1756708072)

## Anwendungsbeispiel
[Anwendungsbeispiel](https://electrocredible.com/ds3231-raspberry-pi-pico-micropython-arduino/)

## Fritzing Part
[Fritzing Part](https://github.com/Michaeltetteh/Fritzing_parts/blob/master/ZS-042%20RTC%20Module.fzpz)

# MAX30102 Heart Rate Sensor Module Pulse Detection Blood Oxygen Concentration Module

## Beschreibung
Der MAX30102 beinhaltet:
2x LEDs, eine rote (660 nm) und eine infrarote (880 nm)
2x Fotodioden zur Messung des reflektierten Lichts
18-Bit-ADC-Wandler mit einer Abtastrate von 50 bis 3200 Abtastungen pro Sekunde.
Darüber hinaus verfügt es über die notwendige Elektronik zur Signalverstärkung und -filterung, Unterdrückung von Umgebungslicht, Unterdrückung von Frequenzen von 50–60 Hz (künstliches Licht) und Temperaturkompensation.
Modulverbrauch kann bis zu 50mA erreichen während der Messung, obwohl die Intensität programmgesteuert angepasst werden kann, mit einem Energiesparmodus von 0.7 µA während der Messungen.

## Technische Daten
### Specification:

LED Peak Wavelength: 660nm/880nm

LED Power Supply Voltage: 3.3 - 5V

Detection Signal Type: Optical Reflection Signal (PPG)

Output Signal Interface: I2C Interface

Communication Interface Voltage: 1.8 - 3.3V- 5V

Reserve Mounting Hole Size:0.5x8.5mm / 0.02x0.33Inches

### Interface:

VIN: Main Power Input 1.8V-5V

3-Bit Pad: I2C Bus Pull Up Level, You Can Choose 1.8V or 3.3V According to the Pin Master Voltage

SCL: I2C Bus Clock

SDA: Connected to the I2C Bus Data

INT: MAX30102 Chip Interrupt PIN

RD: MAX30102 Chip's RD LED Grounding Terminal, Generally Doesn't Need to Connect

IRD: MAX30102 Chip's IR LED Grounding Terminal, Generally Doesn't Need to Connect

GND: Grounding Wire

## Bezugsquelle
[Amazon Produktseite](https://amzn.eu/d/gLniU65)

## Foto
![MAX30102](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%2Fid%2FOIP.PlETOxlu_RatY1Pl-bIIiQAAAA%3Fcb%3Diwc2%26pid%3DApi&f=1&ipt=fd81998983b020f03006f384077353917e1b73766950e31fa034ff1653acb6f0&ipo=images)

## Funktionsdiagramm
![MAX30102](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdfimg.dfrobot.com%2Fnobody%2Fwiki%2F7cf018f2483b44524299a436674798d5.png&f=1&nofb=1&ipt=fd40b72682752eec6201a3e76e3a830ceb53dbe41fcd6151c8b9cd9d7f731ce9)

## Datenblatt
[MAX30102](https://www.analog.com/media/en/technical-documentation/data-sheets/max30102.pdf)

## Anwendungsbeispiel
[Anwendungsbeispiel](https://docs.sunfounder.com/projects/umsk/en/latest/04_pi_pico/pico_lesson14_max30102.html)

[Video](https://www.youtube.com/watch?v=98Szuwh-6l8)

[Anwendungsbeispiel](https://github.com/n-elia/MAX30102-MicroPython-driver#other-things-that-its-worth-mentioning)

## Fritzing Part
[Fritzing Part](https://forum.fritzing.org/uploads/short-url/54LyjpeYKuzNVKssq4irRU79VqA.fzpz)


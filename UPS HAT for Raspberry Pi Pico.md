# Uninterruptible Power Supply (UPS) HAT for Raspberry Pi Pico

## Beschreibung
Charger Power Bank Power Management Expansion Board for Raspberry Pi Pico/Pico W UPS Power Supply Uninterruptible UPS HAT,Support 18650 Lithium Battery

Merkmale:
Raspberry Pi Pico UPS-Modul

Dies ist ein tragbares Netzteil für den Raspberry Pi Pico.

Es unterstützt die Verwendung einer einzelnen 18650-Lithiumbatterie für die Stromversorgung, die Ihren Pico von den Kabelfesseln befreien und es für Sie bequemer machen kann, Pico-Projekte selbst zu erstellen. Alle GPIOs führen nach außen und bieten klare Siebdrucke, die für Pico-Experimente sehr praktisch sind. Die verbleibende Batterieleistung kann an den 4 LED-Anzeigen abgelesen werden. Sie können auch Batteriespannung und Strominformationen lesen, indem Sie das USB-zu-TTL-Kabel an die Pins des seriellen Anschlusses der USV anschließen. Die Ladeaufforderung während des Ladevorgangs ist sehr intuitiv, und wenn der Akku vollständig aufgeladen ist, wird der Ladevorgang beendet und die „Standby-Anzeige“ auf dem Bedienfeld leuchtet auf.

Informationen zum Lesen von Spannung und Strom von der UPS über Pico finden Sie unter [Energieversorgung](wiki.52pi.com/index.php?title=EP-0159)


## Technische Daten

Spannungsversorgung: 1.71 – 3.6 Volt
die meisten Module haben keinen Spannungsregler
VDDIO: 1.71 – 1.95 Volt
Toleranzbereich für I/O-Pins
Kommunikation über I2C, Adressen:
AD0 an LOW: 0x68
AD0 an HIGH: 0x69
Kommunikation über SPI
Gyroskop:
Messbereiche: +/-250, +/-500, +/-1000, +/-2000 °/s
Datenrate: 4.4 Hz – 9 kHz
Beschleunigungssensor:
Messbereiche: +/- 2, +/-4, +/-8, +/-16 g
Datenrate: 4.5 Hz – 4.5 kHz
Magnetometer (AK09916):
Messbereich: +/- 4900 µT
max. Datenrate: 100 Hz
FIFO (first in, first out) Datenspeicher: 512 / 4096 Bytes
Interrupts (die von mir implementierten): FIFO Überlauf, Data Ready, FSync und „Wake-on-Motion“ (Beschleunigungsinterrupt)
Integriertes Thermometer
Der ICM-20948 ermöglicht es, bis zu fünf weitere Sensoren mit einer I2C Hilfsschnittstelle (Auxiliary Interface) zu steuern. Die Messwerte werden in Registern des ICM-20948 gespeichert und von dort ausgelesen.

Das Magnetometer ist nicht wirklich in den ICM-20948 integriert. Es besitzt eigene Register und eine eigene I2C Adresse. Ihr könnt es nur über die eben beschriebene Hilfsschnittstelle erreichen.

## Bezugsquelle
[Amazon Produktseite](https://amzn.eu/d/32H75Oh)

## Foto
<img src="https://wolles-elektronikkiste.de/wp-content/uploads/2021/07/ICM20948_module_small.jpg" width="200">

## Funktionsdiagramm
missing

## Datenblatt
[ICM20948](https://invensense.tdk.com/wp-content/uploads/2016/06/DS-000189-ICM-20948-v1.3.pdf)

[Magnetometer AK09916](https://www.y-ic.es/datasheet/78/SMDSW.020-2OZ.pdf)

### Grundlagen

[WU, Qiuping, et al. A three-stage accelerometer self-calibration technique for space-stable inertial navigation systems. Sensors, 2018, 18. Jg., Nr. 9, S. 2888.](https://pmc.ncbi.nlm.nih.gov/articles/PMC6164698/pdf/sensors-18-02888.pdf)

[SOTO, Hector L. Calibrating a 3-Axis Accelerometer Instrument with a Less Accurate Calibration Device Part 1: Mathematical Methodology. 2020.](https://ntrs.nasa.gov/api/citations/20205005041/downloads/NASA-TM-2020-5005041%20corrected.pdf)

## Anwendungsbeispiel
[Anwendungsbeispiel](https://wolles-elektronikkiste.de/icm-20948-9-achsensensor-teil-i)

### Kalibrierungsbeispiele
[How to Calibrate an Accelerometer](https://github.com/michaelwro/accelerometer-calibration)

## Fritzing Part
missing

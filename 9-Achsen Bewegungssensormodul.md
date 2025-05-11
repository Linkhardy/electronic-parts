# ICM20948 9-Achsen Bewegungssensormodul

## Beschreibung
ICM-20948 ICM20948 9-Achsen Bewegungssensormodul für genaue Trackings und geringen Stromverbrauch in Geräten

Merkmale:
20948 9-Achsen Bewegungssensormodul bietet einen geringen Stromverbrauch, ermöglicht batteriebetriebene Geräte und verlängert die Betriebszeit effizient.
Dieses integriert 3-Achsen Beschleunigungsmesser, Gyroskop und Magnetometer und bietet präzise Bewegungsverfolgung mit Unterstützung für beide I2C Kommunikationsschnittstellen.
für Entwickler, Robotik Enthusiasten und Spiele, die in ihren Projekten präzise Bewegungsverfolgungsfunktionen benötigen.
für den Einsatz in Wearables, Drohnen, Anwendungen und Heimprodukten und ermöglicht eine verbesserte Benutzerinteraktion und stabile Leistungen in verschiedenen Bereichen.
Mit Temperatursensoren und fortschrittlichen Filteralgorithmen gewährleistet der 20948 eine genaue Datenausgabe, minimiert Rauschstörungen und verbessert die Gesamtfunktionalität des Geräts.

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
<img src="Pfad/zum/Bild.jpg](https://wolles-elektronikkiste.de/wp-content/uploads/2021/07/ICM20948_module_small.jpg" width="200">

## Funktionsdiagramm
missing

## Datenblatt
[ICM20948](https://invensense.tdk.com/wp-content/uploads/2016/06/DS-000189-ICM-20948-v1.3.pdf)

[Magnetometer AK09916](https://www.y-ic.es/datasheet/78/SMDSW.020-2OZ.pdf)

## Anwendungsbeispiel
[Anwendungsbeispiel](https://wolles-elektronikkiste.de/icm-20948-9-achsensensor-teil-i)

## Fritzing Part
missing

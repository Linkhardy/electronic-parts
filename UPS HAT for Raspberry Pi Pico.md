# Uninterruptible Power Supply (UPS) HAT for Raspberry Pi Pico

## Beschreibung
Charger Power Bank Power Management Expansion Board for Raspberry Pi Pico/Pico W UPS Power Supply Uninterruptible UPS HAT,Support 18650 Lithium Battery

Merkmale:
Raspberry Pi Pico UPS-Modul

Dies ist ein tragbares Netzteil für den Raspberry Pi Pico.

Es unterstützt die Verwendung einer einzelnen 18650-Lithiumbatterie für die Stromversorgung, die Ihren Pico von den Kabelfesseln befreien und es für Sie bequemer machen kann, Pico-Projekte selbst zu erstellen. Alle GPIOs führen nach außen und sind einzeln, die für Pico-Experimente sehr praktisch sind. Die verbleibende Batterieleistung kann an den 4 LED-Anzeigen abgelesen werden. Sie können auch Batteriespannung und Strominformationen lesen, indem Sie das USB-zu-TTL-Kabel an die Pins des seriellen Anschlusses der USV anschließen. Die Ladeaufforderung während des Ladevorgangs ist sehr intuitiv, und wenn der Akku vollständig aufgeladen ist, wird der Ladevorgang beendet und die „Standby-Anzeige“ auf dem Bedienfeld leuchtet auf.

Informationen zum Lesen von Spannung und Strom von der UPS über Pico finden Sie unter [Energieversorgung]

## Technische Daten
- Plug & Play
- Support Raspberry Pi Pico Only
- Monitor battery voltage (error ±2%), monitor battery current (error ±10%).
- Monitor the charging current.
- If it is not in charging mode, the power LED indicator will not be on, wake up for 5 seconds every 2 minutes to reduce - - light pollution.
- In charging mode, it can judge whether it is fully charged, and stop flashing lights when fully charged.
- In charging mode, the LED will flash when it is not fully charged.
- Evenly allocate the power ratio of each LED to prevent the load from appearing abruptly.
- The static power consumption is less than 10mA.
- Serial output data.
- Power IN: DC 5V/2A
- Only supports 18650 lithium battery

## Bezugsquelle
[Amazon Produktseite]([https://amzn.eu/d/32H75Oh](https://www.amazon.de/dp/B09S5YKBXC))

## Foto
<img src="images/480px-EP-0159-5.jpg" alt="Ueberblick" width="300" style="display:inline-block; margin-right:20px;">
<img src="images/480px-EP-0159-8.jpg" alt="Bild 2" width="300" style="display:inline-block;">


## Verkabelung zum Lesen der Versorgungsdaten
<img src="images/EP-0159接线.jpg" alt="Bild" width="300">

### MircoPython
```Python
from machine import UART, Pin
import time

# create an instance. Connect GP0 to UPS's RX pin, GP1 to UPS's TX pin
uart1 = UART(0, baudrate=115200, tx=Pin(0), rx=Pin(1))

# loop
while True:
    try:
        data = uart1.readline()   # read data from UPS.
        if data != None:
            data = data.decode('utf-8')
            data = data.rstrip('\n')
            print(data)
        
            print("Battery Voltage:{}".format(data.split('|')[0]))
            print("Current of Charging In:{}".format(data.split('|')[1]))
            batt_cur = float(data.split('|')[2]) / 10.0
            print("Consuming Current:{}".format(batt_cur))
        
            sign = data.split('|')[2]
            print("sign: {}".format(sign))
            if float(sign) < 0.0:
                print("Battery is charging....")
            else:
                print("Power is consuming...")
    
        time.sleep(2)
        print("-"*38)
    except ValueError:
        pass
    except IndexError:
        pass
```

## Datenblatt
[EP-0159](wiki.52pi.com/index.php?title=EP-0159)

## Fritzing Part
missing

# Material

## Raspberry Pi 3B+

- Image mit Raspberry Pi Imager erstellt
- GPIO Ausgabespannung 3.3V, max. 16mA/Ausgang (max 60mA Summe)
- Pinout: https://www.seeedstudio.com/blog/2020/02/19/how-to-use-raspberry-pi-gpio-pins-python-tutorial/comment-page-1/

### Software
- Benutername: pi
- Remotedesktop Xrdp (infos @ https://raspberrytips.com/remote-desktop-raspberry-pi/)
- sudo apt-get install xrdp
- sudo journalctl enable ssh

### GPIO commands
- Linux user muss in gpio Gruppe sein
- gpio-Kommando verlangt physische pin nummern (zb 7 für GPIO 4)
- gpio readall
- gpio mode PIN in|out
- gpio write PIT 1|0

## Amazon HiLetgo 8-Kanal-Relais Board

- Alle gleichzeitig ziehen bei 3.3V 6mA vom Raspberry
- DC- : Netzteil - UND Raspberry Ground

# Wiring
- Schwarz       Ground      Pin 6   -
- Weiß/Gelb     Relais 1    Pin 11  GPIO 0
- Weiß/Braun    Relais 2    Pin 13  GPIO 2
- Weiß/Grün     Relais 3    Pin 15  GPIO 3
- Weiß/Lila     Relais 4    Pin 16  GPIO 4
- Gelb/Gelb     Relais 5    Pin 18  GPIO 5
- Gelb/Braun    Relais 6    Pin 22  GPIO 6
- Gelb/Grün     Relais 7    Pin 29  GPIO 21
- Gelb/Lila     Relais 8    Pin 31  GPIO 22

# Programmierung

- npm und Raspberry Pi: https://github.com/fivdi/pigpio/blob/master/doc/gpio.md

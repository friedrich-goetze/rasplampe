# Material

## Raspberry Pi 3B+

- Image mit Raspberry Pi Imager erstellt
- GPIO Ausgabespannung 3.3V, max. 16mA/Ausgang (max 60mA Summe)
- Pinout: https://www.seeedstudio.com/blog/2020/02/19/how-to-use-raspberry-pi-gpio-pins-python-tutorial/comment-page-1/

### Software
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

# Programmierung

- npm und Raspberry Pi: https://github.com/fivdi/pigpio/blob/master/doc/gpio.md

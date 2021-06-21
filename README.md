# virtualbox-linux-setup

- Feste Festplattengröße erzeugen, weil dynamische Festplatten sonst irgendwann zu groß werden könnten.
- Lubuntu installieren (Lubuntu 20.04.2.LTS)
- VM-Einstellungen
  - System
    - Hauptspeicher: möglichst Hoch
    - Prozessoren: möglichst Hoch
  - Anzeige
    - Grafik-Speicher: möglichst Hoch
    - Grafik-Controller: VBoxVGA
    - Beschleunigung: 3D-Beschleunigung aktivieren
  - Allgemein -> Erweitert
    - Gemeinsame Zwischenablage: bidirektional
    - Drag'n'Drop: bidirektional
  - Sonstiges
    - ggf. VM-Monitor (1/2) und Auflösung explizit setzen
    - ggf. Automatische Anpassung der Gastanzeige setzen
- apt-get install perl gcc make 
- as ROOT: GuestEditions einlegen und VBoxLinuxAdditions.run ausführen
  - as ROOT: VBoxClient --clipboard
  - as ROOT: VBoxClient --draganddrop+#
- ggf. Neustart

# lubuntu: Get rid of ^H when hitting Backspace 

stty erase ^H (z. B. wenn gerade mal wieder der ^H-Modus für Backspace aktiv ist)

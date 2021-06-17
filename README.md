# virtualbox-linux-setup

- Feste Festplattengröße erzeugen, weil dynamische Festplatten sonst irgendwann zu groß werden könnten.
- Lubuntu installieren
- VM-Einstellungen
  - System
    - Hauptspeicher: möglichst Hoch
    - Prozessoren: möglichst Hoch
  - Anzeige
    - Grafik-Speicher: möglichst Hoch
    - Grafik-Controller: VBoxVGA
    - Beschleunigung: 3D-Beschleunigung aktivieren
  - Sonstiges
    - ggf. VM-Monitor (1/2) und Auflösung explizit setzen
    - ggf. Automatische Anpassung der Gastanzeige setzen
- apt-get install perl gcc make 
- as ROOT: GuestEditions einlegen und VBoxLinuxAdditions.run ausführen
  - as ROOT: VBoxClient --clipboard
  - as ROOT: VBoxClient --draganddrop


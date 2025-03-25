- Nach etwa 4 Jahren Entwicklung haben wir bereits folgendes an der Hand:

# Boards

- SIPM Board
	- 3 Varianten: Hamamatsu, Sensl und Broadcom
	- Besitzen SiPMs, Test-LEDs und Temperature Sensor für Temperatur Ausgleich
- EMUSCI Board
	- Besitzt Durchgang für Spannung zu SIPM
	- Besitzt EMUSIC amplifier und shaper, discriminator. Alle Ausgänge davon
	- Support. Power Generation für den EMUSIC, Manuelle Kontrolle mit µC onboard
	- Das Board ist aber am Auslaufen. Der EMUSIC wird nicht mehr hergestellt
- Power Boxen
	- Generieren Low Ripple HV, die Temperature Kompensiert ist
	- Generiert Steuerung für EMUSIC
	- Erzeugen Power für EMUSIC board
- Leber Netzteil
	- Generiert Supply für Power Box und das ganze system damit
	- Steuert EMUSIC configuration
- Slow Control
	- Erlaubt Steuerung der Power Boxen via WiFi.

# Infrastruktur

- Johannes Setup
	- Erlaubt es, SiPMs + EMUSIC mit Laserlicht zu testen
	- Liefert in der Theorie 1 photon events und vor allem wiederholbare Ergebnisse. 
	- Erlaubt auch Dark Counts zu Messen.
	- Gerade wieder im Umbau
- Zellen im Keller
	- 3 Zellen mit Szintillator und verschiedenen Reflektoren drin.
	- Erlauben es, Live SiPM Signale von Myonen zu erzeugen und damit Elektronik zu testen
	- Haben Support Infrastruktur zum Befüllen und Leeren.
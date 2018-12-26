# KiCAD

Bibliotheken und Einstellungen für KiCAD

[TOC]

## TODOs
- R.Yageo.MF0 vervollständigen: (https://www.digikey.de/products/de/resistors/through-hole-resistors/53?FV=fffc000d%2C800bd%2Cc0001%2C400001%2C1f140000%2Cffe00035&quantity=0&ColumnSort=2085&page=1&pageSize=25)
- C.Kemet.MLCC.0805 vervollständigen: (https://www.reichelt.de/Vielschicht-SMD-G0805/2/index.html?ACTION=2&LA=2&GROUPID=8048;SID=94W4zLOawQAUAAAOM2boAb1d965e880a477218588e34a86eb72e1)

## Reference designators
Es werden die Bezeichner aus der englischen Wikipedia verwendet (https://en.wikipedia.org/wiki/Reference_designator).
- **A**	Separable assembly or sub-assembly (e.g. printed circuit assembly)
- **AT**	Attenuator or isolator
- **BR**	Bridge rectifier
- **BT**	Battery
- **C**		Capacitor
- **CN**	Capacitor network
- **D**		Diode (including LED, TVS, thyristor, Zener)
- **DL**	Delay line
- **DS**	Display
- **F**		Fuse
- **FB**	Ferrite bead
- **FD**	Fiducial
- **FL**	Filter
- **G**		Generator or oscillator
- **GN**	General network
- **H**		Hardware, e.g., screws, nuts, washers
- **HY**	Circulator or directional coupler
- **J**		Jack (least-movable connector of a connector pair) | Jack connector (connector may have "male" pin contacts and/or "female" socket contacts)
- **JP**	Jumper (Link)
- **K**	Relay or contactor
- **L**	Inductor or coil or ferrite bead
- **LS**	Loudspeaker or buzzer
- **M**	Motor
- **MK**	Microphone
- **MP**	Mechanical part (including screws and fasteners)
- **P**	Plug (most-movable connector of a connector pair) | Plug connector (connector may have "male" pin contacts and/or "female" socket contacts)
- **PS**	Power supply
- **Q**	Transistor (all types)
- **R**	Resistor
- **RN**	Resistor network
- **RT**	Thermistor
- **RV**	Varistor / Variable resistor
- **S**	Switch (all types, including push-buttons)
- **T**	Transformer
- **TC**	Thermocouple
- **TP**	Test point
- **TUN**	Tuner
- **U**	Integrated circuit (IC)
- **V**	Vacuum tube
- **VR**	Voltage regulator (voltage reference) / Variable resistor (potentiometer or rheostat)
- **X**	Socket connector for another item not P or J, paired with the letter symbol for that item (XV for vacuum tube socket, XF for fuse holder, XA for printed circuit assembly connector, XU for integrated circuit connector, XDS for light socket, etc.)
- **XTAL**	Crystal
- **Y**	Crystal or oscillator
- **Z**	Zener diode

## Einstellungen
### Symbol-Editor
- Masseinheiten sind imperial.
- Raster ist 0.1 inch. Pins und Texte werden in diesem Raster abgelegt. **Ausnahme:** Symbolzeichnungen und Nebenbeschriftungen können ein feineres Raster verwenden.
- Hauptbeschriftungen sind 50 mil.
- Nebenbeschriftungen sind 40 mil.
- Datenblätter befinden sich im gleichen Verzeichnis wie die Symbolbibliotheken. Der Name entspricht der Symbolbibliothek und kann durch einen Punkt getrennt noch spezielle Namenszusätze haben (vom Allgemeinen ins Spezielle).
- Die ID ist eine Sonderbeschriftung, kursiv und hat eine Höhe von 25 mil.
- Die Pinnummer ist 50 mil groß.
- Der Pinname ist 50 mil groß. Bei größeren Namen überdecken sich Überstriche und Unterstriche.

### Schaltplan-Editor
- Masseinheiten sind imperial
- Raster ist 0.1 inch. Symbole aus den Originalbibliotheken deren Pins noch im 0.05 inch Raster liegen, müssen in eine eigene Bibliothek überführt werden.
- Die Größe von globalen Labeln ist 50 mil.

### Board-Editor
- Masseinheiten sind imperial.
- Das Raster ist in Vielfachen von 50 mil.

## Verwendung
### Symbol-Editor
- Alle Bauteile bekommen mindestens folgende Felder:
	- Reference (70 mil)
	- Value (70 mil)
	- Footprint (40 mil, nicht sichtbar)
	- Datasheet (40 mil, nicht sichtbar)
	- Package (70 mil, verkürzte Form des Footprint)
	- ID (25 mil, kursiv, Bauteilnummer - meist eine Herstellerbezeichnung)
	
### Layer Setup
#### Zwei Lagen:
- Board Thickness: 1.6 mm

##### Global Design Rules
- Minimum Track Width: 0.1524 mm / 6 mil
- Minimum Via Diameter: 0.6096 mm / 24 mil
- Minimum Via Drill: 0.3048 mm / 12 mil

##### Net Classes
- Default
	- Clearance: 0.1524 mm / 6 mil
	- Track Width: 0.4064 mm / 16 mil
	- Via Dia: 1.016 mm / 40 mil
	- Via Drill: 0.6 mm / 23.62204724 mil

##### Custom Track Width
- 8 mil
- 12 mil
- 16 mil
- 24 mil
- 36 mil
- 48 mil
- 72 mil
- 144 mil
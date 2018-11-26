# KiCAD

Bibliotheken und Einstellungen für KiCAD

[TOC]

## TODOs
- R.Yageo.RC0805 vervollständigen: ab hier: (https://www.digikey.de/products/de/resistors/chip-resistor-surface-mount/52?FV=ffec1104%2Cfffc000d%2Cc0001%2C1c0002%2C400006%2C1f140000%2Cffe00034&quantity=0&ColumnSort=0&page=6&pageSize=25)

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
- Masseinheiten sind imperial
- Raster ist 0.1 inch. Pins und Texte werden in diesem Raster abgelegt. Symbolzeichnungen können ein feineres Raster verwenden.
- Hauptbeschriftungen sind 0.07 inch
- Nebenbeschriftungen sind 0.04 inch
- Datenblätter befinden sich im gleichen Verzeichnis wie die Symbolbibliotheken. Der Name entspricht der Symbolbibliothek und kann durch einen Punkt getrennt noch spezielle Namenszusätze haben (vom Allgemeinen ins Spezielle).
### Schaltplan-Editor
- Masseinheiten sind imperial
- Raster ist 0.1 inch. Symbole aus den Originalbibliotheken deren Pins noch im 0.05 inch Raster liegen, müssen in eine eigene Bibliothek überführt werden.
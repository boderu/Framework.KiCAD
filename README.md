# KiCAD

Bibliotheken und Einstellungen für KiCAD

[TOC]

## TODOs

- vervollständigen: (https://www.digikey.de/products/de/capacitors/tantalum-capacitors/59?k=scs&pkeyword=&sv=0&sf=1&FV=fffc01de%2Cc0003%2C1140050%2Cffe0003b%2C1c0003&quantity=&ColumnSort=2049&page=1&stock=1&rohs=1&pageSize=250)

## Reference designators

Es werden die Bezeichner aus der englischen Wikipedia verwendet (https://en.wikipedia.org/wiki/Reference_designator).

- **A**        Separable assembly or sub-assembly (e.g. printed circuit assembly)
- **AT**    Attenuator or isolator
- **BR**    Bridge rectifier
- **BT**    Battery
- **C**        Capacitor
- **CN**    Capacitor network
- **D**        Diode (including LED, TVS, thyristor, Zener)
- **DL**    Delay line
- **DS**    Display
- **F**        Fuse
- **FB**    Ferrite bead
- **FD**    Fiducial
- **FL**    Filter
- **G**        Generator or oscillator
- **GN**    General network
- **H**        Hardware, e.g., screws, nuts, washers
- **HY**    Circulator or directional coupler
- **J**        Jack (least-movable connector of a connector pair) | Jack connector (connector may have "male" pin contacts and/or "female" socket contacts)
- **JP**    Jumper (Link)
- **K**        Relay or contactor
- **L**        Inductor or coil or ferrite bead
- **LS**    Loudspeaker or buzzer
- **M**        Motor
- **MK**    Microphone
- **MP**    Mechanical part (including screws and fasteners)
- **P**        Plug (most-movable connector of a connector pair) | Plug connector (connector may have "male" pin contacts and/or "female" socket contacts)
- **PS**    Power supply
- **Q**        Transistor (all types)
- **R**        Resistor
- **RN**    Resistor network
- **RT**    Thermistor
- **RV**    Varistor / Variable resistor
- **S**        Switch (all types, including push-buttons)
- **T**        Transformer
- **TC**    Thermocouple
- **TP**    Test point
- **TUN**    Tuner
- **U**        Integrated circuit (IC)
- **V**        Vacuum tube
- **VR**    Voltage regulator (voltage reference) / Variable resistor (potentiometer or rheostat)
- **X**        Socket connector for another item not P or J, paired with the letter symbol for that item (XV for vacuum tube socket, XF for fuse holder, XA for printed circuit assembly connector, XU for integrated circuit connector, XDS for light socket, etc.)
- **XTAL**    Crystal
- **Y**        Crystal or oscillator
- **Z**        Zener diode

## Einstellungen

### Symbol-Editor

- Masseinheiten sind imperial.
- Raster ist 0.1 inch (100mil). Pins und Texte werden in diesem Raster abgelegt. **Ausnahme:** Symbolzeichnungen und Nebenbeschriftungen können ein feineres Raster verwenden.
- Hauptbeschriftungen sind 50 mil.
- Nebenbeschriftungen sind 40 mil.
- ~~Datenblätter befinden sich im gleichen Verzeichnis wie die Symbolbibliotheken. Der Name entspricht der Symbolbibliothek und kann durch einen Punkt getrennt noch spezielle Namenszusätze haben (vom Allgemeinen ins Spezielle).~~
- Die ID ist eine Sonderbeschriftung, kursiv und hat eine Höhe von 25 mil.
- Die Pinnummer ist 50 mil groß.
- Der Pinname ist 50 mil groß. Bei größeren Namen überdecken sich Überstriche und Unterstriche.

### Schaltplan-Editor

- Masseinheiten sind imperial
- Raster ist 0.1 inch (100mil). Symbole aus den Originalbibliotheken deren Pins noch im 0.05 inch Raster liegen, müssen in eine eigene Bibliothek überführt werden.
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
- In den Layern F.Courtyard bzw. B.Courtyard mit Linien/Rechteck/Kreisen/Polygonen! die Sperrflächen für andere Bauteile einzeichnen
- In den Layern F.Fab bzw. B.Fab die Bauteilumrisse zeichnen
- In den Layern F.Silkscreen bzw. B.Silkscreen den Bestückungsdruck zeichnen
- Pins werden im 100mil-Raster angelegt

### Layer Setup

#### Zwei Lagen:

- Board Thickness: 1.6 mm

##### Global Design Rules

- Minimum Track Width: 0.1524 mm / 6 mil
- Minimum Via Diameter: 0.6096 mm / 24 mil
- Minimum Via Drill: 0.3048 mm / 12 mil
- Minimum µVia Diameter: 8 mil (tbd)
- Minimum µVia Drill: 4 mil (tbd)
- Minimum hole to hole: 0.3048 mm / 12 mil (tbd)

##### Net Classes

- Default
  - Clearance: 0.1524 mm / 6 mil
  - Track Width: 0.4064 mm / 16 mil
  - Via Size/Dia: 1.016 mm / 40 mil
  - Via Drill: 0.6 mm / 15.24 mil
  - µVia Size/Dia: (tbd)
  - µVia Drill: (tbd)

##### Custom Track Width

- 8 mil: kann sicher gefertigt werden - passt durch zwei SO-Pins hindurch
- 12 mil
- 16 mil
- 24 mil
- 36 mil
- 50 mil
- 75 mil
- 100 mil
- 150 mil
- 200 mil

##### Custom Vias Size/Drill

- 40/15.24 mil

#### Solder Mask

- Solder mask clearance: 3 mil
- Solder mask minimum wisth: 4 mil
- Solder paste clearance: -0 mil
- Solder paste ratio clearance: -0%
- 

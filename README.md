# KiCad Third-Party Tools

> A curated list of third-party tools to be used in conjunction with the
[KiCad](http://kicad-pcb.org/) open-source electronics design
automation suite.

*Please read the [contribution guidelines](contributing.md) before contributing.*



## Table of Contents

<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Schematic Tools](#schematic-tools)
    - [Schematic Entry Tools](#schematic-entry-tools)
    - [Symbol Library Tools](#symbol-library-tools)
    - [Bill of Materials (BOM) Tools](#bom-tools)
- [PCB Layout Tools](#pcb-layout-tools)
    - [Footprint Library Tools](#footprint-library-tools)
    - [Layout Tools](#layout-tools)
    - [3D Model Tools](#3d-model-tools)

<!-- /TOC -->



## Schematic Tools

### Schematic Entry Tools

- [Skidl](http://xesscorp.github.io/skidl) - A  module that allows you
to compactly describe the interconnection of electronic circuits and components
using Python. The resulting Python program performs electrical rules checking
for common mistakes and outputs a netlist that serves as input to
a PCB layout tool such as KiCad's PCBNEW.

- [KiField](https://xesscorp.github.io/KiField) - A utility for manipulating
part fields in KiCad schematics. KiField can extract all the component fields
from a schematic and place them into a spreadsheet for bulk editing, after
which you can insert the edited values from the spreadsheet back into the schematic.


### Symbol Library Tools

- [Kicad-tools/libgen](https://github.com/boseji/Kicad-tools/tree/master/libgen) - A Python script to generate schematic symbols from XML input.

- [Quick Library Generator](http://kicad.rohrbacher.net/quicklib.php) - A web service to generate common "box type" symbols for ICs from pin descriptions.

- [KiPart](https://xesscorp.github.io/KiPart) - A utility that generates single
and multi-unit symbols from a CSV file containing all the pin information for
one or more parts.

- [KiField](https://xesscorp.github.io/KiField) - A utility for manipulating
part fields in KiCad symbol libraries. KiField can extract all the component fields
from a library and place them into a spreadsheet for bulk editing, after
which you can insert the edited values from the spreadsheet back into the library.

- [QEDA](https://github.com/qeda/qeda)
QEDA is a Node.js library aimed to simplify the creation of Kicad libraries of electronic components. Qeda creates both symbols for Eeschema libraries and IPC7351 Compliant footprints for PcbNew placement.

- [kicadLibCreator](https://github.com/pioupus/kicadLibCreator)
KicadLibCreator is a tool which will generate 'atomic' parts from an Octopart query. By setting up some simple rules, entering a part number in the Octopart search and selecting the appropriate model will add a fully defined component with a consistant style to any library.

- [KiCAD Part Manager](http://mikecrash.com/index.php?name=Content&pa=showpage&pid=10)
Part manager for KiCAD electronic design suite. Based on a MySQL database of components with ability to categorize parts, store part name, part label and part number, description, parameters and also stock count and price. Parts can be assigned to components in KiCAD schematic based on component name, type and value.

- [KiCad Librarian](http://www.compuphase.com/electronics/kicadlibrarian_en.htm)
The KiCad Librarian is a utility to manage and maintain libraries with schematic symbols and footprints. It supports the KiCad EDA suite.
Allows components to be moved between libraries, footprints adjusted etc. Can connect to a server based repository of components to facilitate sharing between workstations.

- [Kicad Multiedit](http://www.xonelectronics.it/download/kicad-medit/)
Simple way of editing large number of components in spreadsheet type view. Will parse the values and footprints of components found
in a KiCAD schematic.

- [KiLibMan](http://www.xonelectronics.it/download/kicad/)
A utility to examine library components and move them between libraries.


### BOM Tools

- [KiCost](https://xesscorp.github.io/KiCost) - A utility that generates a
spreadsheet from a schematic filled with the part pricing information scraped
from distributors like Digi-Key, Mouser, etc. For each distributor and part,
the spreadsheet contains the quantity-dependent prices, available quantities,
link to the part page, and ordering codes.

- [KiCad_BOM_Wizard](https://github.com/HashDefineElectronics/KiCad_BOM_Wizard)
This KiCad plugin can be used to create custom BOM files based on easy configurable templates files. The plugin is writing in JavaScript and has been designed to integrate into KiCad’s BOM plugin manager. Exports CSV, HTML and PDF files. The template files permit customisation of output to include (for example) certification docs, logo etc. KiCad_BOM_Wizard will  group and sort all components together that have same parts value, the same starting designator reference prefix and the same fields value.

- [BOMs Away](https://github.com/Jeff-Ciesielski/Boms-Away)
A Component/BOM Management tool for KiCad. Maintains a local database of components and facilitates associating components on schmatic with identified parts. Simply enter a part's manufacturer, supplier, manufacturer PN, and supplier PN then click 'save to datastore'. Information is keyed off of component value and footprint, so future uses can simply use the part lookup button to retrieve the information. Multiple suppliers, manufacturers, and part numbers are supported. (wxPython)

## PCB Layout Tools

### Footprint Library Tools

- [Kicad-tools/modgen](https://github.com/boseji/Kicad-tools/tree/master/modgen) - A Python Tkinter GUI for creating footprints.

- [monostable/kicad_footprints](https://github.com/monostable/kicad_footprints) - A collection of all the KiCad footprints available on the internet and some scripts to manage them.

- [svg2mod](https://github.com/mtl/svg2mod) - A tool to convert multi-layer Inkscape SVGs into footprints.

- [xess_fp_wizard.py](https://github.com/xesscorp/xess_fp_wizard) - A utility
to make footprints for chips having pins around the periphery (SOICs, QFP, etc.)
and ball grid arrays (BGAs).

- [pointhi/kicad-footprint-generator](https://github.com/pointhi/kicad-footprint-generator) - Python library for generating footprints. The scripts subdirectoy contains the footprints that are already scripted with this tool.

### Layout Tools

- [Laksen/kicad-bga-tools](https://github.com/Laksen/kicad-bga-tools) - A script to generate via fanouts for BGA components on a board.

- [panelize.py](http://projects.borg.ch/electronics/kicad/panelize.html) - A script to create panels. It can copy, rotate and flip rectangular areas from one or more PCB files into a new PCB file.

- [RenumKicadPCB](https://documenteddesigns.com/2017/03/27/renumkicadpcb-v0203/) - RenumKiCadPCB processes a KiCad PCB file and renumbers all the component reference designators ending in numbers based on where they are located on the PCB. It then processes the schematic hierarchy and updates the component reference designators to match. This makes working on a board much easier since you can locate all the components. The download includes a user manual, Windows executable and instructions for compiling to run on Linux.

### 3d Model tools

- [kicad StepUp](https://sourceforge.net/projects/kicadstepup/) - A tool to allign 3d files to their respective footprint. To use these models in kicad they can be exported as step and correctly scaled wrl. This tool is also capable to export a KiCad PCB as a step file.

- [cadquery 3d model generator](https://github.com/easyw/kicad-3d-models-in-freecad/tree/master/cadquery/FCAD_script_generator) - 3d model generators using freecad and the cadquery plugin. The scripts generate step and scaled wrl files similar to kicad stepup.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [XESS Corp.](http://xess.com) has waived all copyright and related or neighboring rights to this work.

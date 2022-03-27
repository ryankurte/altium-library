# Altium Library

My altium footprints and schematic symbols as an excel-backed database library.

**While most components have been verified and used, no guarantees are made to accuracy, please check footprints / symbols / pinouts against manufacturer datasheets prior to use (and raise an issue if you find any inconsistencies)**

If you would like to add a component or suggest an alteration, open an issue or a pull request.  

## Installing

Add altium-library.dblib to your project or to the environment using `DXP->Preferences->Data Management->Installed` Libraries

## Adding components

Note that due to limitations of excel you will need to open the excel database file prior to opening altium to ensure excel has write access.

### If the component does not exist

1. Create a Schematic library file containing the schematic symbol in `symbols/`
2. If there is not already an existing footprint, create a PCB Library containing the component footprint in `footprints/`
3. Add a line to `electronpowered.xls` in the applicable sheet
4. Right click on the library and refresh in altium.

### If the symbol / footprint already exist

For resistors values or other like components:

1. Open the database file `electronpowered.xls`
2. Locate the closest component (ie. `RES-SM-0603-33K`)
3. Copy the component line
4. Paste into a new line
5. Alter the appropriate fields
6. Right click on the library and refresh in altium.


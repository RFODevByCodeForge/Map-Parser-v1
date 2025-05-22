# Batch Convert Tool for RF Map Files

This is a command-line tool for batch converting `.dat` files to `.xlsx` and vice versa, designed for handling map files in Rising Force Nexus projects.

## Features

- Convert all valid `.dat` files in multiple map folders to `.xlsx` format
- Convert all `.xlsx` files back to `.dat`
- Automatically skips files related to portals
- Checks and creates missing folders/files as needed
- Simple command-line interface with three modes

## Usage

Run the executable from a command prompt (terminal) with the following syntax:

MapParser.exe --mode [bin_to_xlsx | xlsx_to_bin | check-files]

## Modes

- `bin_to_xlsx`  
  Converts `.dat` files in `gu_out` folder to `.xlsx` files in `gu_in`.

- `xlsx_to_bin`  
  Converts `.xlsx` files in `gu_in` folder to `.dat` files in `gu_out`.  
  Automatically creates missing `.xlsx` files from `.dat` if needed.

- `check-files`  
  Checks for missing `.xlsx` files in `gu_in` and creates them from `.dat` files in `gu_out`.

## Folder Structure

- `gu_out/` — Contains `.dat` files, organized in map subfolders
- `gu_in/` — Contains `.xlsx` files, organized in corresponding map subfolders

Make sure both folders are in the same directory as the executable.

## Notes

- Files related to portals (e.g. files containing `-portal`, `[portal]`) are excluded from conversion.
- The tool prints progress and error messages to the console.
- Requires Python environment for original `.py` scripts if you want to modify the tool.

## Example

Convert `.dat` files to `.xlsx`:

MapParser.exe --mode bin_to_xlsx

Convert `.xlsx` files to `.dat`:

MapParser.exe --mode xlsx_to_bin

Check and create missing `.xlsx` files:

MapParser.exe --mode check-files

If you encounter issues or have questions, please contact the developer.

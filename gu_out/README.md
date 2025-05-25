# gu_out

This folder contains the output `.dat` files used in RF map projects.

## Structure

- Files are organized into subfolders per map.
- Each `.dat` file represents structured binary data for in-game maps.

## Usage

- When using `MapParser.exe` with `--mode xlsx_to_bin`, `.xlsx` files from `gu_in` will be converted into `.dat` files here.
- When using `--mode bin_to_xlsx`, the tool reads the `.dat` files from here to generate `.xlsx` files in `gu_in`.

## Notes

- Files with names containing `-portal` or `[portal]` are skipped automatically.
- Ensure all `.dat` files are correctly placed in map-named subfolders.

## Example Path
gu_out/
└── Platform01/
    └── Plaform01-[Block].dat

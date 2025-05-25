# gu_in

This folder holds the editable `.xlsx` files used in RF map file editing.

## Structure

- Files are grouped into subfolders based on the map name.
- Each `.xlsx` file is a human-readable version of its corresponding `.dat` file.

## Usage

- Use `MapParser.exe` with `--mode xlsx_to_bin` to convert these files into `.dat` files inside `gu_out`.
- If you're using `--mode check-files`, missing `.xlsx` files will be automatically created from the `.dat` files in `gu_out`.

## Notes

- Files related to portals (e.g., filenames containing `-portal` or `[portal]`) are skipped by the tool.
- Keep this structure clean and mirror the map folder layout in `gu_out`.

## Example Path
```
gu_in/
└── Platform01/
    └── Platform01-[Block].xlsx
```

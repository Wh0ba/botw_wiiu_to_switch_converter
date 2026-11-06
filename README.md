# Breath of the Wild Wii U → Switch Save Converter

A small, browser-based tool for converting *The Legend of Zelda: Breath of the Wild* save files from Wii U format to Switch format. The app is a single static HTML file; conversion happens locally in your browser, and save files are not uploaded.

## Use it

1. Open [`index.html`](./index.html) in a modern browser. No installation, build step, or server is required.
2. Add the Wii U save files to **Wii U files** and a valid Switch save from the same game to **Switch files**. Browse for files or drag and drop them into the corresponding panel.
3. Download each converted file or select **Download all (.zip)**.
4. Back up the entire Switch save slot before replacing anything. Replace only the generated files and leave the other files in the slot unchanged.

The converter recognizes `game_data.sav`, `caption.sav`, and the optional Wii U `caption.jpg`. It converts each `.sav` file only when both the Wii U source and Switch template are provided. The Switch save supplies the target file layout; the Wii U `caption.jpg`, when selected, is copied to the output without conversion.

## Compatibility and cautions

- This is an unofficial conversion. The page warns that conversion from Wii U v1.5 to Switch v1.8 may not be accepted by every game or emulator build.
- The converter reports Switch-only entries retained from the template and Wii U entries dropped during conversion. Review these notes after conversion.
- Always keep an untouched backup of your Switch save. Use the output at your own risk.
- This tool converts save files; it does not transfer saves to a console or emulator.

## Development

There are no dependencies or build tools. Edit `index.html` and open it in a browser to test the app.

## Related resource

For editing a save rather than converting it, see [The Save Editor by Marc Robledo](https://www.marcrobledo.com/savegame-editors/zelda-botw/).

# Image Renamer — abbies®

A lightweight, self-contained browser tool for batch-renaming image files with a prefix code — built for AI image organization and beyond.

No installation. No server. No dependencies. Just open the HTML file and go.

---

## Features

- **Random prefix codes** — generate a unique 5-character code per file, in alphanumeric, letters-only, or numbers-only format
- **Sequential numbering** — count up from any starting number you choose (e.g. `00000`, `00042`, `01000`), with optional zero-padding to 5 digits
- **Live preview** — see exactly what every file will be renamed to before you commit
- **Thumbnail grid** — visual preview of your loaded images
- **Batch ZIP download** — all renamed files packed into a single `renamed_images.zip`, ready to extract
- **Fully offline** — the entire tool runs in your browser; your files never leave your machine
- **50+ file support** — chunked loading with a progress bar keeps things smooth on large batches
- **Separator options** — underscore, dash, or none between the code and the original filename
- **Case control** — uppercase or lowercase codes

---

## How To Use

1. Download `image_renamer_abbies.html`
2. Double-click it to open in any modern browser (Chrome, Firefox, Edge)
3. Drop your images onto the drop zone, or click to browse
4. Choose your code mode and options
5. Preview the new filenames in the table
6. Hit **Download ZIP** — your renamed files will arrive in your downloads folder as `renamed_images.zip`

---

## Code Modes

**Random** — each file gets its own randomly generated 5-character code. Good for creating unique, non-sequential identifiers across large collections.

**Sequential** — files are numbered in order starting from whatever number you enter. Great for building an organized, sortable catalog. Enable zero-padding to always get a consistent 5-digit format like `00001`, `00002`, etc.

---

## Supported File Types

JPG · PNG · WEBP · GIF · AVIF · BMP · TIFF

---

## Technical Notes

- Built as a single self-contained `.html` file — no frameworks, no CDN calls, no external dependencies at runtime
- ZIP files are assembled in-browser using a hand-rolled ZIP writer with CRC-32 checksums — no library required
- Files are processed in chunks of 25 to prevent the browser from freezing on large batches
- Your original files are never modified; renamed copies are written into the ZIP only

---

## Browser Compatibility

Works in any modern browser that supports the File API and async/await — Chrome 80+, Firefox 75+, Edge 80+, Safari 14+.

---

## License

MIT — free to use, modify, and distribute.

---

*Made with abbies®*

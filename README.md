# Polyglot Opening Books

A collection of [Polyglot](http://hgm.nubati.net/book_format.html) (`.bin`) opening books for chess engines, for use with the **Chess System Tal** engine and any other UCI engine that supports Polyglot books.

Because some of these files are large (up to ~170 MB), the books are **not** stored in this git repository — they are published as zipped assets on the [**Releases**](../../releases/latest) page. Each book is a separate `.zip` containing one `.bin` file, so you can grab only the ones you want.

## Community books

Freely-distributed Polyglot books gathered from public sources (see **Credits**). Provided as-is, for convenience.

| Book | `.bin` size | Entries¹ | Source | Download |
|------|------------:|---------:|--------|----------|
| `book.bin` | 169.7 MB | 11,123,374 | Jeroen Noomen (Rebel) | [book.zip](../../releases/latest/download/book.zip) |
| `uho-pohl.bin` | 76.7 MB | 5,027,499 | Stefan Pohl (UHO) | [uho-pohl.zip](../../releases/latest/download/uho-pohl.zip) |
| `codekiddy.bin` | 15.7 MB | 1,030,253 | CodeKiddy collection | [codekiddy.zip](../../releases/latest/download/codekiddy.zip) |
| `komodo.bin` | 8.8 MB | 578,126 | Salvo Spitaleri (Komodo) | [komodo.zip](../../releases/latest/download/komodo.zip) |
| `DCbook_large.bin` | 6.1 MB | 398,022 | CodeKiddy collection | [DCbook_large.zip](../../releases/latest/download/DCbook_large.zip) |
| `Book-ck.bin`² | 5.5 MB | 360,125 | CodeKiddy collection | [Book-ck.zip](../../releases/latest/download/Book-ck.zip) |
| `gavibook.bin` | 5.1 MB | 333,577 | CodeKiddy collection | [gavibook.zip](../../releases/latest/download/gavibook.zip) |
| `KomodoVariety.bin` | 4.1 MB | 267,489 | CodeKiddy collection | [KomodoVariety.zip](../../releases/latest/download/KomodoVariety.zip) |
| `final-book.bin` | 2.8 MB | 183,804 | CodeKiddy collection | [final-book.zip](../../releases/latest/download/final-book.zip) |
| `rodent.bin` | 2.7 MB | 175,355 | Paweł Kozioł (Rodent) | [rodent.zip](../../releases/latest/download/rodent.zip) |
| `baron30.bin` | 2.5 MB | 163,141 | Richard Pijl (The Baron) | [baron30.zip](../../releases/latest/download/baron30.zip) |
| `Elo2400.bin` | 2.4 MB | 155,878 | CodeKiddy collection | [Elo2400.zip](../../releases/latest/download/Elo2400.zip) |
| `Performance.bin` | 1.4 MB | 92,954 | CodeKiddy collection | [Performance.zip](../../releases/latest/download/Performance.zip) |
| `varied.bin` | 1.4 MB | 92,229 | CodeKiddy collection | [varied.zip](../../releases/latest/download/varied.zip) |
| `gavibook-small.bin` | 0.68 MB | 44,694 | CodeKiddy collection | [gavibook-small.zip](../../releases/latest/download/gavibook-small.zip) |
| `Jeroen.bin` | 0.64 MB | 41,733 | Jeroen Noomen (Rebel) | [Jeroen.zip](../../releases/latest/download/Jeroen.zip) |
| `fruit.bin` | 0.48 MB | 31,467 | Fruit engine book | [fruit.zip](../../releases/latest/download/fruit.zip) |
| `gm2001.bin` | 0.46 MB | 30,416 | Oliver Deville (GM 2001–2013, ≥2530) | [gm2001.zip](../../releases/latest/download/gm2001.zip) |
| `gm2600.bin` | 0.33 MB | 21,671 | CodeKiddy collection | [gm2600.zip](../../releases/latest/download/gm2600.zip) |
| `Daring.bin` | 0.29 MB | 19,152 | Jeroen Noomen (Rebel) | [Daring.zip](../../releases/latest/download/Daring.zip) |
| `Rebel.bin` | 0.29 MB | 18,990 | Jeroen Noomen (Rebel) | [Rebel.zip](../../releases/latest/download/Rebel.zip) |
| `Variety.bin` | 0.17 MB | 11,387 | Jeroen Noomen (Rebel) | [Variety.zip](../../releases/latest/download/Variety.zip) |

¹ Each Polyglot entry is a position–move pair (16 bytes); a single position may have several entries.
² The CodeKiddy collection's `Book.bin`, renamed to avoid colliding with the large `book.bin` above.

## Usage

1. Download and unzip the book you want.
2. Point your UCI engine at the `.bin` file — in Chess System Tal, set the **Book File** option (or your GUI's Polyglot book setting) to the unzipped `.bin`.
3. Enable book play (e.g. **OwnBook = true**) if your GUI exposes it.

## For engine authors

Polyglot and Zobrist docs — the `.bin` entry layout, move encoding, and the Zobrist hashing keys used to index positions: <http://hgm.nubati.net/book_format.html>

## Credits

The books were collected from publicly available sources, including:

- The [**CodeKiddy** Polyglot book collection](https://sourceforge.net/projects/codekiddy-chess/files/Books/Polyglot%20books/) (SourceForge).
- [**donna_opening_books**](https://github.com/michaeldv/donna_opening_books) — `gm2001` (Oliver Deville), `komodo` (Salvo Spitaleri), `rodent` (Paweł Kozioł).
- [**The Baron**](https://rebel13.nl/) book by Richard Pijl.
- Jeroen Noomen's Rebel/ProDeo books ([rebel13.nl](https://rebel13.nl/)).
- Stefan Pohl's [UHO openings](https://www.sp-cc.de/) (converted to Polyglot format).

All opening books remain the work of their respective authors and are provided here as-is for use with chess engines.

## License

This repository's text (README) is provided as-is. The opening books are the property of their respective authors; see **Credits**.

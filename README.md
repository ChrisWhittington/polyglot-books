# Polyglot Opening Books

A collection of [Polyglot](http://hgm.nubati.net/book_format.html) (`.bin`) opening books for chess engines, as used with the **Chess System Tal** engine and any other UCI engine that supports Polyglot books.

Because some of these files are large (up to ~170 MB), the books are **not** stored in this git repository — they are published as zipped assets on the [**Releases**](../../releases/latest) page.

## Download

Each book is a separate `.zip` containing one `.bin` file. Grab only the ones you want.

| Book | `.bin` size | Entries¹ | Download |
|------|------------:|---------:|----------|
| `book.bin` | 169.7 MB | 11,123,374 | [book.zip](../../releases/latest/download/book.zip) |
| `uho-pohl.bin` | 76.7 MB | 5,027,499 | [uho-pohl.zip](../../releases/latest/download/uho-pohl.zip) |
| `Jeroen.bin` | 0.64 MB | 41,733 | [Jeroen.zip](../../releases/latest/download/Jeroen.zip) |
| `Rebel-last-one-jeroen.bin` | 0.64 MB | 41,733 | [Rebel-last-one-jeroen.zip](../../releases/latest/download/Rebel-last-one-jeroen.zip) |
| `fruit.bin` | 0.48 MB | 31,467 | [fruit.zip](../../releases/latest/download/fruit.zip) |
| `Daring.bin` | 0.29 MB | 19,152 | [Daring.zip](../../releases/latest/download/Daring.zip) |
| `Rebel.bin` | 0.29 MB | 18,990 | [Rebel.zip](../../releases/latest/download/Rebel.zip) |
| `Variety.bin` | 0.17 MB | 11,387 | [Variety.zip](../../releases/latest/download/Variety.zip) |

¹ Each Polyglot entry is a position–move pair (16 bytes); a single position may have several entries.

## Usage

1. Download and unzip the book you want.
2. Point your UCI engine at the `.bin` file — in Chess System Tal, set the **Book File** option (or your GUI's Polyglot book setting) to the unzipped `.bin`.
3. Enable book play (e.g. **OwnBook = true**) if your GUI exposes it.

## License

The opening books are provided as-is for use with chess engines.

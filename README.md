# tml - Text to HTML Converter

## Overview

`tml` is a simple command-line tool that converts `.txt` and `.md` files into `.html` format. The tool automatically wraps paragraphs from the input `.txt` or `.md` file in `<p>...</p>` or `h1, h2, h3` tags respectively in the resulting `.html` file.

## Installation

To install `tml`, simply clone this repository to your local machine.

```
git clone https://github.com/mnajibi/tml.git
cd tml
```

Ensure `main.py is` executable:

```
chmod +x main.py
```
## Usage

By default, if no output directory is specified, the `.html` files will be saved inside the `tml/examples` directory.

### Txt to HTML
To convert a `.txt` file to `.html`:

```
./main.py <path-to-txt-file>
```

To specify a different output directory:

```
./main.py <path-to-txt-file> --output <path-to-output-directory>
```
### md to HTML

To convert a `.md` file to `.html`:

```
./main.py <path-to-md-file>
```

To specify a different output directory:

```
./main.py <path-to-md-file> --output <path-to-output-directory>
```

## Command Options:
| Options | Description |
| --- | --- |
| `--version` or `-v` | Display the tool's version. |
| `path` | Specify the path to a `.txt` or `.md` file or a directory containing multiple .txt files. If a directory is provided, `tml` will recursively process all `.txt` or `.md` files within. |
| `--output` or `-o` | Specify a custom output directory. The tool will create the directory if it does not exist. |

## Features

* 📄 Converts single or multiple `.txt` and `.md` files to `.html`.
* 🖋 Automatic paragraph wrapping in `<p>...</p>` tags.
* 🖋 Automatic heading wrapping in h1, h2 ,h3 based on number of # specified in the `.md` file.
* 📁 Can output to a custom directory or default to `tml/examples`.
* 🔄 Overwrites existing output directory content to ensure it contains only the most recent outputs.
* 🎉 Extracts title from the text file if present. The title is identified as the first line followed by two blank lines.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

## License

[MIT](https://github.com/mnajibi/tml/blob/main/LICENSE)


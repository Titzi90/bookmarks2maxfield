# bookmarks2maxfield.py

## Description

Input generator for Ingress Maxfield (http://www.ingress-maxfield.com), which
uses the export of the IITC Bookmarks Plugin as input.

## Prerequisites

You'll need Python (version 2 and 3 is considered supported) as well as
docopt.

Install python-docopt package if required and available. Otherwise install
docopt via:

```
pip install docopt
```

## How To Use

1. Mark your portal set in IITC as bookmarks (Bookmarks Plugin).
2. Export it as file.
3. Run `bookmarks2maxfield.py` with the exported file as `<input_file>` and
use the result (standard output or content of `<output_file>`) as input for
Ingress Maxfield (http://www.ingress-maxfield.com)

## Usage

```
bookmarks2maxfield.py <input_file> [<output_file>]
```

### Options

```
input_file:
  IITC Bookmark Plugin export in JSON format, e.g. 'bookmarks.json'

output_file:
  generated output in CSV format, e.g. 'maxfield.csv'
```

## Sample Files
These are for a portal set of 'Hummelsteiner Park, Nuremberg, Germany'

```
'bookmarks-sample.json':
  Sample file for IITC Bookmark Plugin export

'maxfield-sample.csv'
  Sample file for generated output
```

`maxfield-sample.csv` has been generated by `bookmarks2maxfield.py` with
`bookmarks-sample.json` as `input_file`.

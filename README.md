# StructureSheet

[StructureSheet](https://github.com/dotancohen/structuresheet) is a structured spreadsheet application backed by a strongly-typed SQLite database.

StructreSheet is _not_ a [database editor](https://sqlitebrowser.org/), rather it is intended to replace spreadsheets such as [MS Excel](https://www.microsoft.com/en-ww/microsoft-365/excel) in applications where users might not [be careful with datatypes](https://news.ycombinator.com/item?id=30986329). For people who are aware of the pitfalls of MS Excel and meticulous about configuring it properly, StructreSheet provides no additional benefits.


# Feature Roadmap

I like KSP's naming scheme.

## 0.1 "Hello, world!"

* Supports single tab - That's a single table with an arbitrary name "tab1" not exposed to the user.
* Display table contents
* Create INT columns with names
* Create new rows, from blank pseudo-row

## 0.2 "Prototypically unready"

* Add TEXT and VARCHAR columns
* Edit cell
* Delete row

## 0.3 "Fill in the blanks"

* Add remaining column types
* Drag selection, cut/copy, paste to self

## 0.4 "Useful Idiot"

* Sort
* Filter

## 0.5 "Making Friends"

* Excel Export. No import! This is a deliberate feature for now, to be reconsidered after the 1.0 release.
* CSV import and export. The simpler CSV format can help ensure that there is no dataloss at the input stage, it is up to the user to ensure that the CSV contains all the data they wish to import.

## 0.6 "Dogfood"

* Column type "Richtext" with configurable parsing rules: Markdown, HTML, etc. Markdown is the default. Backed by TEXT, useful for e.g. a Notes column.
* Foreign keys
* Raw SQL queries
* Spell Check

## 0.7 "Pivot"

* Pivot

## 0.8 "Formulae"

* Support basic formulae, must be explicitely enabled on the cell. SUM, COUNT, IF (-then)

## 0.9 "Share"

* Executable export. Export a database with the entire program to run it.
* Plots

## 1.0 "Collaborate"

* Import and sync databases
* More formulae


## After 1.0 release

* Consider Excel import
* Drag selection, cut/copy, paste to [plain text,Excel,etc.]
* Python script support
* Plugins



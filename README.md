<!-- vim:se noet lbr tw=72 sts=0 sw=4 ts=4 wrap:
--*- fill-column: 72; truncate-lines: nil; word-wrap: t; -*-->

Syntax highlighting for delimiter-separated value formats
========================================================================

This package adds syntax highlighting for three _de facto_ standards for
representing tabulated data as plain-text databases compatible with most
spreadsheet software:

* [x] [Comma-separated values][CSV]     (`*.csv`)
* [x] [Tab-separated values][TSV]       (`*.tsv`, `*.tab`)
* [ ] [Delimiter-separated values][DSV] (`*.dsv`)

The ambiguously-named latter format is intended to represent any tabular
data that uses a punctuation or control character to delimit its fields.

Limitations
------------------------------------------------------------------------
Because the grammars have no way to distinguish data with column headers
or determine if non-standard escape characters should be supported, this
package avoids making unreasonable assumptions about the author's intent
(other than expecting the first row of tabular data to contain the names
of each field).


<!-- Referenced Links ------------------------------------------------->
[CSV]: https://en.wikipedia.org/wiki/Comma-separated_values
[DSV]: https://en.wikipedia.org/wiki/Delimiter-separated_values
[TSV]: https://en.wikipedia.org/wiki/Tab-separated_values

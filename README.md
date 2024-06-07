# flagsubstr

Concatenate the emoji flags for countries AB and CD and the 4:12-byte substring
is the emoji flag for country BC:

```go
// GOEXPERIMENT=rangefunc go run github.com/icio/flagsubstr@latest | head
"🇦🇨🇦🇨"[4:12] == "🇨🇦" // AC: Ascension Island + AC: Ascension Island == CA: Canada
"🇦🇨🇦🇩"[4:12] == "🇨🇦" // AC: Ascension Island + AD: Andorra == CA: Canada
"🇦🇨🇦🇪"[4:12] == "🇨🇦" // AC: Ascension Island + AE: United Arab Emirates == CA: Canada
"🇦🇨🇦🇫"[4:12] == "🇨🇦" // AC: Ascension Island + AF: Afghanistan == CA: Canada
"🇦🇨🇦🇬"[4:12] == "🇨🇦" // AC: Ascension Island + AG: Antigua & Barbuda == CA: Canada
"🇦🇨🇦🇮"[4:12] == "🇨🇦" // AC: Ascension Island + AI: Anguilla == CA: Canada
"🇦🇨🇦🇱"[4:12] == "🇨🇦" // AC: Ascension Island + AL: Albania == CA: Canada
"🇦🇨🇦🇲"[4:12] == "🇨🇦" // AC: Ascension Island + AM: Armenia == CA: Canada
"🇦🇨🇦🇴"[4:12] == "🇨🇦" // AC: Ascension Island + AO: Angola == CA: Canada
"🇦🇨🇦🇶"[4:12] == "🇨🇦" // AC: Ascension Island + AQ: Antarctica == CA: Canada
```

# Protocol Polyglot Lab

I useed the tool [Mitra](https://github.com/corkami/mitra.git) to generate the [Polyglot](ambigous.zip.pdf)

Please follow the [Mitra Install Instriuctions](https://github.com/corkami/mitra.git) to install `mitra`.

## Quickstart

Merge `in-files/archive-hiding-textfile.zip` (top) and `in-files/sample-pdf` (bottom) into a single file, staying **BOTH** valid `PDF` and valid `ZIP` and without chaning the contents.

```sh
mitra.py --verbose -o . ./in-files/archive-hiding-textfile.zip ./in-files/sample.pdf

# $> ls
# S(c3)-Zip-PDF.XXXXXXXXXX.pdf.zip   P(1e-bf2)-Zip[PDF].XXXXXXXXXX.zip.pdf
```

Note that `S(c3)-Zip-PDF.XXXXXXXXXX.pdf.zip` is equivalent `to ambigous_protocol.zip.pdf`

---

## Generating uncompressed zip files (`MacOS`)

Gnerate uncompressed `in-files/archive-hiding-textfile.zip`

```sh
zip -Z store ./in-files/archive-hiding-textfile.zip ./in-files/hide/
```

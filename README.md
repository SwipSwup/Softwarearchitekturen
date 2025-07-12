# Software architectures - RideShare

[Arc42 Template](https://github.com/NetworkedAssets/arc42-in-markdown-template/tree/master/3.%20Flat%20Structure)

**Members:**
Mayer Lukas, Radic Ivo, Sarzi Sartori Nicoletta, Veigel David


## Generate pdf
```
pandoc ./latex/title.md ./arc42/*.md -o architecture.pdf --pdf-engine=xelatex --metadata-file=./latex/metadata.yaml --resource-path=arc42
```
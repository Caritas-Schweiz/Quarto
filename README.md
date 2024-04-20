# Quarto

This projects uses <https://quarto.org/> and <https://code.visualstudio.com/> to create a data visualisation website for Caritas Schweiz.

## Development

Install Quarto according to: <https://quarto.org/docs/get-started/>

In VSCode install these extensions:

* Quarto
* Juypter

Then install python tools:

`pip install -r requirements.txt`

Open the `hello.qmd` file and run the cell.

## Usage

Add `Falldaten_CaritasbB.csv` and `Caritas Markt.csv` to the folder.

Open the `index.qmd` and run the Quarto preview `> Quarto: Preview`.

### Render

To generate the `.html` document (the static website) run `> Quarto: Render Document` and select HTML.

### Deployment

Download the Quarto binary.

```bash
./install.sh
```

Render the documents.

```bash
./build.sh
```

Deploy with [vercel](https://vercel.com/).

```bash
vercel --prod
```
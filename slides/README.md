# Slide della discussione di laurea

Sorgente LaTeX (Beamer) della presentazione. Il PDF compilato è `main.pdf`.

## Compilazione

Serve **LuaLaTeX** (per il font Work Sans, incluso in `fonts/`):

```sh
cd slides
lualatex main.tex
lualatex main.tex   # seconda passata per i numeri di pagina
```

Su Overleaf: caricare l'intera cartella `slides/` e impostare il compilatore su LuaLaTeX.

## Struttura

| File / cartella | Contenuto |
|---|---|
| `main.tex` | tutte le slide |
| `tema.sty` | tema grafico (colori, intestazione, riquadri, macro `\foto` e `\metriche`) |
| `figure/` | grafici MATLAB (in formato vettoriale) e logo |
| `foto/` | foto del laboratorio (da aggiungere) |
| `fonts/` | font Work Sans (licenza OFL, `fonts/OFL.txt`) |

## Da completare

- **Foto:** salvare in `foto/` i file `lab-oscilloscopio.jpg`, `lab-arduino.jpg`, `lab-banco.jpg`.
  Finché mancano, al loro posto compare un riquadro tratteggiato.
- **Grafico sinusoide su Arduino:** la slide "Risultati su Arduino: sinusoide" mostra la curva
  ricostruita dai coefficienti della Tabella 4.2. Per usare il grafico della tesi (riferimento +
  stima Arduino) salvarlo come `figure/arduino_sinusoide.pdf`: viene usato automaticamente.
- **Riferimento bibliografico del BQBE** nella slide "Obiettivo della tesi e contributo"
  (segnato con `TODO` in `main.tex`).
- **Valore di ε:** la slide "Verifica della pipeline in MATLAB" riporta ε = 0.08, la slide di
  riserva R1 ε = 0.008. Controllare quale è corretto.

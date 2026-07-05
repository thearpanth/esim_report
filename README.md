# Designing Integrated Circuits in eSim

**FOSSEE Semester Long Internship Report — Spring 2026**
Submitted by **Aarpan Thapa**, Department of Mechanical Engineering, Thapathali Engineering Institute
Under the guidance of Assistant Prof. Sumanto Kar and Project Research Assistant Varad Vilasrao Patil, IIT Bombay

## About

This repository contains the full LaTeX source, figures, and compiled PDF for a FOSSEE (IIT Bombay) internship
report on modelling digital integrated circuits as reusable subcircuits in [eSim](https://esim.fossee.in/), an
open-source EDA tool. Ten ICs spanning TTL and CMOS logic families were built from datasheet specifications,
simulated in NgSpice, and verified against their published function tables.

### Contributed ICs

| # | Part        | Description                                        |
|---|-------------|-----------------------------------------------------|
| 1 | 74LS93      | 4-Bit Binary Ripple Counter                         |
| 2 | 74LS175     | Quad D-Type Positive-Edge-Triggered Flip-Flop       |
| 3 | 74LS374     | Octal D-Type Edge-Triggered Flip-Flop (3-State)     |
| 4 | CD4024BC    | 7-Stage Ripple-Carry Binary Counter                 |
| 5 | SN74LS244   | Octal Buffer/Line Driver (3-State)                  |
| 6 | SN74S181    | 4-Bit Arithmetic Logic Unit (ALU)                   |
| 7 | SN5470      | AND-Gated Positive-Edge-Triggered J-K Flip-Flop     |
| 8 | 74LS670     | 4-Word × 4-Bit Register File (3-State)              |
| 9 | 74LS173     | 4-Bit D-Type Register (3-State)                     |
| 10| 74LVC157    | Quad 2-Input Multiplexer (Low-Voltage CMOS)         |

Each chapter documents the general description, key features, applications, eSim subcircuit symbol, datasheet
pin diagram, test circuit, function table, and simulated output waveforms, with a direct link to the
manufacturer's datasheet.

## Repository structure

```
.
├── main.tex        # LaTeX source for the full report
├── figs/           # Schematic, symbol, and waveform screenshots exported from eSim
├── report.pdf       # Pre-built PDF (compiled from main.tex)
└── README.md
```

## Building from source

The report is written in standard LaTeX (`report` class) and requires no exotic packages. To build it locally:

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
pdflatex main.tex
pdflatex main.tex   # run twice to resolve the table of contents, citations, and cross-references
```

Or open `main.tex` directly in [Overleaf](https://www.overleaf.com/) — upload the whole repository (or a zip of
it) as a new project.

## License

Report text and figures © Aarpan Thapa. Feel free to open an issue or pull request if you spot an error.

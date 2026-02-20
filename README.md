# CELM Profilprojekt

**Eigentokens: Grammar-Aware Inline Deduplication and Deterministic Compilation for Large Language Models**

## About

This repository contains the scientific documentation and analysis for the profile project (Profilprojekt) at TU Dresden, Chair of Scalable Software Architectures for Data Analytics (Prof. Dr. Michael Faerber).

The project investigates the CELM (Compiled Eigentoken Language Model) architecture and its implementation within the comdare-db database system, developed by BEP Venture UG (brand: Comdare).

## Structure

```
.
├── doku.tex              # Main LaTeX document
├── doku.bib              # Bibliography
├── doku.pdf              # Compiled output (auto-updated by CI)
├── zihpub.cls            # TU Dresden ZIH LaTeX template
├── Makefile              # Build automation
└── presentation/         # Interim presentation slides
```

## Building

### Prerequisites

- TeX Live (full installation recommended)
- pdflatex, bibtex

### Compile

```bash
make
```

Or manually:

```bash
pdflatex doku.tex
bibtex doku
pdflatex doku.tex
pdflatex doku.tex
```

## CI/CD

The GitLab CI pipeline automatically compiles `doku.tex` on every push and commits the resulting `doku.pdf` back to the repository.

## License

This research project is licensed under the Apache License 2.0. See [LICENSE](LICENSE) for details.

The comdare-db database system referenced in this work is a commercial product of BEP Venture UG and is subject to a separate EULA.

## Author

Benjamin-Elias Probst
Matriculation number: 4510512
TU Dresden, Faculty of Computer Science
INF-PM-FPA Profilprojekt Anwendungsforschung in der Informatik

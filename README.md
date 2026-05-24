# CV

This repository contains English and Russian versions of the same CV, written in LaTeX and built
with XeLaTeX.

## PDF versions

- [English CV](cv_en.pdf)
- [Russian CV](cv_ru.pdf)

## Requirements

The CV uses Noto Sans and Noto Sans Mono. The fonts are licensed under the SIL Open Font License
1.1 and are not bundled in this repository.

Required tools and fonts:

- XeLaTeX
- latexmk
- [Noto Sans](https://fonts.google.com/noto/specimen/Noto+Sans)
- [Noto Sans Mono](https://fonts.google.com/noto/specimen/Noto+Sans+Mono)

## Structure

- `cv_en.tex` and `cv_ru.tex` are the public build entrypoints.
- `cv_content_en.tex` and `cv_content_ru.tex` contain language-specific CV content.
- `cv_style.tex` contains the shared preamble, fonts, colors, layout, and macros.
- `cv_template.tex` contains the shared document wrapper.
- `cv_en.pdf` and `cv_ru.pdf` are generated PDF versions committed intentionally for direct access.

## Build

Build with `latexmk`:

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error cv_en.tex cv_ru.tex
```

Clean auxiliary files:

```sh
latexmk -c
```

## License

This repository is licensed under the [0BSD License](LICENSE).

You may use, copy, modify, and distribute the LaTeX template for personal or commercial purposes
without attribution.

The included CV content is real personal example data. If you use this repository as a template,
replace all personal information and generated PDF files with your own.

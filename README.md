# CV

This repository contains English and Russian versions of the same CV.

## Requirements

The CV uses Noto Sans and Noto Sans Mono, licensed under the SIL Open Font License 1.1.
The fonts are not bundled in this repository.

- XeLaTeX
- latexmk
- [Noto Sans](https://fonts.google.com/noto/specimen/Noto+Sans) font
- [Noto Sans Mono](https://fonts.google.com/noto/specimen/Noto+Sans+Mono) font

## Structure

- `cv_en.tex` and `cv_ru.tex` are the public build entrypoints.
- `cv_style.tex` contains the shared preamble, fonts, colors, layout, and macros.
- `cv_template.tex` contains the shared document wrapper.
- `cv_content_en.tex` and `cv_content_ru.tex` contain language-specific CV content.

## Build

Build one version directly:

```sh
xelatex cv_en.tex
xelatex cv_ru.tex
```

Or build both versions with latexmk:

```sh
latexmk -xelatex cv_en.tex cv_ru.tex
```

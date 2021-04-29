IEEEtransSN Spanish customization
=================================

**Warning: Personally, for new projects I would recommend using BibTeX and [BabelBib](https://github.com/TeX-Live/babelbib) and leaving aside the approach offered by this file. I fixed this configuration to be able to work on a project template that uses Polyglossia and had a large number of options configured, so migrating all the configuration would have involved a much greater effort than adjusting this file.**

This repository contains a file which adapts the Michael Shell's [IEEEtransSN](https://www.ctan.org/pkg/ieeetran) BibTeX bibliographic style to the Spanish orthography.

To use this style is necessary:

1. Copy the file `IEEEtranSN_custom_es.bst` to your project.
2. In your main LaTeX file, import the CTAN's `doi` package with:

```tex
\usepackage{doi}
```

3. Then, you can use the style with:

```tex
\bibliographystyle{IEEEtranSN_custom_es}
```

List of fixes of the Spanish adaptation
---------------------------------------

- Use of translated bibliographic tags like "y" instead of "and", "en" instead of "in", etc. Used RAE's (Real Academia Española) official recommended abbreviations [[1]].
- Use of translated month abbreviations. Used Fundéu-RAE's official recommended abbreviations [[2]].
- Use of Latin quotes (`«»`) instead of English ones (`"`).
- Final punctuation symbols are written outside of quotations and not inside: I.e.: "«Bla, bla, bla»." and not "«Bla, bla, bla.»". Here Spanish and English orthographies are different [[3]].
- An approach to write the items DOI, when it was available. It is similar to the used by Zotero app when export citation as IEEE format.

[1]: https://www.rae.es/dpd/ayuda/abreviaturas
[2]: https://www.fundeu.es/escribireninternet/abreviaturas-de-los-meses-y-los-dias-de-la-semana/
[3]: https://www.rae.es/dpd/comillas

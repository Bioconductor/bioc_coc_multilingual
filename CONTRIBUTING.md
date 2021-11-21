# Contributing to the Multilingual Bioconductor Code of Conduct

## New language

- Identify the language code that will be used to name files.
  + Go to <https://www.techonthenet.com/js/language_tags.php>
  + Use the table to identify the language code, e.g. `fr-FR` for "French, France".
  + If you cannot find a suitable language code, open an issue on this repository to discuss options or identify a better reference of language codes.

- Copy the current version of the `en-US.Rmd` file in the root directory of this repository to a new file `xx-XX.Rmd`, replacing `xx-XX` by the language code identified above.

- Edit the new file as needed, following these rules:
  + Maintain a 1-to-1 mapping between original lines and translated lines, i.e. do not split or merge lines between the original files and the translated file.
  + Maintain the styling. Maintain the level of section headers. Do not replace section headers with font styling (e.g., bold, italic).
  + In the title, replace `emo::ji('United_States')` by the emoji for the country of the language.
    * If you cannot find a suitable emoji, open an issue on this repository to discuss options.
  + In the title, the language name should be written in the language itself.

- Update the file `index.Rmd` as needed, following these rules:
  + Insert a row to the new language in alphabetical order (latin alphabet), e.g. Chinese -> English -> French
  + The name and country of the language should be written in English, not the language itself.
  + Make sure that you indicate the correct version of the code of conduct that you have translated.
  + Set the link to `[xx-XX](xx-XX.html)`, replacing `xx-XX` by the language code identified above.

```
| `r emo::ji("United_States")` | English, United States | 1.0.1 | [en-US](en-US.html) |
```

- Update the file `about.Rmd` as needed, following these rules:
  + Add a level 4 section header with the flag of the country, name of the language, and flag of the country.
    * If you cannot find a suitable emoji for the flag, open an issue on this repository to discuss options.
  + The name and country of the language should be written in English, not the language itself.
  + One author should be prefix with `**Maintainer:**` and associated with a hyperlink that may be used to contact them.

```
#### `r emo::ji("United_States")` English, United States

- [BioC 2020 Organizing committee](https://bioc2020.bioconductor.org/organizers)
- **Maintainer:** [Bioconductor Code of Conduct Committee](https://www.bioconductor.org/about/code-of-conduct/)
```

For instance:

```
      - text: "English, United States"
        href: en-US.html
```

- Update the file `_site.yml` as needed, following these rules:
  + Insert a link to the new language in alphabetical order (latin alphabet), e.g. Chinese -> English -> French
  + The text of the link should be written in English, not the language itself.
  + The link should point to `xx-XX.html`, replacing `xx-XX` by the language code identified above.

For instance:

```
      - text: "English, United States"
        href: en-US.html
```

If you have any doubt, open an issue on this repository to discuss options.

## Existing language

### Fixes

Fixes comprises edits and suggestions related to a specific version of the code of conduct.
For updates to a newer version of the code of conduct, see below.

- Open an issue or a pull request, tagging the maintainer of the language.

### New version

New versions refer to the process of replacing an earlier translation of the code of conduct by a translation of a more recent version of the code of conduct.

- Open an issue or a pull request, tagging the maintainer of the language.
  + Make sure that the version number for that language has been updated in all relevant places:
    * the file `xx-XX.Rmd`
    * the file `index.Rmd`

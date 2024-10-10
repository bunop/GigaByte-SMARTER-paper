# SMARTER-database: a tool to integrate SNP array datasets for sheep and goat breeds

Source code of the SMARTER-database GigaByte paper

## Convert LaTeX to word document

Install `pandoc` and `pandoc-crossref` in a conda environment, or install using
conda lock:

```bash
conda-lock install --name my-environment conda-lock.yml
```

Activate the environment and run the following command:

```bash
conda activate my-environment
pandoc -s main.tex --filter pandoc-crossref --bibliography=paper-refs.bib \
    -o main.docx --csl oup-contemporary.cls
```

This will be enough to convert almost the LaTeX file to a word document, some
changes may be needed in the final document.(check for figure/table captions)

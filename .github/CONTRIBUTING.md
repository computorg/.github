# Contributing to Computo

Computo ([computo-journal.org](https://computo-journal.org/)) is a diamond open-access journal at the intersection of computational and statistical methods. This repository belongs to the [computorg](https://github.com/computorg) organization; how you contribute depends on what kind of repository you're in.

## Submitting a manuscript

If you're an author preparing a submission:

1. Create your repository from one of the official templates: `template-computo-R`, `template-computo-python`, or `template-computo-julia`.
2. Follow the [author guidelines](https://computo-journal.org/site/guidelines-authors.html): edit the `.qmd` file and the metadata in `_quarto.yml`, freeze dependencies (renv, `environment.yml`, or `Project.toml`), and make sure the CI workflow renders the manuscript successfully.
3. Submit the PDF and a link to your repository on [OpenReview](https://openreview.net/group?id=Computo).

## Reviewing a manuscript

If you've accepted a review invitation, see the [reviewer guidelines](https://computo-journal.org/site/guidelines-reviewers.html). Reviews are conducted on OpenReview and evaluate scope, clarity, correctness, adequacy of evaluation, and reproducibility — reviewers are expected to actually run the authors' code, not just read it.

## Contributing to the tooling

For contributions to the Computo tooling itself (the [Quarto extension](https://github.com/computorg/computo-quarto-extension), submission templates, or automation scripts):

- Open an issue first to discuss non-trivial changes before submitting a pull request.
- Fork the repository and submit a pull request against `main`.
- Make sure `quarto render` succeeds locally before opening the PR.

## Questions

For anything not covered above, contact contact@computo-journal.org.

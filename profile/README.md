<div align="center">

<img src="https://computo-journal.org/assets/img/logo.png" alt="Computo logo" width="120"/>

# Computo

**A diamond open-access journal in statistics and machine learning**
*A journal of the French Statistical Society (SFdS) — ISSN 2824-7795*

[Website](https://computo-journal.org/) · [Articles](https://computo-journal.org/site/publications.html) · [Author guidelines](https://computo-journal.org/site/guidelines-authors.html) · [Reviewer guidelines](https://computo-journal.org/site/guidelines-reviewers.html) · [Mastodon](https://mathstodon.xyz/@computo)

</div>

---

## About

Computo promotes computational and algorithmic contributions in statistics and machine learning that provide insight into which models or methods are most appropriate for a given scientific question. Rather than sticking to classical static publications, Computo leverages literate programming and modern scientific-reporting tools to make every published article **fully reproducible**: code, data, and narrative live together, and readers can re-run the analysis behind the results.

Computo is a diamond open-access journal: free to read, free to publish in, with peer review handled openly through [OpenReview](https://openreview.net/group?id=Computo).

## How the organization is structured

- **[computorg.github.io](https://github.com/computorg/computorg.github.io)** — source of the journal's website ([computo-journal.org](https://computo-journal.org/)), built with Quarto.
- **[computo-quarto-extension](https://github.com/computorg/computo-quarto-extension)** — the Quarto extension defining the Computo article format, used by every submission and by the journal's own build pipeline.
- **Submission templates**, one per supported language, each a GitHub template repository authors can use to start a new submission:
  - [template-computo-R](https://github.com/computorg/template-computo-R)
  - [template-computo-python](https://github.com/computorg/template-computo-python)
  - [template-computo-julia](https://github.com/computorg/template-computo-julia)
- **`published-*` repositories** — one repository per published article (e.g. [published-paper-tsne](https://github.com/computorg/published-paper-tsne)), each containing the reproducible source of that article and its rendered GitHub Pages version.
- **[.github](https://github.com/computorg/.github)** (this repository) — organization-wide defaults: profile README, issue templates, and contribution guidelines shared across all Computo repositories.

## Contributing an article

If you are an author, start from the template matching your language ([R](https://github.com/computorg/template-computo-R), [Python](https://github.com/computorg/template-computo-python), or [Julia](https://github.com/computorg/template-computo-julia)) and follow the [author guidelines](https://computo-journal.org/site/guidelines-authors.html). Reviewers can find the process described in the [reviewer guidelines](https://computo-journal.org/site/guidelines-reviewers.html).

## Contact

- Website: [computo-journal.org](https://computo-journal.org/)
- Email: contact@computo-journal.org
- Mastodon: [@computo@mathstodon.xyz](https://mathstodon.xyz/@computo)
- LinkedIn: [company/computo-sfds](https://www.linkedin.com/company/computo-sfds)

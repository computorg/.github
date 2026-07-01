---
name: Production tracking
about: Checklist for the 3 phases of manuscript production (acceptance, production start-up, final publication)
title: "[Production Issue] "
labels: production
assignees: ""
---

## Phase 1: acceptance [authors + AE]

When the Associate Editor (AE) is satisfied with the author's answers to the reviewers comments, he/she exchanges with authors (via the discussion tool on OpenReview) to confirm that:

- [ ] authors are informed of final acceptance
- [ ] affiliation, author-url, affiliation-url and other metadata are correctly filled in on the author git repository
- [ ] CI/github-action validates the reproducibility of the manuscript

The authors inform the AE upon completion of the tasks required on their side.

## Phase 2: production start-up [AE]

The AE 

- [ ] set status key to "accepted"
- [ ] invites the corresponding author as a member of computorg: https://github.com/orgs/computorg/people
- [ ] asks the corresponding author to transfer the ownership of their repo to computorg: at the bottom of https://github.com/corresp-author/repo-name/settings, click  "Transfer ownership" and choose "computorg" in "Select one of my organizations"
- [ ] renames this repo to `published-yearmonth-first_author_last_name-manuscript_keyword` (year-month in format YYYYMM; use only hyphens, e.g. `published-202407-legrand-wildfires`)
- [ ] checks, assisted by the technical team, that the manuscript is formatted using the latest Computo extension and ensures that CI works 
- [ ] checks that the README.qmd is correctly rendered, with appropriate badges (at the moment, the number of authors is hardcoded ; the rendering of DOI badge is postponed to last phase)
- [ ] makes the review public by creating an issue in the repository with a link to the reviews (OR or PCI), [following this model](https://github.com/computorg/published-202509-boulet-simulator/issues/5), and adds the label "review" to this issue (which will automatically link to the review badge in the HTML version of the paper)
  - also ensure that the reviews and the rebuttal  are indeed "visible for everyone" on OR
- [ ] checks that the reviewers are not opposed to be listed in the reviewers' page and complete this page accordingly
- [ ] makes an Issue asking for final proofreading by the authors (possibly with some minor additional questions), made as a pull-request on Computorg's repository
- [ ] informs the EiC that phase 2 has ended(check that proofread Issue is closed)

## Phase 3: final publication [EiC]

the EiC 

- [ ] sets/checks the metadata: status to "published", license to CC-BY-4.0, repos, doi, google-scholar: true; date: publication date under format MM-DD-YYYY; date-modified: last-modified.
  - [ ] checks for existing arxiv/HAL versions of the paper and links them accordingly ([example](https://github.com/computorg/published-202606-devijver-scb/blob/main/_quarto.yml#L30-L33))
  - [ ] DOI is created with [this script](https://github.com/computorg/tools-automation/blob/main/submit.sh), will hopefully be integrated in the workflow
- [ ] archives the repository on [software heritage](https://archive.softwareheritage.org/save/)
- [ ] creates a release of the firstly published version, tagged v1.0, on GitHub `git tag v1.0 -a -s -m "Publication v1.0"`
- [ ] moves the corresponding author as a an "outside collaborator" of computorg: https://github.com/orgs/computorg/people
- [ ] posts on LinkedIn

# Milestones

This project is built one milestone at a time. Each milestone should be completed in its own pull request so reviewers can check scope, links, examples, and consistency before the next milestone begins.

## Milestone Rules

- Implement exactly one milestone per pull request.
- Keep changes small enough to review carefully.
- Preserve existing links and file paths unless a pull request explicitly migrates them.
- Use GitHub-flavored Markdown for course material and documentation.
- Keep Python examples clean, reproducible, and beginner-friendly.
- Keep notebooks executable from top to bottom.
- Add exercises, quizzes, solutions, examples, or tests when they fit the milestone.
- Update related indexes and README files when adding new course assets.

## Repository Structure Contract

```text
Statistics-Course/
|-- assets/
|   |-- charts/
|   |-- cheatsheets/
|   |-- icons/
|   `-- images/
|-- course/
|-- datasets/
|-- exercises/
|-- notebooks/
|-- projects/
|-- quizzes/
|-- solutions/
|-- README.md
|-- syllabus.md
|-- roadmap.md
`-- requirements.txt
```

New material should extend this structure instead of creating parallel folders.

## Milestone Sequence

| Milestone | Scope | Status |
|---:|---|---|
| 1 | Course governance, repository standards, and milestone process | In progress |
| 2 | Chapter 02: Python for Statistics | Planned |
| 3 | Chapter 01 notebook, exercises, quiz, and solution files | Planned |
| 4 | Chapter 03: NumPy Fundamentals | Planned |
| 5 | Chapter 04: Pandas Fundamentals | Planned |
| 6 | Chapter 05: Data Visualization | Planned |
| 7 | Chapter 06: Exploratory Data Analysis | Planned |
| 8 | Chapters 07-12: Descriptive Statistics | Planned |
| 9 | Chapters 13-18: Probability | Planned |
| 10 | Chapters 19-26: Probability Distributions | Planned |
| 11 | Chapters 27-34: Statistical Inference | Planned |
| 12 | Chapters 35-38: Regression | Planned |
| 13 | Chapters 39-45: Machine Learning Statistics | Planned |
| 14 | Chapters 46-49: Advanced Statistics | Planned |
| 15 | Chapter 50: Capstone Project | Planned |
| 16 | Dataset documentation and data dictionaries | Planned |
| 17 | Notebook execution checks and examples | Planned |
| 18 | Course-wide review, link audit, and 1.0 release polish | Planned |

## Definition of Done

A milestone is complete when:

- New and changed links have been checked.
- Markdown renders cleanly in GitHub.
- Python examples have been run when applicable.
- Notebook outputs are reproducible when notebooks are part of the milestone.
- Related exercises, quizzes, solutions, projects, datasets, or assets are added or explicitly deferred.
- The pull request description explains the milestone scope and verification performed.

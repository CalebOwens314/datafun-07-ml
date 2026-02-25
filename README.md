# datafun-07-ml

[![Docs Deploy](https://github.com/CalebOwens314/datafun-07-ml/actions/workflows/deploy-mkdocs.yml/badge.svg?branch=main)](https://github.com/CalebOwens314/datafun-07-ml/actions/workflows/deploy-mkdocs.yml)
[![CI](https://github.com/CalebOwens314/datafun-07-ml/actions/workflows/ci-basic-mkdocs.yml/badge.svg?branch=main)](https://github.com/CalebOwens314/datafun-07-ml/actions/workflows/ci-basic-mkdocs.yml)
[![Docs](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://github.com/CalebOwens314/datafun-07-ml/)
[![Python](https://img.shields.io/badge/python-3.14-blue?logo=python&logoColor=white)](https://www.python.org/)

> Professional Python project: predictive machine learning (ML) project, implemented using one Jupyter notebook and one .csv data file. (Created from the repository for my own project submission for project 4, which was constructed from Dr. Case's datafun-04-notebooks repository.)

## Notebook Info

Two languages:

- This file is written in **Markdown**, a simple markup language for presenting text.
- Our analytics logic is written in **Python**, a scripting language for implementing logic.

Notebooks (see "owens_ml.ipynb" under the "notebooks" folder) combine Markdown cells for section headings and narrative with Python Code cells for calculations and charts.

---

## Daily Workflow (Working With Python Project Code)

Follow the detailed instructions at:
[**03. Daily Workflow**](https://denisecase.github.io/pro-analytics-02/03-daily-workflow/)

Commands are provided below to:

1. Git pull
2. Run and check the Python files
3. Build and serve docs
4. Save progress with Git add-commit-push
5. Update project files

VS Code should have only this project (datafun-04-notebooks) open.
Use VS Code menu option `Terminal` / `New Terminal` and run the following commands:

```shell
git pull
```

**Please note that in this project, notebooks are the only analysis artifact (there are no scripts to run).**

- Go to the owens_ml.ipynb file (under the "notebooks" folder in this repo) to run the analysis. Start by clicking "Clear All Outputs," then click "Restart," and finally, click "Run All" to see everything.

Run Python checks and tests (as available):

```shell
uv run ruff format .
uv run ruff check . --fix
uv run pytest --cov=src --cov-report=term-missing
```

Build and serve docs (hit **CTRL+c** in the VS Code terminal to quit serving):

```shell
uv run mkdocs build --strict
uv run mkdocs serve
```

While editing project code and docs, repeat the commands above to run files, check them, and rebuild docs as needed.

Save progress frequently (some tools may make changes; you may need to **re-run git `add` and `commit`** to ensure everything gets committed before pushing):

```shell
git add -A
git commit -m "update"
git push -u origin main
```

Additional details and troubleshooting are available in the [Pro-Analytics-02 Documentation](https://denisecase.github.io/pro-analytics-02/).

---

## Resources

- [Pro-Analytics-02](https://denisecase.github.io/pro-analytics-02/) - guide to professional Python
- [ANNOTATIONS.md](./ANNOTATIONS.md) - REQ/WHY/OBS annotations used
- [INSTRUCTORS.md](./INSTRUCTORS.md) - guidance and notes for instructors and maintainers
- [POLICIES.md](./POLICIES.md) - project rules and expectations that apply to all contributors
- [SE_MANIFEST.toml](./SE_MANIFEST.toml) - project intent, scope, and role

## Citation

[CITATION.cff](./CITATION.cff) - TODO: update author and repository fields to reflect your creative work

<!--
WHY: Support correct citation and attribution.
-->

## License

[MIT](./LICENSE)

<!--
WHY: Provide terms of reuse and limits of liability.
You are welcome to copyright your own projects or open source them as you like.
-->

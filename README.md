# Portfolio Template

A starter repo for building and validating a personal portfolio webpage.

<!-- Optional (extension B): add your workflow status badge here -->

## Structure

```
.
├── index.html                     # Your portfolio page (edit this)
├── style.css                      # Stylesheet (customize this)
├── scripts/
│   └── validate.py                # Checks your portfolio meets requirements
├── .htmlhintrc                    # HTMLHint linting rules
├── .github/
│   └── workflows/
│       └── pipeline.yml          # CI pipeline (you create this in Part 2)
└── README.md
```

## Running the validator locally

```bash
python3 scripts/validate.py
```

(on Windows: `python` or `py` instead of `python3`)

The script checks `index.html` against the requirements and prints `[PASS]`
or `[FAIL]` for each.

## CI pipeline

Create `.github/workflows/pipeline.yml` in Part 2 (the folder does not exist yet).
Your pipeline runs `htmlhint` and `scripts/validate.py` on every push and pull
request to `main`, and then deploys the page to GitHub Pages (only on a push to
`main`).

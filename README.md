# Simon Delaigue - CV

Online resume website hosted on GitHub Pages.

## Workflow

- `cv-check.yml`: validates PDF and static files on `main`, `dev`, and PR to `main`.
- `deploy.yml`: publishes to GitHub Pages on push to `main`.
- `release.yml`: creates a GitHub Release on tag `cv-*` and uploads the CV PDF.

## Release Process

1. Update `VERSION` with `cv-x.y.z`.
2. Commit and push to `main` (check/deploy run automatically).
3. Create and push the `cv-x.y.z` tag.
4. Verify the GitHub Release and the attached PDF asset.

## Tag Convention

- Format: `cv-x.y.z` (example: `cv-0.2.1`).
- The tag must exactly match the content of `VERSION`.
- PDF expectation: the exported PDF must contain the exact `VERSION` value as visible text.

[https://cv.simon-delaigue.fr](https://cv.simon-delaigue.fr)

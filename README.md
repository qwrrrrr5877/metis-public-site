# Metis Public Site

This repository contains the sanitized public MkDocs site exported from the
private Metis workspace.

## Publish With GitHub Pages

1. Create a GitHub repository, for example `metis-public-site`.
2. Push this folder as the repository root.
3. In the GitHub repository, open `Settings -> Pages`.
4. Set `Build and deployment -> Source` to `GitHub Actions`.
5. Push to `main` or run the `Deploy Metis Public Site` workflow manually.

The workflow builds the MkDocs site and publishes the generated `site/`
artifact to GitHub Pages.

## Update From Private Workspace

From the private Metis workspace, rerun:

```powershell
& "C:\Users\Pu\.cache\codex-runtimes\codex-primary-runtime\dependencies\python\python.exe" .\Metis\metis_core\publication\export_public_site.py
```

Then review the regenerated files before pushing this public site repository.

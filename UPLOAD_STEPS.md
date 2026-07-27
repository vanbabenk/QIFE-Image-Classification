# Upload Steps for GitHub Web Interface

Use this file as a simple checklist if you do not use Git command line.

## Option A — upload the ZIP contents manually

1. Download and extract the repository package.
2. Open https://github.com/vanbabenk/QIFE-Image-Classification
3. For each top-level file, click `Add file` → `Upload files`.
4. Drag and drop the file.
5. Commit changes.
6. For folders such as `notebooks`, `docs`, `results`, and `configs`, open or create each folder first, then upload the files inside it.

## Option B — easiest method using GitHub Desktop

1. Install GitHub Desktop.
2. Clone `vanbabenk/QIFE-Image-Classification`.
3. Copy all files and folders from this package into the cloned repository folder.
4. In GitHub Desktop, review the changed files.
5. Use commit message: `Prepare QIFE publication repository`.
6. Click `Commit to main`.
7. Click `Push origin`.

## After upload

Open the GitHub repository and check that this structure appears:

```text
notebooks/
docs/
results/
configs/
README.md
requirements.txt
requirements-colab.txt
.gitignore
CITATION.cff
LICENSE
```

Then click the Colab badges in the README and test the notebooks from a clean Colab runtime.

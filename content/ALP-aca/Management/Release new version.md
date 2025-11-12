---
title: Release new version
draft: false
tags:
  - ALPaca
---
## Prepare changelog

Write the new features in a MD file in the folder `changelogs`. Link the changelog in `README.md`
## Change version numbers
- In `pyproject.toml`: This is the version that will be used by PyPi
- In `alp-aca/__init__.py`: This is the version that will be used internally in the library.
- In the badge of `README.md`: this will redirect to the permanent branch.
## Frozen branch
Create a new branch named after the version. Also create a tag and push it. In GitHub, create a new release using the changelog.
## Build and upload
```bash
rm -rf dist
python -m build
twine upload dist/*
```
## Check Zenodo
When the tag is created, a new DOI should be automatically assigned by Zenodo. Check that everything is ok (authors, format of the changelog...)
## ReadTheDocs
??
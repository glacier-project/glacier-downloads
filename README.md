# GLACIER Downloads

Public distribution point for downloadable GLACIER resources.

Source code and project documentation are maintained in their respective
repositories. Downloadable packages are published as GitHub Release assets.

Do not commit ZIP files, PDFs, datasets, binaries, or other distribution
artifacts directly to this repository.

## Downloading resources

Open the repository's **Releases** page.

Each release corresponds to a specific GLACIER resource, tutorial, event,
demo, or distribution.

Examples:

- `fdl-2026` — material prepared for the FDL 2026 PhD School
- `frost-demo-2027` — Frost demonstration package

## Updating an existing download

### GitHub website

1. Open **Releases**.
2. Open the relevant release.
3. Choose **Edit**.
4. Replace the downloadable asset.
5. Keep the same filename if a public web page already links to it.
6. Save the release.

### Command line

```bash
gh release upload <release-tag> <file> \
  --clobber \
  --repo glacier-project/glacier-downloads
```

Example:

```bash
gh release upload fdl-2026 \
  fdl2026-glacier-student.zip \
  --clobber \
  --repo glacier-project/glacier-downloads
```

## Adding a new resource

Create a new GitHub Release with a descriptive tag, for example:

- `fdl-2026`
- `summer-school-2027`
- `frost-demo-2027`

Upload the files as release assets, then link the required asset from the
appropriate page on the GLACIER website.

## Rule of thumb

- `glacier-website`: explains what a resource is and how to use it.
- `glacier-downloads`: distributes downloadable files.
- project repositories: contain source code and authoring material.

# Test Design — Homework Upload

## Equivalence Partitioning

### File formats
Valid class:
- PDF
- DOCX
- JPG
- PNG

Invalid class:
- EXE
- ZIP
- MP4
- unsupported extension

Representative tests:
- PDF as valid representative
- EXE as invalid representative

## Boundary Value Analysis

### File count
Requirement: maximum 5 files.

Boundary tests:
- 4 — valid
- 5 — valid
- 6 — invalid

### File size
Requirement: maximum 10 MB.

Boundary tests:
- 9.9 MB — valid
- 10 MB — boundary
- 10.1 MB — invalid

## Error Guessing

- filename contains spaces
- filename contains Cyrillic
- filename contains emoji
- duplicate file upload
- corrupted file
- upload while network becomes offline
- double-click Submit
- refresh during upload

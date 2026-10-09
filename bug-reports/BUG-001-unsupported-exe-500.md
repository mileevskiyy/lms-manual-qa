# BUG-001 — Server returns 500 for unsupported EXE upload

**Environment:** Staging, Chrome, macOS  
**Severity:** Major  
**Reproducibility:** 5/5

## Preconditions
Student is logged in and homework is available.

## Steps
1. Open homework.
2. Click Attach File.
3. Select an `.exe` file.
4. Wait for upload result.

## Expected Result
Unsupported file is rejected with a clear validation message.

## Actual Result
Generic error is shown. Network request returns `500 Internal Server Error`.

## Technical Details
`POST /api/homework/attachments`  
Status: `500`

## Attachments
- Network screenshot
- Screen recording

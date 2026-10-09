# Homework Submission Test Cases

| ID | Title | Preconditions | Steps | Expected Result |
|---|---|---|---|---|
| TC-001 | Submit text-only homework | Student logged in; homework available | Open homework → enter text → Submit | Status becomes Submitted; timestamp shown |
| TC-002 | Submit PDF attachment | Student logged in | Attach valid PDF → Submit | Submission succeeds |
| TC-003 | Submit without text and files | Student logged in | Leave all fields empty → Submit | Submission blocked; validation shown |
| TC-004 | Attach exactly 5 files | Student logged in | Attach 5 supported files | All 5 files accepted |
| TC-005 | Attach 6 files | Student logged in | Attach 6 supported files | 6th file rejected or clear validation shown |
| TC-006 | Attach exactly 10 MB file | Student logged in | Attach supported 10 MB file | File accepted if boundary is inclusive |
| TC-007 | Attach file larger than 10 MB | Student logged in | Attach 10.1 MB file | File rejected with clear message |
| TC-008 | Attach unsupported EXE file | Student logged in | Attach EXE file | File rejected; no server 500 |
| TC-009 | Edit submission before grading | Existing submitted homework; not graded | Edit text → Save | Updated content persists |
| TC-010 | Edit after grading | Homework graded | Try to edit text/file | Editing unavailable |
| TC-011 | Double-click Submit | Valid homework data | Double-click Submit quickly | Only one submission is created |
| TC-012 | Refresh after successful submission | Homework submitted | Refresh page | Submitted state persists |

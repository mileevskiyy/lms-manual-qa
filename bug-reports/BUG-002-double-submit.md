# BUG-002 — Double click creates duplicate homework submission

**Environment:** Staging, Chrome, macOS  
**Severity:** Major  
**Reproducibility:** 4/5

## Steps
1. Open homework.
2. Enter a valid answer.
3. Double-click `Submit` quickly.
4. Open teacher view.

## Expected Result
Only one submission is created.

## Actual Result
Two submissions are created for the same student and homework.

## Notes
Two POST requests are visible in DevTools Network immediately after the double click.

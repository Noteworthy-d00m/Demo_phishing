# PayBuddy cyber awareness demo

Static fictional banking simulation. **Use invented usernames and passwords only.**

## Behavior
- First login attempt deliberately shows an incorrect-password error.
- Second attempt opens `account.html` showing John Doe, €67 balance and €1,000 debt.
- `check.html` displays demo attempts and entered demo passwords **only in the same browser**, using localStorage. Nothing is uploaded or shared between devices.
- Logout resets the per-tab attempt counter.

## GitHub Pages
Create a repository, upload `index.html`, `account.html`, `check.html`, and enable **Settings > Pages > Deploy from a branch > main / root**. Visit the published URL. The activity page is at `check.html` (GitHub Pages does not automatically rewrite `/check` to `check.html`).

## Important limitation
GitHub Pages is static. Attendees on other devices will have separate logs, and the presenter's `/check` page cannot see their entries. A shared live event dashboard requires a backend and should not store or expose passwords. The supplied version intentionally does not collect credentials from other devices.

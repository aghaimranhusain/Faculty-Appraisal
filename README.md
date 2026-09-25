# Faculty Performance Appraisal (Teaching Faculty)

A browser-based appraisal form for teaching faculty. Faculty fill category-wise claims, attach PDF/image proofs, see auto-capped scores, and either:

1. **Download a ZIP package** (JSON data + all evidence files) and email it to the HOD/admin, or  
2. **Submit online** via [Web3Forms](https://web3forms.com) (free) so attachments arrive in your inbox.

Works on **GitHub Pages** with no server of your own.

## Categories & caps (total 100)

| Category | Cap |
|----------|-----|
| A. Teaching & learning | 30 |
| B. Student feedback & outcomes | 15 |
| C. Research, publications & innovation | 25 |
| D. Departmental & institutional service | 15 |
| E. Professional development & community | 15 |

## Deploy on GitHub Pages

1. Create a new repository (e.g. `faculty-appraisal`).
2. Upload the contents of this folder (`index.html` and this `README.md`) to the repo root, **or** put them in a `docs/` folder.
3. In the repo: **Settings → Pages → Source**: Deploy from branch `main` (root or `/docs`).
4. After a minute, your link will be:  
   `https://<your-username>.github.io/<repo-name>/`
5. Share that link with faculty.

## One-time admin setup (optional online submit)

1. Go to [https://web3forms.com](https://web3forms.com) and create a free access key (tied to your email).
2. Open the live form page.
3. In the yellow **Admin setup** box at the top, paste the access key and your notification email.
4. The key is stored only in that browser’s localStorage (for convenience). For a permanent setup, edit `index.html` and set a default value on the `#web3key` input, or keep using ZIP packages only.

Faculty never need accounts. Submissions land in the email you registered with Web3Forms (with JSON body + file attachments).

## How faculty use it

1. Open the shared link.
2. Fill particulars and each category; attach proofs (PDF / JPG / PNG).
3. Scores update automatically; category caps are applied.
4. Tick the declaration.
5. Either **Download submission package (ZIP)** and email it, or **Submit online** if the key is configured.

## How you validate later

- **ZIP path:** Open `appraisal_data.json` for scores and claims; open the `evidence/` folder for proofs. Mark verified scores offline (e.g. on the Word form) or in a spreadsheet.
- **Online path:** Check your Web3Forms / inbox for the message and attachments. Same JSON structure.

## Customise

- Change institution name: edit the text inside `#institutionName` in `index.html`.
- Adjust point hints or items: edit the arrays `A2_ITEMS`, `B_ITEMS`, `C_ITEMS`, `D_ITEMS`, `E_ITEMS` in the script section.
- Change caps: edit the `CAPS` object.

## Privacy

Data stays in the faculty member’s browser until they download the ZIP or submit via Web3Forms. Drafts saved with “Save draft” use `localStorage` on that device only (files are not stored in drafts — they must re-attach proofs).

## Files

- `index.html` — single-page form (CSS + JS included)
- `README.md` — this guide

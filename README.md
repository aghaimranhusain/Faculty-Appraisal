# Manav Rachna — Faculty Performance Appraisal Proforma (Form 1594)

Browser-based self-appraisal form aligned with **Manav Rachna Form No. 1594**. Faculty fill particulars, claim scores under Categories I–IV, attach PDF/image proofs, and either download a ZIP package or submit online.

## Score structure (total 700)

| Category | Details | Max |
|----------|---------|-----|
| **I** | Teaching, learning & evaluation related activities | 200 |
| **II** | Research and innovation | 300 |
| **III** | Co-curricular, extension & professional development | 100 |
| **IV** | Institutional commitments / society / admissions / CDC / CRC & general attributes | 100 |
| | **TOTAL** | **700** |

Performance bands (from the official summary):
- **< 40%** → No increment or incentive
- **40–65%** → One increment
- **> 65%** → Two increments and/or incentive

## What is included

- Employee particulars (1–8) including leave table
- Additional qualification (9) & FDP / refresher courses (10)
- Five most significant publications (11) & other professional info (12)
- Future plans (17) & declaration
- **Category I** — lectures %, innovation ratings (Outstanding→Modest), student feedback, continuous assessment, ICT, effective teaching, results analysis
- **Category II** — papers (Q1–Q4), books, ICT courses, PhD/PG guidance, projects, consultancy, IPR, policy docs, fellowships, invited talks, labs, awards
- **Category III** — FDP, MOOCs, co-curricular, committees, organising events, immersions, administrative roles
- **Category IV** — placement/industry/alumni, community, admissions, general attributes
- Auto **category caps** and live performance %
- File upload (PDF / JPG / PNG) per claim
- **Download ZIP** (JSON + evidence folder) or **Submit online** via Web3Forms

## Deploy on GitHub Pages

1. Create a repository (e.g. `faculty-appraisal`).
2. Upload `index.html` and this `README.md` to the root.
3. **Settings → Pages → Source**: branch `main`, folder `/ (root)`.
4. Share: `https://<username>.github.io/faculty-appraisal/`

## Admin setup (optional online submit)

1. Create a free access key at [web3forms.com](https://web3forms.com).
2. On the live form, paste the key in the yellow **Admin setup** box.
3. Submissions (JSON + attachments) arrive at the email registered with Web3Forms.

Faculty never need accounts. Without a key, they use **Download submission package** and email the ZIP to HOD/admin.

## Validation workflow

1. Faculty submits ZIP or online form.
2. Open `appraisal_data.json` for claimed scores and notes.
3. Check files in `evidence/` against each claim.
4. Enter verified scores offline (or on the paper Form 1594) and route to Reporting Officer → Reviewing Officer → Dean → VC as per university guidelines.

## Guidelines (from Form page 12)

- Assessment period: **1 July – 30 June**; submit to HoD by **15 June**.
- Documentary proof required for every claim; write **NIL** where there is no claim.
- Multi-author credit, committee involvement %, and administrative role % follow the printed guidelines.

## Customise

Edit `index.html` script arrays `CAT_I_RATED`, `CAT_II`, `CAT_III`, `CAT_IV` or the `CAPS` object if your school adjusts sub-items. Branding text is in the hero section.

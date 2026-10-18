# ICPC Calculator

A web tool for the **ICPC India 2026 – Amritapuri** site. Find your team's rank or seat number in the rank list, then see who gets selected once the per-institution caps are applied.

🔗 **Live site:** [icpc-calculator.vercel.app](https://icpc-calculator.vercel.app/)

> **Note:** This calculator is for Amritapuri only. Ranks and seat numbers may change, and some teams may not appear in the loaded rank list.

---

## Table of Contents

- [Features](#features)
- [Selection Rules](#selection-rules)
- [How to Use](#how-to-use)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Running Locally](#running-locally)
- [Deployment](#deployment)
- [Disclaimer](#disclaimer)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **Built-in rank list:** works out of the box with the ICPC India 2026 Amritapuri rank list.
- **Upload your own list:** drop or choose a saved `.html` page or a `.csv` file. The end range is automatically set to the last rank in the file.
- **Search by rank or team name:** locate any team and check its seat number and selection status.
- **Adjustable caps:** change the `X` (ranks 51–100) and `Y` (ranks 101–140) per-institution limits and see the selection update.

---

## Selection Rules

| Rank range | Rule |
|------------|------|
| 1 – 50 | All teams selected, with **no limit** per institution. |
| 51 – 100 | Up to **X** teams in total per institution, counting those already selected. |
| 101 – 140 | Up to **Y** teams in total per institution, counting those already selected. |
| 141 onward | **One team per institution per pass**, starting with institutions that have nobody selected, until the **360 general slots** are full. |

---

## How to Use

1. Open the [live site](https://icpc-calculator.vercel.app/).
2. (Optional) Upload your own rank list as `.html` or `.csv`.
3. Set the values of **X** and **Y**.
4. Search by **rank** or **team name**.
5. Check whether your team is selected under the institution caps.

| Rank list format | How to provide it |
|------------------|-------------------|
| `.html` | Save the official rank list page and upload the file. |
| `.csv` | Upload a CSV export of the rank list. |

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Hosting / Deployment | [Vercel](https://vercel.com/) |
| Frontend framework | _[fill in: e.g. React / Next.js / Vite / plain HTML-CSS-JS]_ |
| Language | _[fill in: e.g. JavaScript / TypeScript]_ |
| Styling | _[fill in: e.g. Tailwind CSS / CSS Modules / plain CSS]_ |
| Rank list parsing | Supports `.html` and `.csv` uploads _[fill in: library used, e.g. PapaParse, DOMParser]_ |
| Package manager | _[fill in: npm / yarn / pnpm]_ |
| Version control | Git + GitHub _[fill in repo link]_ |

---

## Project Structure

```
_[paste the output of `tree -L 2 -I node_modules` here]_
```

---

## Running Locally

```bash
git clone <your-repo-url>
cd icpc-calculator

# install dependencies and start the dev server
# (replace with the commands from your package.json)
npm install
npm run dev
```

Then open the local URL printed in the terminal.

---

## Deployment

The app is deployed on **Vercel**. Every push to the connected GitHub branch triggers a new deployment.

To deploy your own copy:

1. Push the repository to GitHub.
2. Import it in the [Vercel dashboard](https://vercel.com/new).
3. Vercel detects the framework, runs the build, and publishes the site.

---

## Disclaimer

This is an unofficial tool built for convenience. Results depend on the rank list loaded and the selection rules above. Always refer to official ICPC India announcements for final results.

---

## Contributing

Issues and pull requests are welcome. If you find a wrong rank, a missing team, or a rule change, please open an issue.

## License

_[add a license, e.g. MIT]_

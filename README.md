# ICPC-claculator
ICPC Calculator

A web tool for the ICPC India 2026 – Amritapuri site. Find your team's rank or seat number in the rank list, then see who gets selected once the per-institution caps are applied.

🔗 Live site: icpc-calculator.vercel.app

Note: This calculator is for Amritapuri only. Ranks and seat numbers may change, and some teams may not appear in the loaded rank list.

Table of Contents
Features
Selection Rules
How to Use
Tech Stack
Project Structure
Running Locally
Deployment
Disclaimer
Contributing
License
Features
Built-in rank list: works out of the box with the ICPC India 2026 Amritapuri rank list.
Upload your own list: drop or choose a saved .html page or a .csv file. The end range is automatically set to the last rank in the file.
Search by rank or team name: locate any team and check its seat number and selection status.
Adjustable caps: change the X (ranks 51–100) and Y (ranks 101–140) per-institution limits and see the selection update.
Selection Rules
Rank range	Rule
1 – 50	All teams selected, with no limit per institution.
51 – 100	Up to X teams in total per institution, counting those already selected.
101 – 140	Up to Y teams in total per institution, counting those already selected.
141 onward	One team per institution per pass, starting with institutions that have nobody selected, until the 360 general slots are full.
How to Use
Open the live site.
(Optional) Upload your own rank list as .html or .csv.
Set the values of X and Y.
Search by rank or team name.
Check whether your team is selected under the institution caps.
Rank list format	How to provide it
.html	Save the official rank list page and upload the file.
.csv	Upload a CSV export of the rank list.
Tech Stack
Layer	Technology
Hosting / Deployment	Vercel
Frontend framework	[fill in: e.g. React / Next.js / Vite / plain HTML-CSS-JS]
Language	[fill in: e.g. JavaScript / TypeScript]
Styling	[fill in: e.g. Tailwind CSS / CSS Modules / plain CSS]
Rank list parsing	Supports .html and .csv uploads [fill in: library used, e.g. PapaParse, DOMParser]
Package manager	[fill in: npm / yarn / pnpm]
Version control	Git + GitHub [fill in repo link]
Project Structure
_[paste the output of `tree -L 2 -I node_modules` here]_
Running Locally
bash
git clone <your-repo-url>
cd icpc-calculator

# install dependencies and start the dev server
# (replace with the commands from your package.json)
npm install
npm run dev

Then open the local URL printed in the terminal.

Deployment

The app is deployed on Vercel. Every push to the connected GitHub branch triggers a new deployment.

To deploy your own copy:

Push the repository to GitHub.
Import it in the Vercel dashboard.
Vercel detects the framework, runs the build, and publishes the site.
Disclaimer

This is an unofficial tool built for convenience. Results depend on the rank list loaded and the selection rules above. Always refer to official ICPC India announcements for final results.

Contributing

Issues and pull requests are welcome. If you find a wrong rank, a missing team, or a rule change, please open an issue.

License

[add a license, e.g. MIT]

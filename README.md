# Cost Benefit Analysis — Decision Lab

A responsive, self-contained calculator for product investment decisions. No dependencies, build step, API key, or backend required.

## Run locally

Open `index.html` in a web browser.

## Upload and publish with GitHub Pages

1. Extract this ZIP on your computer.
2. Create a GitHub repository (for example, `cost-benefit-analysis`).
3. Upload the extracted files into the repository root. Make sure `index.html` is at the root, rather than inside an extra folder. Upload the extracted files, not the ZIP.
4. Commit the files to your default branch, typically `main`.
5. In repository Settings, open Pages. Choose deployment from a branch, select your default branch and the root folder, then save.
6. Wait for deployment and open the website URL shown by GitHub Pages.

GitHub Pages documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Features

- One-time development costs and monthly operational costs.
- Monthly retained-revenue contribution, cost savings, and new-revenue contribution.
- Total cost, net benefits, benefit-cost ratio, and fractional-month payback.
- Conservative, base, and optimistic benefit scenarios.
- Cumulative cash-flow chart and period breakdown.
- Currency display selector, CSV export, and print report.

## Model assumptions

All prefilled amounts are illustrative. Development costs occur at month 0. Operational costs and benefits are constant from month 1. Scenario factors scale benefits only. Use contribution after variable delivery costs for revenue benefits and avoid double counting savings. Currency selection relabels values without conversion. The model is undiscounted and excludes taxes, inflation, growth, financing, and launch delays.

Total cost = development + monthly operations × horizon.
Total benefits = monthly benefits × scenario factor × horizon.
Net benefits = total benefits − total cost.
BCR = total benefits / total cost; undefined when total cost is zero.
Payback = development / (realized monthly benefits − monthly operations), when positive monthly net cash flow can recover the investment. Zero upfront cost means no investment to recover.

Inputs are processed in your browser. Entries are not saved after refreshing; export a CSV to retain assumptions and results.

## Verification

JavaScript syntax and default-case arithmetic checked: 36 months, INR 2,640,000 total cost, INR 1,680,000 net benefits, 1.63636 BCR, and 15-month payback. Browser-level verification remains pending.

## LegalEase context
This edition uses the LegalEase AI summarizer idea shared in the conversation. The image-based source PDF could not be extracted; no financial figures are claimed as document-derived. All example values are editable planning assumptions. Retained and new revenue use contribution after variable costs. Customer time savings are separate from LegalEase operating savings.

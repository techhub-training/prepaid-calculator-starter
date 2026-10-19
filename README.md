# Build a Prepaid Amortization Calculator with an AI Assistant

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/techhub-training/prepaid-calculator-starter?quickstart=1)

A TechHub.training challenge. Ridgeline Home & Tool (fictional) pays some costs in advance and expenses them
month by month. The accounting team wants a small web page that turns a prepaid into its monthly schedule.
Build it with an AI assistant, publish it with GitHub Pages, and use it to answer the TechHub checker.

## 1. Get your own copy

Click **Use this template › Create a new repository** (top right of this page). Owner: you. Name: `prepaid-calculator`.
Make it **Public** (GitHub Pages needs that on a free account).

## 2. Open it somewhere you can work

* **No installs:** on *your* repository, click **Code › Codespaces › Create codespace on main**. A preview of
  `index.html` opens by itself; refresh it after each change. GitHub gives every account free Codespaces hours each month.
* **On your computer:** `gh repo clone <your-username>/prepaid-calculator`, edit with any editor, and double-click
  `index.html` to view it.

## 3. Build it with your AI assistant

`SPEC.md` has the rules. Give them to your assistant (Copilot in Codespaces, ChatGPT, Claude, Gemini…), ask it to
replace `index.html`, and **check its numbers against the test case in SPEC.md**. AI assistants often get the
rounding and the year rollover wrong.

Then `git add`, `git commit` and `git push` (Codespaces: the *Source Control* panel does the same).

## 4. Publish it

On your repository: **Settings › Pages › Build and deployment › Source: Deploy from a branch › Branch: main, / (root) › Save**.
After a minute your calculator is live at `https://<your-username>.github.io/prepaid-calculator/`.

## 5. Answer the checker

Use your published calculator on the test case in SPEC.md, download the CSV, and upload it to the TechHub checker.

## Never commit keys

This app needs no API key. If a project ever does, keep the key out of Git: put it in a `.env` file
(already in `.gitignore`) or in **Settings › Secrets and variables › Codespaces**. Anything you push to a public
repository can be read by anyone, forever.

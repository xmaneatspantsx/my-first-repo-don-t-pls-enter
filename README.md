# Nautilus Cloud — DSi compatibility test

This is the first, static compatibility test for the Nautilus Cloud project.

## Important
- This is **not** the finished file manager.
- It has no login system, accounts, uploads, downloads, or storage.
- Do not enter real passwords or private information on this page.
- The purpose is to test whether the Nintendo DSi Browser can load the chosen hosting provider over HTTPS and display basic HTML/CSS/JavaScript.

## Deploy using Cloudflare Pages and a private GitHub repository

1. Create a **private** GitHub repository named `nautilus-cloud`.
2. Extract this ZIP.
3. Upload `index.html` to the repository root using GitHub's website.
4. In Cloudflare, open Workers & Pages and create a Pages project.
5. Connect your GitHub account and select the private `nautilus-cloud` repository.
6. For a plain HTML project, leave the build command empty and set the output directory to `/` if the setup screen permits it. If the dashboard requires a directory name, use the repository root setting offered by the current Pages flow.
7. Deploy and open the generated `*.pages.dev` address on the DSi.

## Report the result
Record whether:
- The page opens without a certificate/TLS error.
- The dark styling appears.
- The JavaScript test displays the browser time.
- The form test works.
- The page remains usable on the DSi's small screen.

Do not add private files, passwords, API tokens, or encryption keys to this repository.

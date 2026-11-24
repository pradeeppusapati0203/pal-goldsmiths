P.A.L GOLDSMITHS WEBSITE — READY TO UPLOAD

CONTENTS
- index.html: complete mobile-friendly website and live market-rate fetch
- assets/pal-logo.jpg: the supplied P.A.L logo
- manifest.webmanifest and sw.js: installable/offline website shell

IMPORTANT ABOUT GOLD RATES
The website requests the India API bullion endpoint at:
https://api.dharun.dev/v1/bullion
Its documentation says the rates are IBJA benchmark rates, checked periodically, before GST and making charges. They are market reference rates, NOT a local Chilakaluripet retail quote. Upstream API availability, response structure, CORS policy and rate limits are outside this website's control. If the API changes or blocks browser requests, the site displays an unavailable message rather than inventing a price.

PUBLISH USING GITHUB PAGES (ANDROID PHONE)
1. Open https://github.com/signup and create/verify a GitHub account.
2. Sign in and tap +, then New repository.
3. Name it: pal-goldsmiths
4. Choose Public, enable Add a README file, then Create repository.
5. Open the repository's Code tab. Use Add file > Upload files.
6. Upload index.html, manifest.webmanifest, sw.js, README.txt, and the assets folder containing pal-logo.jpg. If mobile upload does not preserve folders, create an assets folder in GitHub first and upload pal-logo.jpg inside it.
7. Commit the uploaded files to the main branch.
8. Open Settings > Pages.
9. Under Build and deployment, choose Deploy from a branch.
10. Select Branch: main and Folder: /(root), then Save.
11. Wait for the deployment. In Settings > Pages, tap Visit site.
12. Your public link will be https://YOUR-GITHUB-USERNAME.github.io/pal-goldsmiths/

TROUBLESHOOTING
- If the logo is missing, confirm its exact path is assets/pal-logo.jpg.
- If rates show unavailable, test the endpoint in a browser: https://api.dharun.dev/v1/bullion?utm_medium=pal-goldsmiths . The API may be temporarily unavailable or may change its schema/CORS behavior. Do not manually substitute guessed prices.
- Changes may take several minutes to publish.
- GitHub Pages is static hosting; this package does not contain a private server or guarantee live-data uptime.

BEST OF SHARK TANK — WEBSITE UPLOAD PACKAGE

1. Unzip this package.
2. Create a GitHub repository named bestofsharktank (private or public).
3. Upload the dist folder and this README.txt into the repository.
   The repository must contain dist/index.html, dist/style.css,
   dist/app.js, and dist/assets/.
4. In Cloudflare, open Workers & Pages and create a Pages project.
   Select Import an existing Git repository and connect this repository.
5. Build settings:
   Production branch: main
   Framework preset: None
   Build command: exit 0
   Build output directory: dist
6. Deploy. Test the temporary pages.dev address Cloudflare provides.
7. Add bestofsharktank.com through the project's Custom domains settings.
   For this root domain, Cloudflare requires the domain to use Cloudflare
   nameservers. Add the domain to Cloudflare and follow its instructions
   at the company where you bought your domain. Keep the domain registered
   there; a registrar transfer is not required.
8. Add www.bestofsharktank.com as another custom domain if desired.

Every later update committed to main will deploy automatically.
The ZIP itself should not be uploaded into GitHub; upload its contents.

Official setup guides:
https://developers.cloudflare.com/pages/get-started/git-integration/
https://developers.cloudflare.com/pages/configuration/custom-domains/

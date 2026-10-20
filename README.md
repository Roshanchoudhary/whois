# Whois Tools

A fast, responsive, multilingual domain and internet toolkit designed for Cloudflare Pages.

## Features
- Domain registration lookup via public RDAP
- DNS record lookup (A, AAAA, MX, TXT, NS and CNAME) via Cloudflare DNS over HTTPS
- Public IP lookup via ipwho.is
- English, Hindi and Spanish interface
- Responsive design, FAQ content, metadata, structured data, robots.txt and XML sitemap
- Static deployment: no framework, build command, or package installation required

## Deploy on Cloudflare Pages
1. Open Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages**.
2. Connect the `Roshanchoudhary/whois` GitHub repository.
3. Choose the `main` branch.
4. Select **Framework preset: None**.
5. Leave the build command blank. Set the build output directory to `/` (or `.` if the dashboard asks for a relative path).
6. Save and deploy. Future commits to `main` can trigger automatic deployments.

## Before launch
- Confirm the actual Pages hostname or connect your custom domain. The SEO canonical and sitemap currently use `https://whois.pages.dev/`; update these if your actual hostname differs.
- Test the three lookup tools in production. Public providers may rate-limit requests, and their availability can change.
- Verify the site and submit the sitemap in Google Search Console.
- Add substantial, original tool-specific guides and translated content pages before expanding SEO. Language toggles alone do not create separate indexable pages or guarantee rankings.

## Data and privacy
Lookup queries send the entered domain or IP to the selected public data provider. Registration details can be redacted and geographic IP estimates may be approximate. This project is not affiliated with ICANN or any registrar.

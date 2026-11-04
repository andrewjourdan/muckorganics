# Muck Organics

Website: https://muckorganics.com/

## Local preview

This is a static website with no package installation or build step.
Run `python3 -m http.server 8000` from the repository root, then open
http://localhost:8000/. Stop the preview with Ctrl+C.

## Validation

Run `python3 scripts/check_site.py` with Python 3.12 or newer. It checks the
homepage metadata, local links and files, JSON-LD syntax, CNAME, sitemap and
robots.txt. GitHub Actions runs these checks on pull requests and pushes to main.

## Publishing and maintenance

GitHub Pages publishes the root of main at https://muckorganics.com/.
Keep CNAME, canonical metadata, robots.txt and sitemap.xml consistent.
Use a pull request, wait for Site checks to pass, then merge. Main should block
force pushes and deletion, and require the Site checks job. No second-person
approval is required for the sole maintainer. Merged branches are deleted automatically.

Before publishing, preview mobile and desktop layouts and exercise navigation
and contact controls. Automated checks do not validate external websites or inbox delivery.
Domain renewal, DNS and HTTPS settings require separate verification.

The existing LICENSE file governs use of this repository.

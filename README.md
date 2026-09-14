# Capshot — downloads

This repo is public so two things can be: the page at
[capshot.me](https://capshot.me), and the installers attached to each
release.

The application source lives in a separate private repo. Nothing here is
part of the app — `index.html` is the landing page and the binaries arrive
as release assets.

Installers are release assets rather than committed files because GitHub
rejects any file over 100 MB in git, and a Capshot build is about 127 MB.

## Cutting a release

1. Build on Windows: `npm run dist:win`
2. Draft a new release here, tag it `v0.1.0`
3. Attach `Capshot-<version>-x64.exe` and `Capshot-<version>-portable.exe`
4. Publish — the download buttons point at `releases/latest`, so they
   follow automatically

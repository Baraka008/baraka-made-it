# Repository audit — first pass

## Findings
- `package.json` contains a web-app manifest (`name`, `short_name`, `start_url`, `icons`) rather than a Node package manifest. Rename it to `manifest.webmanifest` and reference it from the HTML before relying on npm scripts.
- The project is a multi-page static site (`index.html`, `booking.html`, `services.html`, `help.html`) and can be hosted on Vercel without a Node backend.
- Verify every local image path and booking/help form behavior; static hosting alone does not process form submissions.
- Add page metadata, accessible labels, responsive checks, and a clear privacy notice for any booking data.

## Verification
Root files inspected; runtime and browser checks remain outstanding.
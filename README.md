# Coupon site

The static page App Platform serves. Every rotating app is created from this
repo unchanged; only the hostname DigitalOcean assigns differs per slot.

Regenerate `index.html` from the template after editing `pages/coupon.html`
in the backend repo:

    node scripts/render-site.js

Then commit and push. Apps created after the push pick up the new content;
apps already running keep serving the old page until they are deleted.

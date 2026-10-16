# The Pelion website

Static site: `index.html` plus the `img/` folder. No build step and no database.

## Deploy
Copy `index.html` and `img/` into the web root of the server (for nginx, usually `/var/www/thepelion`), point the domain's DNS A record at the server's IP, and turn on HTTPS (for example with Let's Encrypt `certbot`).

## Before launch
- The reservation form is not connected yet. Set `FORM_ENDPOINT` near the bottom of `index.html` to a form service URL (Formspree or similar), or to a script on the server.
- Update `FOUNDING_CLAIMED` in `index.html` as founding spots sell. The bar under the $179 offer fills from it.
- Hours are copied from the business overview (weekdays 7:00 am to 8:30 pm, Saturday to noon, Sunday closed).

# The Pelion website

Static site: `index.html` plus the `img/` folder. No build step and no database.

## Deploy
Copy `index.html` and `img/` into the web root of the server (for nginx, usually `/var/www/thepelion`), point the domain's DNS A record at the server's IP, and turn on HTTPS (for example with Let's Encrypt `certbot`).

## Before launch
- Reservations are emailed to bfasano84@gmail.com through FormSubmit (formsubmit.co). The first submission sends an activation email that must be confirmed once.
- Update `SPOTS` near the top of the script in `index.html` as founding spots sell (`vip` is the $159 tier, `core` the $179 tier). The counters and bars read from it.
- The form has no payment step. Each request emails the name, contact and chosen tier, and the $50 deposit is collected by following up.
- Hours are copied from the business overview (weekdays 7:00 am to 8:30 pm, Saturday to noon, Sunday closed).

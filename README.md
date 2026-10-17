# IMAP Mobileconfig Generator

A single static page (`index.html`) that builds an Apple configuration profile
(`.mobileconfig`) adding an IMAP email account on iOS, iPadOS or macOS.

No backend and no dependencies: open `index.html` in a browser (or host it on any
static host such as GitHub Pages), fill in the account and server details, and
click **Download .mobileconfig**. Everything is generated client-side.

Add `?server=mail.example.com` to the URL to preset both the IMAP and SMTP
server fields.

Notes:
- Passwords are optional. If left blank, the device prompts for them on install.
- The profile is unsigned, so devices show it as "Not Verified". Any password you
  enter is stored in the file in plain text.

# SDA Church Calendar OAuth Pages

This public repository hosts the application homepage and privacy policy
required by Google OAuth for the private SDA Church Calendar Integration.

- Homepage: https://yaconsult.github.io/sda-church-calendar-oauth/
- Privacy policy: https://yaconsult.github.io/sda-church-calendar-oauth/privacy.html

## Why This Repository Is Public

Google requires an OAuth app with an External audience to provide publicly
accessible branding and privacy-policy URLs before moving from Testing to In
production. Google must be able to retrieve those pages without authenticating
to GitHub.

The application repository itself does not need to be public. Keeping these
small disclosure pages in a separate public GitHub Pages repository allows the
application source code to remain private.

This repository contains no application source code, OAuth credentials,
refresh tokens, calendar data, or other user data.

## Google Auth Platform Values

Use these values on the application's Branding page:

```text
Application homepage:
https://yaconsult.github.io/sda-church-calendar-oauth/

Application privacy policy:
https://yaconsult.github.io/sda-church-calendar-oauth/privacy.html

Authorized domain:
yaconsult.github.io
```

Enter the authorized domain without `https://` and without a URL path.

## Reusing This Pattern

For another private OAuth application:

1. Create a separate public repository containing only an `index.html`, a
   privacy-policy page, and explanatory documentation.
2. Explain what Google user data the application accesses and why.
3. Explain how data is stored, shared, retained, deleted, and protected.
4. Include a contact address.
5. Enable GitHub Pages from the repository's `main` branch.
6. Enter the resulting public URLs and exact GitHub Pages host name in Google
   Auth Platform.

Do not place OAuth client-secret files, `token.json`, application source code,
or user data in the public repository.

## Publishing

GitHub Pages is configured to publish from the root of the `main` branch.
Changes pushed to `main` automatically update the public pages.

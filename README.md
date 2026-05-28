# RRRTX FreeVerse — Public Certificate Registry

This repo is the public, append-only registry for certificates issued by
[RRRTX FreeVerse](https://github.com/ahmadrrrtx/rrrtx-freeverse).

## Structure

Every issued certificate is a JSON file at:
`/certs/YYYY/MM/RFV-YYYY-XXXXXXXX.json`

Each file contains:
- The certificate ID
- The recipient's display name
- A SHA-256 hash of their email (never the raw email)
- The quiz title, score, and date
- The integrity record (secure-mode status + violation count)

## Verifying a certificate

Visit https://rrrtx-freeverse.vercel.app/verify?id=RFV-YYYY-XXXXXXXX
or fetch the raw JSON file directly from this repo.

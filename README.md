# concept-email-signatures

Static asset host for Concept team email signatures, served via GitHub Pages on
`assets.conceptsf.com`.

## Layout

```
email-signature/
  jacob/    {chip,concept-logo,name,phone,web}.{png,gif}
  misha/    same five files, personalized name/chip
  zoltan/   same
  leandre/  same
```

Each asset is reachable at:

```
https://assets.conceptsf.com/email-signature/<person>/<file>
```

## Updating

Drop replacement files in the appropriate person's folder, commit, push.
GitHub Pages redeploys within ~1 minute. Hard-refresh recipient inboxes (or
wait — mail clients cache image URLs aggressively).

## DNS

`assets.conceptsf.com` is a CNAME to `<github-user>.github.io`.
Configured at the registrar that hosts conceptsf.com's DNS.

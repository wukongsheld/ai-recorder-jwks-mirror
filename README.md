# AI Recorder Google JWKS mirror

This repository mirrors the public Google OpenID Connect signing keys from
`https://www.googleapis.com/oauth2/v3/certs` for the AI Recorder identity
gateway. The keys are public and contain no credentials or user data.

GitHub Actions refreshes the JSON every two hours. Google can roll out signing
keys at slightly different times in different regions, so keys observed during
the last 72 hours are merged into the published set. Consumers must still
verify the token issuer, audience, and expiry in addition to its signature.

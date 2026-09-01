# AI Recorder Google JWKS mirror

This repository mirrors the public Google OpenID Connect signing keys from
`https://www.googleapis.com/oauth2/v3/certs` for the AI Recorder identity
gateway. The keys are public and contain no credentials or user data.

GitHub Actions refreshes the JSON every two hours. Consumers must still verify
the token issuer and audience in addition to its signature.

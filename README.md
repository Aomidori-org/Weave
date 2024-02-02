# Weave
#### Weave Micro-sites and APIs together

Weave is a like a reverse-proxy for your front-end applications.

## Features
- Authentication and Authorization (TBD)
  - Control API, site and content access (via User Scopes)
- Easy to use CORS
- Experiements (Randomized w %, User, Region)
- Site layout embedding
- Static content cache

# Archetecture
An over-simplification of Weave is an abstraction of Cloudfront.

It lets you specify S3 buckets, API gateways, http/https origins to forward content to, control headers to pass-thru, and selectively cache content.

The biggest change is that it handles your user authentication and site layout as well, makeing it easier to make several micro-sites and micro-front-ends appear as one website.

Weave is designed so that is not concerned with your rendering stratergy (ex. SSR, ISR, CSR, ODSR)

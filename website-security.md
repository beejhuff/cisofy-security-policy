# Website Security

Used technologies
- HTTPS
- HTST

## Configuration
### HTTP protocol
Where possible, servers need to be configured to allow HTTP1.1 and HTTP2. Using the latter indirectly forces to use HTTPS, which is the preferred way of deploying any service provided by our company.

### HTTPS only
All websites and intranet sites that contain confidential or sensitive data, will be HTTPS-only. The server configuration is allowed to listen to port 80 and redirect visitors to the secured protocol version.

### SSL version
Old protocol versions of SSL (SSLv2 and SSLv3) are no longer allowed, as they are considered insecure.

### TLS version
When possible, limit clients to the last few versions of the TLS protocol. Currently this is 1.1 and 1.2. Older version should only be allowed when there is a clear business need.

### Ciphers
See the useful references to create secure configurations. Always mark the configuration with a reference above the ciphers on when the configuration has been created, or last updated. This way others can see if the cipherset needs to be updated.

### Content Security Protocol (CSP)
Although not required yet, all of our websites and web-based products are expected to be configured with CSP.

## Tooling
As part of ongoing security testing, here are some of the tools that we use, besides the internal ones.

* [Mozilla SSL configuration generator ](https://mozilla.github.io/server-side-tls/ssl-config-generator/)
* [Mozilla Observatory - Test website security](https://observatory.mozilla.org/)
* [Google CSP Evaluator](https://csp-evaluator.withgoogle.com/)

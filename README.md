# API Checklist

##Best Practices
- [ ] API is using standard HTML verbs.
- [ ] API avoids using a single-endpoint. (We are not jamming multiple operations into the same endpoint with the same HTTP verb.)
- [ ] API endpoints will be on HTTPS (if needed).
- [ ] API uses JSON as it's primary request/reponse format.
- [ ] API uses HTTP Accept Headers.
- [ ] API leverages Content Delivery Network (CDN) for security and caching (if externally exposed)
- [ ] API can communicate via HTTP basic, oAuth or Akamai tokenization (ways to handshake).

##Documentation
- [ ] API has meaningful error and response messages and are being used appropiately.
- [ ] API documentation is up-to-date and documentation stays up-to-date as part of the application lifecycle.
- [ ] API documentation is offering an openly license suite of code samples, libraries and SDKs.
- [ ] API documentation is intuitive, simple, and up-to-date. Showing all API endpoints, complete with authentication details, is the standard with many APIs also providing interactive documentation using formats like Swagger or API Blueprint from Apiary.io.
- [ ] API is follow a semantically meaningful versioning convention (http://semver.org/)
- [ ] API supports CORS for security. (not JSONP)
- [ ] API supports an unlimited number of clients.
- [ ] API has 100% test coverage.
- [ ] API is designed to accommodate future and currently unknown business requirements.
- [ ] API is using security best practices (based on OWASP, etc...)
- [ ] API has a mechanism for clients to establish their own copy of the API's dataset in its entirety.
- [ ] API uses ISO 8601 in UTC for date/time.
- [ ] API responses are JSON object (not an array). 
- [ ] API should use under_score case for keys. Different languages use different case conventions. JSON uses under_score, not camelCase.

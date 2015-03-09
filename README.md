# WNMG API Standards & Best Practice Checklist

- [ ] API is using standard HTML verbs.
- [ ] API avoids using a single-endpoint. (We are not jamming multiple operations into the same endpoint with the same HTTP verb.)
- [ ] API endpoints will be on HTTPS (if needed).
- [ ] API uses JSON as it's primary request/reponse format.
- [ ] API uses HTTP Accept Headers.
- [ ] API leverages Content Delivery Network (CDN) for security and caching (if externally exposed)
- [ ] API can communicate via HTTP basic, oAuth or Akamai tokenization (ways to handshake).
- [ ] API has meaningful error and response handling. For example, good messaging for response codes and using them appropiately.
- [ ] API documentation is up-to-date and documentation stays up-to-date as part of the application lifecycle.
API documentation should be kept up-to-date as part of the application lifecycle.
API documentation should offer openly licensed suite of code samples, libraries, and SDKs should be made available in top programming languages like PHP, Python, Ruby, JavaScript, Java, C#, and possibly leading languages like Go, for developers to put to use in their integrations.
API documentation should be intuitive, simple, and up to date. Showing all API endpoints, complete with authentication details, is the standard with many APIs also providing interactive documentation using formats like Swagger or API Blueprint from Apiary.io.
APIs should follow a semantically meaningful versioning convention (http://semver.org/)
APIs should support and be tested on IE8+ and all modern browsers.
APIs output to be 508 compliant if we define output format we should be able to support.
APIs TOS & licensing with privacy.
APIs should support CORS for security. (not JSONP)
APIs should support partial request when possible.
APIs should be built to support an unlimited number of clients.
APIs should have 100% test coverage
APIs should be designed to accommodate future, currently unknown business requirements
APIs should be built using security best practices (OWASP, etc…)
APIs should support translation services like Google Translate API and Transperfect.
API’s should have some mechanism for clients to establish their own copy of the API's dataset in its entirety. If the API can't easily act as a bulk data provider, provide a separate mechanism for acquiring the backing dataset in bulk.
APIs should use ISO 8601 in UTC for date/time.
APIs responses should be a JSON object (not an array). Using an array to return results limits the ability to include metadata about results, and limits the API's ability to add additional top-level keys in the future.
APIs shouldn't use unpredictable keys. Parsing a JSON response where keys are unpredictable (e.g. derived from data) is difficult, and adds friction for clients.
APIs should use under_score case for keys. Different languages use different case conventions. JSON uses under_score, not camelCase.

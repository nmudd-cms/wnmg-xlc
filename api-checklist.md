#API Checklist
The following checklist outlines the standards and best practices development team should follow when building an API for CMS. The idea is that this checklist would exist in an API's repo and all checklist items would be completed. This checklist relies heavily on work done by 18F and the White House. We strongly recommend you checkout the links at the bottom to learn more about standards WNMG would like to align with. 

##General
- [ ] API was built using an ["API-first"](http://apievangelist.com/2014/08/11/what-is-an-api-first-strategy-adding-some-dimensions-to-this-new-question/). mentality. - Before you build your website or application you develop an API first, then you get to work on defining the channels you will be making the API resources available on.
- [ ] API is using standard HTTP verbs (GET, POST, PUT, DELETE).
- [ ] API endpoint URLs identify a resource.
- [ ] API endpoint URLs include nouns, not verbs.
- [ ] API endpoint use plural nouns only for consistency (no singular nouns).
- [ ] API uses a comma separted list for optional fields.
- [ ] API formats should be in the form of api/v2/resource/{id}.json
- [ ] API returns results with a default limit if not limit is identified.
- [ ] API uses HTTP status codes correctly to indicate response success/failure.
- [ ] API uses JSON as it's primary request/reponse format.
- [ ] API is follow a semantically meaningful versioning convention (http://semver.org/).
- [ ] API puts the version number of the API in the URL.
- [ ] API uses ISO 8601 in UTC for date/time.
- [ ] API responses are JSON object (not an array). 
- [ ] API is using under_score case for keys. (Different languages use different case conventions. We use under_scores, not camelCase).
- [ ] API avoids jamming multiple operations into the same endpoint with the same HTTP verb.
- [ ] API uses HTTP Accept Headers.
- [ ] API leverages Content Delivery Network (CDN) for security and caching (if externally exposed)
- [ ] API has meaningful error and response messages and are being used appropiately.
- [ ] API supports an unlimited number of clients and proper SLAs have been defined for the API.
- [ ] API has 100% test coverage.
- [ ] API has a mechanism for clients to establish their own copy of the API's dataset in its entirety.

##Security
- [ ] API keys and tokenization is used to track and manage clients
- [ ] API endpoints use HTTPS.
- [ ] API supports CORS for security (not JSONP).
- [ ] API is using security best practices (based on OWASP, etc...).

##Documentation
- [ ] API documentation is up-to-date and documentation stays up-to-date as part of the API lifecycle.
- [ ] API documentation is offering an openly license suite of code samples, libraries and SDKs.
- [ ] API documentation is intuitive, simple, and up-to-date. Showing all API endpoints, complete with authentication details, is the standard with many APIs also providing interactive documentation using formats like Swagger or API Blueprint from Apiary.io.

##Management
- [ ] API has “self-service” registration in place via web interface that assigns a client a API key to track and manage the API (if publically accessible). 
- [ ] API can be throttled gracefully based on specific criteria (application token, geography, environment stress).
- [ ] API has robust logging and analytics to measure usage, performance and behavior.
- [ ] API is managed in publically accessible version control system like "Github.com" for third party developers to contribute.
- [ ] API has a mechanism for clients to submit issues.
- [ ] API has a mechanism to notify clients of changes.

# Credit, Inspiration & Resources
* White House API Standards - https://github.com/WhiteHouse/api-standards
* 18F API standard - https://github.com/18F/api-standards
* 18F Developer Resource - https://18f.gsa.gov/developer/
* 18F Developer program - http://18f.github.io/API-All-the-X/
* 18F API guidelines - http://18f.github.io/API-Usability-Testing/pages/Agency-API-Guidelines

Errors
---
What, how, when, and why of errors

# What
## __er·ror__
_/ˈerər/_<br />
`a mistake.`<br />

## no but really...
invalid state, invalid arguement, or invalid precondition. Something went wrong or is wrong.

# When
Anytime an application or service encounters an invalid state, argument, or precondition. This should happen as soon as possible but no sooner.

# How
There are two main contexts in which we are handling errors. In an application and in between services.

## Appilcation
In an application context we will create javascript `Error`s.

## Services (HTTP)
Our services use HTTP/JSON. We will communicate errors to clients using a subset the canonical HTTP response [status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) (we do not need to use all of them).

- [`400 Bad Request`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400) - The request will not be processed due to something we detected as a client error
  - Syntax error in source code or AST
  - Missing required parameters
- [`401 Unauthorized`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/401) - The request did not provide valid authentication credentials
- [`403 Forbidden`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/403) - The authenticated user is not authorized to perform request
- [`404 Not Found`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/403) - The request is for a resource that cannot be found
  - The `data` (`code` or `src`) cannot be found for the provided `dataId`.

# Why

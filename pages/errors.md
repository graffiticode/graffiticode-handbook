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

# Why

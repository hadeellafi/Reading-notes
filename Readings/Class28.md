# Authentication, Authorization, Cookies

This topic is important because  Cookies allows to save information about a visitor and retrieve it on subsequent requests. This is a critical strategy that is utilized in a variety of scenarios, such as keeping the user locked in, tracking their use of the website.

## Using HTTP cookies

An HTTP cookie is a small piece of data sent by a server to a user's web browser, used to indicate if two requests come from the same browser and remember stateful information for the stateless HTTP protocol.

**Cookies are mainly used for three purposes:**

1. Session management
2. Personalization
3. Tracking

### Define the lifetime of a cookie

- Session cookies are deleted when the current session end
- Permanent cookies are deleted at a date specified by the Expires attribute.

### Restrict access to cookies

the `Secure` attribute and the `HttpOnly` attribute are used to ensure that cookies are transmitted securely and are not viewed by undesired parties or scripts.

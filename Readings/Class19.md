# Roles, Claims, and JWT Tokens

## Why Does This Topic Matter?

These concepts are foundational to the security, flexibility, and user experience of an application. They simplify access control and ensure that the appropriate users have the correct permissions.

### Claims-Based Authentication

A claim is a name-value pair that represents attributes of a subject, not what the subject can do. These attributes are characteristics of a user that the system uses to determine what actions they're allowed to perform within an application.

Claim-based authorization checks:

- Are declarative.
- Are applied to Razor Pages, controllers, or actions within a controller.
- Cannot be applied at the Razor Page handler level; they must be applied to the Page.

### JWT Authentication

JSON Web Token (JWT) is a method of representing claims for transfer between two parties.

There are three parts in JWTs:

- Header
- Payload: contains the claims
- Signature: Calculated by base64url encoding the header and payload and concatenating them with a period as a separator.

#### Producer and Consumer Concepts for APIs

- Producer: The entity providing a service (server).
- Consumer: The entity using the service (client).

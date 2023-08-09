# Claims-based authorization in ASP.NET Core

Claims-based authorization in ASP.NET Core is a way of controlling access to resources based on the claims that a user has. A claim is a piece of information about the user, such as their name, role, email, etc. A policy is a set of requirements that the user must meet to access a resource, such as having a specific claim or value. Policies can be applied to controllers, actions, razor pages, or any other resource that needs protection.

To use claims-based authorization in ASP.NET Core, we need to do the following steps:

- Assign claims to users when they sign in or register. We can use the Identity API to store and manage claims in the AspNetUserClaims table.
- Define policies that specify what claims are required for accessing a resource. we can use the AddAuthorization method in the ConfigureServices method of the Startup class to register policies.
- Apply policies to resources using the [Authorize] attribute with the Policy property. we can also use the [AllowAnonymous] attribute to override a policy for a specific resource.

## The difference between Authentication and Authorisation

Authentication and authorization are two important concepts in the field of information security. Authentication is the process of verifying the identity of a user, device, or system. It is used to ensure that the user is who they claim to be. Authorization, on the other hand, is the process of granting or denying access to a resource or service. It is used to ensure that the user has the necessary permissions to access the resource or service.

In other words, authentication is about verifying identity, while authorization is about verifying permissions. Authentication answers the question “Who are you?” while authorization answers the question "What can you do?".

## JWT Authentication

*** JSON Web Token *** is a way of sending information between two parties (such as a client and a server) in a secure and compact way. The information is encoded as a JSON object and signed with a secret key or a public/private key pair.

- The parts of a JWT token: A JWT token consists of three parts: a header, a payload, and a signature. The header contains information about the type of token and the algorithm used for its generation. The payload contains the data that the sender wants to share with the receiver. The signature is used to verify that the token has not been tampered with.
- How to authenticate servers API’s using JWT: The page uses an example of a producer and a consumer server that communicate with each other using JWT. The producer server generates a JWT token and sends it to the consumer server along with the data. The consumer server verifies the token using the same secret key or the public key of the producer server and extracts the data from the payload. The consumer server can then use the data to authorize or reject the request from the producer server.
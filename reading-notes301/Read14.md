# OAuth
OAuth allows websites and services to share assets among users. It is widely accepted, but be aware of its vulnerabilities.
## OAuth definition
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.
## OAuth history
Created and strongly supported from the start by Twitter, Google and other companies, OAuth was released as an open standard in 2010 as RFC 5849, and quickly became widely adopted. Over the next two years, it underwent substantial revision, and version 2.0 of OAuth, was released in 2012 as RFC 6749. Even though version 2.0 was widely criticized for multiple reasons covered below, it gained even more popularity. Today, you can add Amazon, Facebook, Instagram, LinkedIn, Microsoft, Netflix, Paypal and a list of other internet who’s-whos as adopters.
## OAuth explained
When trying to understand OAuth, it can be helpful to remember that OAuth scenarios almost always represent two unrelated sites or services trying to accomplish something on behalf of users or their software. All three have to work together involving multiple approvals for the completed transaction to get authorized.
## How OAuth works
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
1. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
1. The first site gives this token and secret to the initiating user’s client software.
1. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
1. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
1. The user approves (or their software silently approves) a particular transaction type at the first website.
1. The user is given an approved access token (notice it’s no longer a request token).
1. The user gives the approved access token to the first website.
1. The first website gives the access token to the second website as proof of authentication on behalf of the user.
1. The second website lets the first website access their site on behalf of the user.
1. The user sees a successfully completed transaction occurring.
1. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

# Authentication and Authorization Flows
uth0 uses the OpenID Connect (OIDC) Protocol and OAuth 2.0 Authorization Framework to authenticate users and get their authorization to access protected resources. With Auth0, you can easily support different flows in your own applications and APIs without worrying about OIDC/OAuth 2.0 specifications or other technical aspects of authentication and authorization.

## Authorization Code Flow

Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token.

- Authorization Code Flow

- Add Login Using the Authorization Code Flow

- Call API Using the Authorization Code Flow.

## Authorization Code Flow with Proof Key for Code Exchange (PKCE)
During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

- Authorization Code Flow with Proof Key for Code Exchange (PKCE)

- Add Login Using the Authorization Code Flow with PKCE

- Call API Using the Authorization Code Flow with PKCE.
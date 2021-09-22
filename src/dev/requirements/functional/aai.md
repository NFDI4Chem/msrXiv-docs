---
Changelog:

---

# Authentication and Authorization

## Basic Authentication

1. The user should be able to register locally at the server 
2. The following fields are mandatory (see also [User accounts](accountmanagement.md#users-and-user-accounts))
   - username
   - password 
   - email
   - full name
3. The following fields are optional (see also [User accounts](accountmanagement.md#users-and-user-accounts))
   - institution
   - photo
4. email address is verified by sending a verification link which must be followed
5. The user is able to reset the password by email
   - a link for new password will be sent


### Validation
1. The email address is a valid email address (RFC5322,RFC6530)and unique
2. The username is unique
3. The password has at least 8 chars

## Common NFDI(4Chem) AAI
### Elixir AAI
[Documentation](https://docs.google.com/document/d/1ihb0hH2YJqSCPZS0syVpvAOeQP1HTxdf_XMsZZLe_W0/edit)
- the application is a SAML 2.0 Service Provider for Elixir
- OR the application is an OpenID Connect Relying Party

### Orcid
- The application supports login with the Orcid ID

### Optional: nmrXiv
- login with your nmrXiv account

## Other single sign on possibilities
* github.com
* twitter



---
Version: 0.1

Date: 2021-09-16

Changelog:

---

# Authentication and Authorization

## General Authentification

### Local Authentification

1. The user should be able to register locally at the server 
2. The following fields are mandatory 
   - username
   - password 
   - email
   - full name
3. The following fields are optional
   - institution
4. email address is verified by sending a verification link
5. The user is able to reset the password by email
   - a link for new password will be sent


#### Validation
1. The email address is a valid email address (RFC5322,RFC6530)and unique
2. The username is unique
3. The password has at least 8 chars

## Common NFDI(4Chem) AAI
### Elixir AAI
[Documentation](https://docs.google.com/document/d/1ihb0hH2YJqSCPZS0syVpvAOeQP1HTxdf_XMsZZLe_W0/edit)
- The application is a SAML 2.0 Service Provider for Elixir

OR

- The application is an OpenID Connect Relying Party

### Orcid
- The application supports login with the Orcid ID

### Optionional: nmrXiv
- login with your nmrXiv account

## Roles
### Access for reviewers
- Reviewers get a password to access the resource they are reviewing
- Reviewers have read-only access to this resource


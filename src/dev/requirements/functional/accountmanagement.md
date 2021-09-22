---
Changelog:

---

# Account management

## Content
- [Users and user accounts](#users-and-user-accounts)
- [User login](#user-login)
- [Roles](#roles)
- [Teams](#teams)
- [Authentication and authorization](aai.md)

## Users and user accounts

1. A user generally is a single person with an account
2. Anyone can register an account
3. Each account contains a user profile with user specific information and settings
4. An account at least includes the following information
    1. Full (real) name of the user
    2. Username (unique short name)
    3. An email address
        * The e-mail address must be verified by the user
    4. At least one authentication method including necessary additional information
        * Authentication methods are described in [AAI](aai.md)
        * multiple authentication methods are possible
5. Additionally, an account can include the following information
    * an institution name
    * API Tokens (for access by external access)
    * A profile photo
      * profile photos have a recommended (**TODO**) size and format
      * MIME: PNG, JPEG
    * Team memberships
      * see [Teams](#teams)
    * Two-factor authentication
    * Roles 
      * see [Roles](#Roles)
    * Linked social accounts
      * social account links contain a provider name and an ID for the user
7. Users can change their profile information
8. User information can be edited by users with permissions (**TODO**)
9. The user gets a notification on changes made by anyone else

## User login
1. users choose their authentication method for login
2. They are asked to provide authentication information, e.g. username and password, or are redirected to an external site
3. Users can reset their authentication credentials if allowed by the method

## Roles
### Global
* super-admins - roles, read/write all data, stats on the platform
* curators - read/write, stats (UI)
* community-curators - read, stats
* advisor - read, stats
* developer - read (API)

### Team / Project
* owner - read/write
* collaborator - comment (private)
* reviewer - read only (optional)
  * Read only reviewer link (password)

## Teams
1. A team is a group of users
2. Each team has one owner
3. Each user is at least in one team, called the "personal team"
4. Each member of a team has permissions in the team defined by role
   * see [Roles](#roles)
5. Any User can create a new team and will be the owner
6. Ownership for non-personal teams can be transferred to members (by current owner)
7. Users have to be invited to a team by the owner or a member (by owner)
8. To invite a user to a team a username or email address and a role have to be provided
   * an external person can be invited by email and have to create an account
   * users will be notified about invitations
9. Users can be removed from teams (by owner)
10. Members are notified about changes in the team
11. A non-personal team can be removed (including memberships)




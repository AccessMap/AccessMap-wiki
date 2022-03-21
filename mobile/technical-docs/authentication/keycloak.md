# Summary
In the past, we manually created our own user/profiles/auth API server [here](https://github.com/AccessMap/accessmap-api) (Now Outdated). We would like to consolidate the authentication service across all AccessMap (and some other TCAT) applications. This means that a user of AccessMap web would be able to sign in with social media login or their account (managed by Keycloak), create profile on AccessMap web, then go to AccessMap mobile, sign in, and see the profiles they had saved.
To do this, we are investigating the usage of **Keycloak**, an open source Identity and Access Management service.

## What has been Accomplished
- Deployed the Keycloak server to Azure (accessible through: https://identity.opensidewalks.com)
  - Please contact the team for credentials
- Code for a Node.js server created [here]() (still needs to be pushed to Nick's Azure server and to our GitHub group, currently deployed on Jay's test server [here](https://accessmap-backend.herokuapp.com/api/v1/))


## Issues
- Need to resolve the 403 Access Denied after a user on the mobile app gets a valid unexpired token and tries to make a request to the backend with keycloak.protect() on.

## Links
Meeting Notes: https://docs.google.com/document/d/1zGyKTWw-4pY13WDBmWGbLFiFz792vkhbgmpwSk7a3ZU/edit?usp=sharing
# Summary
AccessMap Profiles Backend is a Node.js server written with Typescript. It handles connecting
users of AccessMap (mobile, web, and beyond) to their custom mobility profiles (maximum tolerated uphill/downhill steepness etc).
Link to profiles backend codebase: https://github.com/AccessMap/accessmap-backend

## PostgreSQL and Keycloak
Profiles Backend utilizes Keycloak Authentication to protect the endpoints and a PostgreSQL database to store user profiles.

## Database
Database Table example: 
```markdown
   user_id    | uphill_max | downhill_max | avoid_curbs 
--------------+------------+--------------+-------------
mice1-j0fl-46 |         10 |            5 | f
jkp55-pinld3  |          6 |            1 | t
```

Where the column types are:
```markdown
    Column    |          Type          | Collation | Nullable | Default 
--------------+------------------------+-----------+----------+---------
 user_id      | character varying(255) |           | not null | 
 uphill_max   | integer                |           |          | 
 downhill_max | integer                |           |          | 
 avoid_curbs  | boolean                |           |          | 
```

The user_id should be the keycloak-assigned user ID for the logged in user.

## Keycloak
You must have the following set in your environment variables: 
- DATABASE_URL (url of your postgresql db instance)
- POSTGRES_USER (db username)
- POSTGRES_PASSWORD (db password)
- REALM_PUBLIC_KEY (for accessing resources from the keycloak server)

## TODO
- Get Login feature to work with keycloak (or any third party OIDC) (investigate why keycloak.protect() is returning a 403)
- Consider scalability of database
  - Note that keycloak already handles user registration + social media login + identity for us. Do not create redundancy.
  - The purpose of the Profile table is to store the mobility profile values of the user registered with keycloak.
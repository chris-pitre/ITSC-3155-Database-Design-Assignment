# v1 ERD
![ERD](Database%20Design%20Assignment%20ERD.png)

# Plan to migrate schema to v2
The schema designed in v1 is relatively flexible so making changes to migrate over to v2 will be easy.

## Features to be added in v2
1. Multiple playlists for users
2. Multiple account types for users

## How to add each feature
1. To add multiple playlists for users, first we would remove the playlist_id column from the user table. In the playlist table, a user_id column would be introduced as a foreign key to allow for a one to many relationship between users and playlists.
2. To add multiple account types for users, a new account type column with enumerators for each account type would be added to the user table. The privileges would be handled by whatever backend uses the database and not by the database itself.

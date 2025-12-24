# Users and Groups

## Cos'è
Users and groups manage access and permissions for different people on the system.

## Perché è importante
Proper user and group management ensures security, prevents unauthorized access, and organizes permissions.

## Comandi principali
```bash
id <user>           # Show user and group IDs
whoami              # Show current user
adduser username    # Create new user
usermod -aG group user  # Add user to group
groups username     # List groups of a user

## Errori comuni
- Giving too many privileges to users
- Forgetting to remove inactive users
- Not checking group memberships for access control

# Linux Permissions

## Cos'è
Linux permissions control access to files and directories using read, write, and execute flags for owner, group, and others.

## Perché è importante
Understanding permissions is crucial for security, avoiding unauthorized access, and privilege escalation.

## Comandi principali
```bash
ls -l           # Shows file permissions
chmod 755 file  # Change permissions
chown user:group file  # Change ownership

## Errori comuni
- Setting too permissive permissions (e.g., 777)
- Not checking ownership before editing system files
- Ignoring permission inheritance in directories

# Linux Logs

## Cos'è
Logs are files that record system events, errors, and user activity.

## Perché è importante
Monitoring logs helps diagnose issues, detect intrusions, and maintain system health.

## Comandi principali
```bash
tail -f /var/log/syslog     # Follow log in real time
cat /var/log/auth.log       # View authentication logs
grep "error" /var/log/*     # Search for errors in logs

## Errori comuni
- Ignoring log file locations
- Using logs without understanding context
- Not rotating or archiving old logs

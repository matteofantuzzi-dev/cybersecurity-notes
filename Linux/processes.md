# Linux Processes

## Cos'è
Processes are programs currently running on the system. Each process has an ID (PID) and runs with specific permissions.

## Perché è importante
Monitoring processes helps understand system behavior, detect suspicious activity, and manage resources.

## Comandi principali
```bash
ps aux       # List all running processes
top          # Interactive process monitor
kill <PID>   # Terminate a process by PID

## Errori comuni
- Killing the wrong process without checking PID
- Ignoring background processes that consume resources

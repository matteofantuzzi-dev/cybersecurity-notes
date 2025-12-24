# Bash Scripting

## Cos'è
Bash scripting allows automating tasks in Linux using shell commands, loops, and conditionals.

## Perché è importante
Automation saves time and is essential for administration, penetration testing, and repetitive tasks.

## Comandi principali
```bash
#!/bin/bash        # Script shebang
echo "Hello"       # Print text
for i in {1..5}; do echo $i; done  # Loop example
if [ -f file ]; then echo "Exists"; fi  # Conditional example

## Errori comuni
- Forgetting the shebang line
- Incorrect syntax in loops or conditionals
- Running scripts without execute permissions

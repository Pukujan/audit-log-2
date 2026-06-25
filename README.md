# audit-log-2

Reserved Stupidly Simple Cortex audit-log shard.

Use this repo when `audit-log-1` reaches the configured shard limit.

Entries belong in:

```text
agent/
```

Search the library first:

```powershell
cd ..\audit-log-library
rg -i "query" ..\audit-log-1\agent ..\audit-log-2\agent
```


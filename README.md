# audit-log-2

Reserved Stupidly Simple Cortex audit-log shard.

Use this repo when `audit-log-1` reaches the configured shard limit.

## Exact Problem It Solves

This repo keeps the audit-log system ready to scale before it is urgent.

Memory providers do not normally create the next GitHub-backed audit shard when
the current one gets too large. Cortex does. `audit-log-2` is the reserved next
place for compact fix logs once `audit-log-1` should stop growing.

Entries belong in:

```text
agent/
```

Search the library first:

```powershell
cd ..\audit-log-library
rg -i "query" ..\audit-log-1\agent ..\audit-log-2\agent
```

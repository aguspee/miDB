AguspeDB is composed of the following modules:

- Parser
- Executor
- Storage Engine
- Index Manager
- Catalog

Query flow:

SQL → Parser → Executor → Storage → Disk

uses fixed-size pages of 8192 bytes.

Each page contains:

- PageHeader
- Slot directory
- Free space
- Row data

Each slot contains:
-Offset
-Length
-Flag (deleted)
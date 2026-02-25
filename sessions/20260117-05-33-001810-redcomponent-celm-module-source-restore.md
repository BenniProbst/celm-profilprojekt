# Session: redcomponent-celm module source restore

Date: 2026-01-17 05:33
Scope: Restore redcomponent-celm module sources after wrapper cleanup removed content; keep the duplicate target guard.

## Updates
- Restored the full module source tree (include/src/tests/third_party) from the emergency backup after the wrapper commit removed it.
- Kept the early TARGET guard in CMakeLists.txt to avoid duplicate target definitions when module and product clones are built together.

## Files
- CMakeLists.txt
- include/
- src/
- tests/
- third_party/
- main.cpp
- sessions/20260117-05-33-001810-redcomponent-celm-module-source-restore.md

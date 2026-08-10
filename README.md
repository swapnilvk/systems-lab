# systems-lab
C++20 systems programming lab. Covers low-latency concurrency, profiling, Linux internals, and on-device AI inference.

## Status
Phase 1: Systems Core

## Highlights
- [Event Bus](week12-event-bus/) — lock-aware pub/sub, p99 latency Xµs
- [False Sharing Bench](benches/week03-false-sharing/) — 3.2x speedup via padding
- [SPSC Queue](week08-spsc-queue/) — TSan-clean lock-free ring buffer

## Build
\`\`\`bash
cmake -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build
ctest --test-dir build
\`\`\`

## Structure
| Folder | Description |
|---|---|
| weekNN-*/ | Weekly katas and labs |
| benches/ | Profiling results and flamegraphs |
| notes/ | Learning log, retros, resume notes |

## Author
Swapnil Kulkarni — [swapnilvk.github.io](https://swapnilvk.github.io)

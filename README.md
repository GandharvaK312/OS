# OS / Systems Roadmap

---

## Phase 0 - Foundations

## Completed projects

- [x] [A memory manager in C (Heap manager + garbage collector)](https://github.com/gandharvak312/memory-manager-c)

## Current Status (as of Sept 2026)

**Active right now:**

- [LeetCode problem-solving in systems-style C](https://github.com/gandharvak312/The-C-Programming-Language)

- [Computer Organization and Architecture](./resources/Computer%20Organization%20and%20Embedded%20systems%20Carl%20Hamacher.pdf)

- [nand2tetris](./resources/The%20Elements%20of%20Computing%20Systems%20_%20Building%20a%20Modern%20Computer%20from%20First%20Principles,%202nd%20edition,%202021.pdf)

- [ ] Start rated Codeforces contests alongside LeetCode — external, comparable signal (Candidate Master+) beyond archive-grinding

---

## Phase 1 — C mastery consolidation (ongoing, parallel to Phase 0)

- [ ] Finish KN King
- [ ] Beej's Guide to C (short, sharper on pointers/memory than King)
- [ ] Read x86-64 assembly at a basic level (not write it) — use Compiler Explorer (godbolt.org)
- [ ] Get fluent in `gdb` — non-negotiable for OS work

## Phase 1.5 — C++ transition (once C fundamentals are solid, before/parallel to Phase 2)

- [ ] "A Tour of C++" (Stroustrup) — fast, dense overview of modern C++ from someone who already knows C
- [ ] Core practice: RAII, move semantics, smart pointers, templates basics
- [ ] "Effective Modern C++" (Scott Meyers) — idiomatic modern C++ (C++11/14 practices that still matter)
- [ ] Port a couple of existing C projects (allocator, a nand2tetris component) to modern C++ as a forcing function

## Phase 2 — OS theory foundation (next semester, when OS course starts)

- [ ] OSTEP (Operating Systems: Three Easy Pieces) — primary text, free online
  - [ ] Virtualization: processes, CPU scheduling
  - [ ] Virtualization: memory (address spaces, paging, segmentation, TLBs)
  - [ ] Concurrency: threads, locks, condition variables, deadlock
  - [ ] Persistence: file systems, disks, RAID
- [ ] Silberschatz — secondary/reference, already on GATE book list, useful for coursework alignment
- [ ] Do OSTEP's homework simulators (scheduling, paging) alongside reading

## Phase 3 — Build a real (tiny) OS kernel

Pick a track:

**Guided track (recommended given timeline pressure):**
- [ ] xv6 source read-through
- [ ] MIT 6.828/6.1810 (Operating System Engineering) labs — syscalls, scheduler, virtual memory, basic file system, shell

**Harder mode (optional deep-dive later, not the main track):**
- [ ] OSDev wiki "Bare Bones" — bootloader, real mode → protected mode, GDT/IDT, paging by hand

## Phase 4 — Specialize (trading OS / unikernel direction, final year)

- [ ] Unikernel study: Unikraft (most engineering-accessible), MirageOS, OSv
- [ ] Network programming: Beej's Guide to Network Programming → then DPDK docs, io_uring
- [ ] Lock-free data structures: "The Art of Multiprocessor Programming" (Herlihy & Shavit), esp. memory ordering / atomics — checkpoint: implement a lock-free SPSC queue
- [ ] Networking/latency measurement work, building on the DPDK/io_uring study above
- [ ] NUMA-aware memory (Linux kernel docs, papers — learned in-context once deep in Phase 4)
- [ ] **Capstone: order book implementation** — ties lock-free structures + networking + low-latency design into one artifact defensible line-by-line in interviews

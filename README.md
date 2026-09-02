# OS / Systems Roadmap

Single source of truth. Update the checkboxes as you go instead of re-deriving the plan from scratch every few weeks.

---

## Current Status (as of Sept 2026)

**Active right now:**

- [ ] [LeetCode problem-solving in systems-style C](https://github.com/gandharvak312/The-C-Programming-Language)

- [ ] [Computer Organization and Architecture](./resources/Computer Organization and Embedded systems Carl Hamacher.pdf)

- [ ] a small "break in" kernel/OS project garbage collector in C

---

## Phase 0 — Foundations (now)
  
- [ ] [Computer Organization and Architecture](./resources/Computer Organization and Embedded systems Carl Hamacher.pdf)

- [ ] [LeetCode problem-solving in systems-style C](https://github.com/gandharvak312/The-C-Programming-Language)

- [ ] Garbage Collector in C

- [ ] nand2tetris Part I (projects 1-6: gates → ALU → CPU → assembler) — run parallel to COA, patches the exact "shaky registers/counters" gap from top-down Hamacher explanations

## Phase 1 — C mastery consolidation (ongoing, parallel to Phase 0)

- [ ] Finish KN King
- [ ] Beej's Guide to C (short, sharper on pointers/memory than King)
- [ ] Read x86-64 assembly at a basic level (not write it) — use Compiler Explorer (godbolt.org)
- [ ] Get fluent in `gdb` — non-negotiable for OS work

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
- [ ] Lock-free data structures: "The Art of Multiprocessor Programming" (Herlihy & Shavit), esp. memory ordering / atomics
- [ ] NUMA-aware memory (Linux kernel docs, papers — learned in-context once deep in Phase 4)

## Deferred / Later

- [ ] malloc family (malloc/calloc/realloc/free) — full implementation, revisit after break-in project + stronger fundamentals

---

### Notes
- Rough timeline: Phase 0/1 this semester → Phase 2 next semester (parallel with OS coursework) → Phase 3 over summer break + following semester (don't rush, it's the meatiest chunk) → Phase 4 final year.
- Don't skip straight to Phase 4 material (DPDK, unikernels) without Phase 3's xv6-level grounding — it'll show in interviews.

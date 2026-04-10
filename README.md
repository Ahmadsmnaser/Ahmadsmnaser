<h1 align="center">Hi 👋, I'm Ahmad Naser</h1>

🎓 **B.Sc. in Computer Science – Ben-Gurion University**<br>
💻 **Software Engineer | Low-Level & Systems Programming**<br>
🌍 Based in Israel<br>

I work close to the machine — kernel internals, memory management, syscall tracing, and scheduling.
I care about understanding how software actually runs: how the scheduler picks the next task, how memory gets allocated and freed, how a process call crosses into the kernel.

Currently a **Software Engineering Intern at Siraj Technologies**, and actively seeking my first full-time role in **systems, infrastructure, or performance engineering**.

---

## 🔥 Featured Projects

### 🧠 Scheduler Study — Kernel + Userspace

A two-part study on CPU scheduling built from the ground up.

| Project | What it does | Tech |
|---|---|---|
| ⚙️ [**SchedScope**](https://github.com/Ahmadsmnaser/SchedScope-Linux-Kernel-Scheduler) | Instruments and modifies `pick_next_task_fair()` in Linux 6.6 inside QEMU. Introduces a controlled vruntime placement bias and measures the effect: **+64% context switches, +66% preemptions** vs baseline CFS. Full trace → metrics → plots pipeline. | C, Linux Kernel, QEMU, ftrace, Python |
| 🔬 [**Mini Scheduler**](https://github.com/Ahmadsmnaser/Mini-Scheduler) | Deterministic userspace simulator in C11 that mirrors the same scheduling concepts. Compares Round Robin vs Fair on identical workloads: Fair cut response time to zero for all tasks at the cost of **+366% context switches**. Same trace format as SchedScope. | C11, JSON |

> Built SchedScope to work inside the real kernel. Built Mini Scheduler to iterate on policy logic in milliseconds. Same concepts, two levels of the stack.

---

### 🕵️ [SysPeek — Linux Syscall Tracer](https://github.com/Ahmadsmnaser/Syspeek-Syscall-Tracing-Tool)

A lightweight Linux system call tracer built on `ptrace`, inspired by `strace`.

- Traces syscall entry and exit: number, name, up to 6 arguments, return value, errno
- x86_64 syscall table with named mapping (`write`, `openat`, `execve`, ...)
- No external dependencies — pure C, pure Linux
- Tested against real programs: file I/O, heap allocation, process execution

> Hands-on understanding of Linux syscall mechanics, ptrace-based process control, and x86_64 ABI register layout.

---

### 🦅 [HawkAlloc — Custom Memory Allocator](https://github.com/Ahmadsmnaser/HawkAlloc)

A userspace dynamic memory allocator implementing `malloc`, `free`, `calloc`, and `realloc` from scratch.

- Arena-based allocation via `mmap`
- Doubly-linked free list with first-fit search
- Block splitting and forward coalescing to reduce fragmentation
- 10,000-iteration stress test with pattern verification and corruption detection
- Validated with AddressSanitizer

---

### ⚙️ [xv6 Kernel Enhancements](https://github.com/Ahmadsmnaser/Operating-Systems)

Three independent kernel-level extensions on the xv6 teaching OS:

- **System calls:** Added new syscalls with full user→kernel data transfer and argument validation
- **Shared memory:** Implemented cross-process shared memory using page table manipulation and reference counting
- **Synchronization:** Peterson locks, sleep/wakeup primitives, and condition variables — debugged under QEMU/GDB to eliminate race conditions

---

### 🔌 [SPL — System Programming Projects](https://github.com/Ahmadsmnaser/SPL-System-Programming-Laboratory)

Three systems-focused projects in Java and C++:

- **TFTP Server/Client:** Binary protocol over TCP, thread-per-client architecture, concurrent file upload/download with server-wide notifications
- **Set Card Game:** Multithreaded game engine with thread-safe state management and synchronization primitives
- **Warehouse Management System:** OOP design in C++ with strict Rule-of-5 memory management and zero leaks

---

## 🧠 Technical Skills

### Languages
- **C, C++, Java**
- Python, JavaScript / TypeScript

### Systems & Low-Level
- Linux kernel internals — scheduler (`fair.c`, `core.c`), `task_struct`, runqueues, vruntime
- `ptrace`, syscall tracing, x86_64 ABI
- Memory management — allocators, `mmap`, free lists, heap layout, coalescing
- Processes, threads, scheduling, preemption
- Locks, synchronization, race conditions, Peterson algorithm
- xv6 kernel — page tables, reference counting, trap handling
- Debugging: **GDB**, **Valgrind**, **AddressSanitizer**, **UBSan**
- `ftrace`, `trace_printk`, QEMU

### Backend & Infrastructure
- Java, Spring Boot
- TCP/IP, binary protocols, client–server architecture
- Docker, Azure DevOps
- REST APIs, Cucumber/BDD

### Tools
- Linux, Git, Make
- QEMU / GDB
- Docker, Postman

---

## 🎯 What I'm Looking For

A role where I work close to the system — **kernel, systems software, infrastructure, or performance engineering**.
Ideally somewhere that cares about how things actually work under the hood.

---

## 🤝 Let's Connect

📧 **Email:** Ahmadsmnaser@gmail.com<br>
📞 **Phone:** +972-50-314-8019<br>
🔗 **LinkedIn:** https://www.linkedin.com/in/ahmadsmnaser<br>
🐙 **GitHub:** https://github.com/Ahmadsmnaser<br>
🌐 **Website:** https://personal-websiteahmad.vercel.app/<br>

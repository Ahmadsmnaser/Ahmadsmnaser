<h1 align="center">Hi 👋, I'm Ahmad Naser</h1>

🎓 **B.Sc. in Computer Science – Ben-Gurion University**
💻 **Software Engineer | Low-Level & Systems Programming**
🌍 Based in Israel

I'm a software engineer who works close to the machine — operating systems, kernel internals, memory management, and system call tracing.
I care about understanding how software actually runs: how the scheduler picks the next task, how memory gets allocated and freed, how a process call crosses into the kernel.

Currently a **Software Engineering Intern at Siraj Technologies**, and actively seeking my first full-time role in **systems, infrastructure, or performance engineering**.

---

## 🔥 Featured Projects

### 🧠 Scheduler Study — Kernel + Userspace

A two-part study on CPU scheduling, built from the ground up.

| Project | What it does | Tech |
|---|---|---|
| ⚙️ [**SchedScope**](https://github.com/Ahmadsmnaser/SchedScope-Linux-Kernel-Scheduler) | Instruments and modifies `pick_next_task_fair()` in Linux 6.6 inside QEMU. Introduces a controlled vruntime placement bias and measures the effect: **+64% context switches, +66% preemptions** vs baseline CFS. Full trace → metrics → plots pipeline. | C, Linux Kernel, QEMU, ftrace, Python |
| 🔬 [**Mini Scheduler**](https://github.com/Ahmadsmnaser/Mini-Scheduler) | Deterministic userspace simulator in C11 that mirrors the same scheduling concepts. Compares Round Robin vs Fair on identical workloads: Fair cut response time to zero for all tasks at the cost of **+366% context switches**. Same trace format as SchedScope. | C11, JSON |

> Built SchedScope to work inside the real kernel. Built Mini Scheduler to iterate on policy logic in milliseconds. Same concepts, two levels of the stack.

---

### 🕵️ [SysPeek — Linux Syscall Tracer](https://github.com/Ahmadsmnaser/syspeek)

A lightweight Linux system call tracer built on `ptrace`, inspired by `strace`.

- Traces syscall entry and exit with number, name, arguments, return value, and errno
- x86_64 syscall table with named mapping (`write`, `openat`, `execve`, ...)
- No external dependencies — pure C, pure Linux
- Tested against real programs: file I/O, heap allocation, process execution

> Demonstrates hands-on understanding of Linux syscall mechanics, ptrace-based process control, and register-level ABI reasoning.

---

### 🦅 [HawkAlloc — Custom Memory Allocator](https://github.com/Ahmadsmnaser/HawkAlloc)

A userspace dynamic memory allocator implementing `malloc`, `free`, `calloc`, and `realloc` from scratch using `mmap` and free list management.

---

### Other Projects

| Project | Description | Tech |
|---|---|---|
| ⚙️ **xv6 Kernel Enhancements** | Extended xv6 with new system calls, process lifecycle logic, synchronization, and shared memory via page tables and reference counting | C, xv6, QEMU, GDB |
| 🔌 **Client–Server IPC System** | Custom application-level protocol over TCP with a multithreaded server | Java, TCP/IP, Sockets |
| 🎮 **Set Game – Multithreaded Engine** | Thread-safe game logic with synchronization primitives and concurrent data structures | Java, Threads, Locks |
| 🔐 **Chrome Security Extension** | File hashing and threat analysis pipeline using external threat-intelligence APIs | JavaScript, Chrome APIs, REST |

---

## 🧠 Technical Skills

### Languages
- **C, C++, Java**
- Python, JavaScript / TypeScript

### Systems & Low-Level
- Linux kernel internals — scheduler (`fair.c`, `core.c`), `task_struct`, runqueues
- `ptrace`, syscall tracing, x86_64 ABI
- Memory management — allocators, `mmap`, heap layout
- Processes, threads, scheduling, preemption
- Locks, synchronization, race conditions
- Debugging with **GDB**, **Valgrind**, **AddressSanitizer**
- QEMU, `ftrace`, `trace_printk`

### Backend & Infrastructure
- Java, Spring Boot
- TCP/IP, client–server architecture
- Docker, Azure DevOps
- REST APIs

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

📧 **Email:** Ahmadsmnaser@gmail.com
📞 **Phone:** +972-50-314-8019
🔗 **LinkedIn:** https://www.linkedin.com/in/ahmadsmnaser
🐙 **GitHub:** https://github.com/Ahmadsmnaser
🌐 **Website:** https://personal-websiteahmad.vercel.app/

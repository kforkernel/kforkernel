### `$ fastfetch --config minimal`

```text
       .--.          kforkernel@devbox
      |    |         -----------------
      |    |         LANGUAGES: Rust, C, C++, Python, Bash, HTML/CSS, SQL
     //   \ \        OS:        Linux, FreeBSD, OpenBSD, Android, Windows (7/10/11)
    (|     | )       SYSADMIN:  RHCSA-level Linux Administration
   /'\_   _/`\       KERNEL:    OS Development [IN PROGRESS]
   \___)=(___/       NETWORK:   CCNA-level Networking & Protocols
                     HARDWARE:  MCU Programming, Circuit Design & Prototyping
```

---

```yaml
kforkernel@localhost:~$ uname -a
Linux kernel-dev 6.x.x-custom #1 SMP PREEMPT_DYNAMIC x86_64 GNU/Linux

kforkernel@localhost:~$ ./whoami --verbose

USER:       kforkernel
ROLE:       Aspiring Systems Programmer | OSev & Kernel Enthusiast | Hardware Tinkerer | Linux Enjoyer | BSD Lover
MISSION:    Exploring how computers work from bare-metal hardware up to userspace.
```

---

### `$ cat /proc/focus`
> Focused on **operating system development** and **low-level systems programming**—building software close to the metal, understanding kernel internals, and bridging the gap between hardware and code.

```text

       |  |  |  |  |  |  |  |
     .------------------------.
   --|   [ KERNEL RING 0 ]    |--
   --|   ARCH:   x86_64/ARM   |--
   --|   MEM:    MMU / Paging |--
   --|   MODE:   Bare-Metal   |--
     '------------------------'
       |  |  |  |  |  |  |  |
```

---

### `$ ls -la ~/interests/`

```text
drwxr-xr-x  2 kforkernel wheel  4096 Nov 22 05:22 .
drwxr-xr-x 14 kforkernel wheel  4096 Nov 22 05:22 ..
-rw-r--r--  1 kforkernel wheel   512 Nov 22 05:22 os_and_kernel.txt      # OS architecture, kernel programming, memory management
-rw-r--r--  1 kforkernel wheel   512 Nov 22 05:22 systems_prog.txt       # Low-level Rust & C/C++, Linux internals
-rw-r--r--  1 kforkernel wheel   512 Nov 22 05:22 infra_and_net.txt      # Linux sysadmin, routing/switching, network protocols
-rw-r--r--  1 kforkernel wheel   512 Nov 22 05:22 hardware_embedded.txt  # MCU firmware, circuit design, bare-metal prototyping
```

---

### `$ cat ~/projects/roadmap.c`

```c
#include <stdio.h>
#include <stdbool.h>

#define ARCH "x86_64"

typedef enum {
    STATUS_STUDYING,
    STATUS_WRAPPING_UP,
    STATUS_ACTIVE
} State;

typedef struct {
    const char *name;
    const char *lang;
    const char *desc;
    State status;
} Project;

int main(void) {
    Project current[] = {
        {
            .name   = "rust-shell",
            .lang   = "Rust",
            .desc   = "Custom POSIX-like shell (piping, redirection, job control)",
            .status = STATUS_WRAPPING_UP
        },
        {
            .name   = "c-coreutils",
            .lang   = "C",
            .desc   = "Reimplementing standard Linux GNU coreutils from scratch",
            .status = STATUS_ACTIVE
        },
        {
            .name   = "rust-coreutils",
            .lang   = "Rust",
            .desc   = "Memory-safe Linux coreutils rewrite for systems practice",
            .status = STATUS_ACTIVE
        },
        {
            .name   = "custom-os",
            .lang   = "C / Rust / Asm",
            .desc   = "Studying OS theory, bootloaders, and kernel internals",
            .status = STATUS_STUDYING
        }
    };

    printf("Loaded %zu active systems projects on %s.\n",
           sizeof(current) / sizeof(current[0]), ARCH);

    return 0;
}
```

```text
kforkernel@localhost:~\$ fortune -s
"Talk is cheap. Show me the code." — Linus Torvalds

kforkernel@localhost:~\$ █
```

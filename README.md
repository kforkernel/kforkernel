<div align="center">

# `kforkernel`
**Systems Programmer • Windows Trampler • OS & Kernel Enthusiast • Hardware Tinkerer • Penguin Herder • Packet Plumber**

[Email](mailto:contact@kforkernel.com) • [Matrix](https://matrix.to/#/@kforkernel:matrix.org) • [Website (WIP)](https://kforkernel.com)

</div>

---
***
___

### `$ fastfetch --config minimal`

```text
_     __            _                   _ 
| | __/ _| ___  _ __| | _____ _ __ _ __ | |
| |/ / |_ / _ \| '__| |/ / _ \ '__| '_ \| |
|   <|  _| (_) | |  |   <  __/ |  | | | | |
|_|\_\_|  \___/|_|  |_|\_\___|_|  |_| |_|_|

[ ring 0 // bare-metal -> userspace ]


       .--.          kforkernel@devbox
      |    |         -----------------
      |    |         LANGUAGES: Rust, C, C++, Python, Bash, HTML/CSS, SQL
     //   \ \        OS:        Linux, FreeBSD, OpenBSD, Android, Windows (7/10/11)
    (|     | )       SYSADMIN:  RHCSA-level Linux Administration
   /'\_   _/`\       KERNEL:    OS Development [IN PROGRESS]
   \___)=(___/       NETWORK:   CCNA-level Networking & Protocols
                     HARDWARE:  MCU Programming, Circuit Design & Prototyping

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

### `$ cat /usr/bin/projects.rs`

```rust
#![allow(dead_code)]
use std::{
    net::{IpAddr, TcpStream},
    os::unix::fs::PermissionsExt,
    process::Command,
    sync::Arc,
};

struct Engineer {
    focus: &'static [&'static str],
    infrastructure: Infrastructure,
    projects: Projects,
    security: Security,
}

struct Infrastructure {
    networking: &'static [&'static str],
    self_hosted: &'static [&'static str],
}

struct Projects {
    systems_cli: &'static [&'static str],
    embedded_firmware: &'static [&'static str],
}

struct Security {
    offensive_labs: &'static [&'static str],
    cryptography: &'static [&'static str],
}

pub fn build_profile() -> Engineer {
    Engineer {
        focus: &[
            "Linux Systems Administration",
            "Low-Level & OS Development",
            "Embedded Firmware Engineering",
            "Network Architecture",
        ],
        infrastructure: Infrastructure {
            networking: &[
                "Multi-VLAN segmented enterprise topologies (L2/L3 switching)",
                "Dynamic routing via OSPF & custom static routing tables",
                "Link aggregation using EtherChannel (LACP/PAgP)",
                "Core network services: DHCP, hardened SSH, & LAN provisioning",
            ],
            self_hosted: &[
                "Encrypted DNS sinkhole (AdGuard Home) with DNS-over-TLS (DoT)",
                "Internal PKI & custom Certificate Authority (CA) for local HTTPS",
                "Privacy-respecting metasearch engine (SearXNG)",
                "Multi-protocol file storage servers (SMB/Samba & FTP)",
            ],
        },
        projects: Projects {
            systems_cli: &[
                "Rust: Cryptographic file encryption utility",
                "Rust: Data compression & archival CLI tool",
                "Rust: SHA checksum hashing & integrity verification tool",
                "Python: Terminal-based raw HTTP/HTTPS web client",
                "C: Command line utilities and games",  
            ],
            embedded_firmware: &[
                "Bare-metal C/C++ firmware for microcontroller (MCU) peripherals",
                "PWM actuation control for DC motors & servo positioning",
                "Digital tilt-switch telemetry & inversion state detection",
                "GPIO hardware state signaling & deterministic interrupt handling",
            ],
        },
        security: Security {
            offensive_labs: &[
                "Penetration testing & vulnerability assessment in isolated virtualised labs",
                "Linux privilege escalation, network enumeration & post exploitation",
            ],
            cryptography: &[
                "End-to-end TLS certificate lifecycle management",
                "Symmetric/asymmetric cipher implementation & cryptographic hashing",
            ],
        },
    }
}
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
            .name   = "friction",
            .lang   = "Rust",
            .desc   = "Custom Linux shell (piping, redirection, job control)",
            .status = STATUS_WRAPPING_UP
        },
        {
            .name   = "linux-c-core-utils",
            .lang   = "C",
            .desc   = "Reimplementing standard Linux GNU coreutils from scratch",
            .status = STATUS_ACTIVE
        },
        {
            .name   = "linux-rust-core-utils",
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

---

### `$ man kforkernel`

```text
KFORKERNEL(1)               Candidate Manual               KFORKERNEL(1)

NAME
       kforkernel - Systems, Embedded, Linux & Network Infrastructure Engineer

SYNOPSIS
       kforkernel [--hire] [--intern] [--freelance] [--interview] [--jobseeker]

DESCRIPTION
       Motivated systems programmer with hands-on experience in C, Rust,
       systems administration, networking, and bare-metal hardware programming.
       Proven ability to learn complex architectures from the ground up—
       demonstrated by writing a shell, Linux coreutils from scratch,
       and studying OS kernel internals.

OPTIONS
       --hire
              Available for Systems, Embedded, Systems Administration,
              Networking, Help Desk/IT Support & Linux Infrastructure roles.

       --intern
              Open to Systems Engineering, Kernel, Firmware,
              Cybersecurity, IT/Tech Support Internships/Apprenticeships.

       --interview
              Ready for technical screenings, live C/Rust coding, and
              system architecture discussions.

       --location
              Based in London (UK), available for in person, hybrid and remote jobs.

KEY STRENGTHS
       * Memory-safe & low-level programming (Rust, C, C++)
       * Linux system administration (RHCSA-level) & networking (CCNA-level)
       * Microcontroller firmware, debugging, and hardware prototyping
       * Self-directed problem solver who reads specs and datasheets
       * Strong passion for IT and learning new things
       * Technical curiosity and creativity, constantly building, tinkering, and exploring new tools
       * Can work under pressure and in limited time constraints
       * Problem isolation and analytical thinking 

FILES
       /usr/bin/projects.rs
              Completed projects and builds.

       ~/projects/roadmap.c
              Source-level overview of active systems and Linux builds.

       ~/arch/x86_64/contact.asm
              Direct contact handles for recruiters and hiring teams.

EXIT STATUS
       0      Ready to onboard and ship production code and administer systems.

SEE ALSO
       contact.asm(7), resume(1), fortune(6)
```

---

### `$ cat ~/arch/x86_64/contact.asm`

```nasm
section .rodata
    ; Direct interfaces for recruiters & engineering teams
    email    db "contact@kforkernel.com", 0
    matrix   db "@kforkernel:matrix.org", 0
    website  db "https://kforkernel.com  [STATUS: 503 - Under Development]", 0

section .text
    global _connect

_connect:
    lea  rdi, [rel email]       ; Preferred for job inquiries & interviews
    lea  rsi, [rel matrix]      ; Real-time chat (Element)
    lea  rdx, [rel website]     ; Portfolio & kernel notes (WIP)
    ret
```

---

```text
kforkernel@localhost:~\$ fortune -s
"Some motivating quote or something" — kforkernel ...probably

kforkernel@localhost:~\$ cat << "EOF" >> ~/.bash_logout
   ____  _   _ ____   ___    ______   _______ 
  / ___|| | | |  _ \ / _ \  | __ ) \ / / ____|
  \___ \| | | | | | | | | | |  _ \\ V /|  _|  
   ___) | |_| | |_| | |_| | | |_) || | | |___ 
  |____/ \___/|____/ \___/  |____/ |_| |_____|

EOF

kforkernel@localhost:~\$ █
```

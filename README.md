<div align="center">

```ansi
 [1;31mkforkernel@localhost:~$ [0m  [1;32mneofetch --custom [0m

 [1;32m
       .--.                                     /\       |==|
      |    |     USER:    kforkernel           /  \      |==|
      |    |     ROLE:    Systems Programmer   \  /      |==|
     //   \ \    OS:      Linux / FreeBSD       \/       |  |
    (|     | )   KERNEL:  Ring 0 Tinkerer       ||       |  |
   /'\_   _/`\   NET:     CCNA / Packet Filter  ||       |__|
   \___)=(___/   ADMIN:   RHCSA / ZFS / Jails   ||      [____] [0m
```

**`[ SYSTEMS PROGRAMMER ]` • `[ OS & KERNEL DEV ]` • `[ NETWORK ENGINEER ]` • `[ *NIX SYSADMIN ]`**

</div>

---

### `0x01 // SYSTEM_OVERVIEW`

```ansi
 [1;31mkforkernel@localhost:~\$ [0m  [1;32m./whoami --verbose
Exploring how computers work from bare-metal silicon and raw Ethernet frames 
all the way up to userspace daemons. Focused on operating system architecture, 
low-level C/Rust, and hardened Linux/BSD network infrastructure. [0m
```

---

### `0x02 // INFRASTRUCTURE_&_STACK`

#### **`[ KERNEL & LOW-LEVEL ]`**
* **OS Development:** Custom kernel design, memory management (paging/allocators), syscalls, schedulers, Ring 0 internals
* **Systems Languages:** `Rust`, `C`, `C++`, `POSIX Shell (sh/bash/zsh)`, `x86_64 Assembly`, `Python`, `SQL`
* **Embedded & Hardware:** MCU firmware, bare-metal prototyping, circuit & PCB design

#### **`[ LINUX & BSD ADMINISTRATION ]`**
* **Linux (RHCSA-level):** `systemd`, `SELinux`, `LVM`, `Podman / KVM`, `iptables / nftables`, RHEL / Debian / Arch
* **BSD Internals:** FreeBSD `Jails`, `ZFS` storage pools, `rc.d`, `ports`, OpenBSD `pf` (Packet Filter) & `doas`

#### **`[ NETWORKING & TOPOLOGY ]`**

```ansi
 [1;31mkforkernel@localhost:~\$ [0m  [1;32mtraceroute -n core.backbone.local

    [WAN / ISP]
         |
   .-----+-----.

   |  BSD/pf   |  --> Stateful Firewall / WireGuard VPN (UDP 51820)
   '-----+-----'
         |  (802.1Q Trunk / BGP & OSPF)
   .-----+-----.

   |  L3 Core  |  --> VLAN Segmentation / Routing / Switching (CCNA)
   '-----+-----'
      /     \
 [Linux]  [FreeBSD]  --> KVM Hypervisor & ZFS Jail Host [0m
```

---

### `0x03 // ACTIVE_DIRECTORIES`

```ansi
 [1;31mkforkernel@localhost:~\$ [0m  [1;32mls -la ~/workspace/
drwxr-xr-x  2 kforkernel wheel  512 Nov 22 05:22 .
drwxr-xr-x 14 kforkernel wheel  512 Nov 22 05:22 ..
-rw-r--r--  1 kforkernel wheel  512 Nov 22 05:22 custom_kernel.c     # [IN PROGRESS] Bootloader & memory paging
-rw-r--r--  1 kforkernel wheel  512 Nov 22 05:22 net_packet_lab.rs   # Raw socket & TCP/IP stack experiments
-rw-r--r--  1 kforkernel wheel  512 Nov 22 05:22 bsd_router.conf     # pf.conf rulesets, CARP failover & WireGuard
-rw-r--r--  1 kforkernel wheel  512 Nov 22 05:22 mcu_firmware.asm    # Bare-metal microcontroller register control [0m
```

---

<div align="center">

```ansi
 [1;31mkforkernel@localhost:~\$ [0m  [1;32mfortune -s
"Talk is cheap. Show me the code." — Linus Torvalds
"The power to serve." — FreeBSD [0m

 [1;31mkforkernel@localhost:~\$ [0m  [1;32m█ [0m
```

</div>

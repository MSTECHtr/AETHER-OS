# Aether OS

**The Unhackable Linux Server**

Aether OS is a radically hardened, privacy‑centric Linux distribution built on Debian 12.  
No desktop, only CLI. SSH protected by physical USB key.

## Features
- Kernel hardening: module lockdown, ASLR, ptrace restrictions
- Mandatory USB key for SSH access
- AppArmor enforced
- nftables firewall (only port 2222)
- File integrity (AIDE) and audit (auditd)
- Auto security updates
- Configuration tool: `aether-config`

## Build ISO
1. Set up Debian 12 chroot at `/home/mamura/chroot` with `debootstrap`
2. Copy the files from this repo into the chroot
3. Run `sudo ./build-iso.sh` (provided in `scripts/`)

## Default Login
Username: `aether`  
Password: `147147`  
Change after first boot.

## License
GNU GPL v3.0

# Homelab Documentation

> Personal homelab docs — includes older notes migrated from elsewhere. Updated every two weeks.

---

## Table of Contents

- [About](#about)
- [Hardware](#hardware)
- [Weekly Log](#weekly-log)
  - [Week 1 — January 22](#week-1--january-22)
  - [Week 2 — January 29](#week-2--january-29)
  - [Week 3 — February 5](#week-3--february-5)

---

## About

This repo documents the setup, configuration, and ongoing maintenance of my personal homelab. Some entries predate the creation of this repository and have been migrated here for consolidation. New entries are added on a biweekly basis.

**Base OS:** Red Hat  
**Primary Machine:** Mini PC *(update with model/specs)*

---

## Hardware

| Component | Details |
|-----------|---------|
| Primary Machine | Mini PC *(update with model)* |
| Installation Media | Bootable USB flash drives |

---

## Weekly Log

### Week 1 — January 22

#### Overview
First week of the homelab. Acquired a mini PC as the base machine, evaluated Linux distributions, and created bootable USB installation media from scratch.

#### OS Selection

| Distro | Status | Notes |
|--------|--------|-------|
| Ubuntu | Abandoned | Ran into download issues, could not complete installation |
| Red Hat | Adopted | Installed successfully — selected as the base OS for the entire homelab |

Red Hat will serve as the foundation going forward.

#### Bootable Flash Drives

Created bootable Linux USB drives from scratch using spare flash drives for use as installation media and recovery tools.

**Steps taken:**
1. Downloaded the target Linux ISO
2. Flashed the ISO to a USB drive *(update with tool used — e.g., Balena Etcher, `dd`, Rufus)*
3. Verified the drive booted correctly before use

#### Lessons Learned
- Ubuntu download issues are worth investigating later (possible causes: corrupted ISO, network/mirror problem)
- Red Hat confirmed stable on this hardware
- Physical bootable drives are handy for quick installs and recovery

#### Next Steps
- [ ] Document mini PC specs in full
- [ ] Begin Red Hat post-install configuration
- [ ] Set up networking and remote access

---

### Week 2 — January 29

#### Overview
Installed Oracle VirtualBox on the Red Hat mini PC to enable virtualization. The intention is to run Ubuntu Linux Server inside a VM, allowing server processes to operate in the background isolated from the host OS.

#### Virtualization Setup

| Software | Guest OS | Status |
|----------|----------|--------|
| Oracle VirtualBox | Ubuntu Linux Server | Installed |

#### Purpose
Rather than running server processes directly on the Red Hat host, Ubuntu Server will run inside a VirtualBox VM. This keeps the host clean and allows the server environment to be managed, snapshotted, or rebuilt independently.

#### Next Steps
- [ ] Create and configure the Ubuntu Server VM
- [ ] Install Ubuntu Linux Server ISO in VirtualBox
- [ ] Configure VM networking
- [ ] Begin setting up server processes inside the VM

---

### Week 3 — February 5

#### Overview
Created a virtual machine running Oracle Linux inside VirtualBox. Ran into issues during both installation and storage provisioning, but resolved them through troubleshooting. The VM is now fully operational.

#### Issues & Resolutions

| Issue | Resolution |
|-------|------------|
| Installation problems during VM setup | Resolved through troubleshooting *(document specific fix)* |
| Problems provisioning storage space for the VM | Resolved through troubleshooting *(document specific fix)* |

#### Outcome
A working Oracle Linux virtual machine is up and running inside VirtualBox on the Red Hat host.

#### Next Steps
- [ ] Document the specific installation and provisioning fixes for future reference
- [ ] Begin configuring the Oracle Linux VM for its intended workload

---

*Last updated: February 5*

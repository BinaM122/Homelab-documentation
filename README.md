# Homelab Documentation

> Personal homelab docs — includes older notes migrated from elsewhere. Updated every two weeks.

---

## Table of Contents

- [About](#about)
- [Hardware](#hardware)
- [Weekly Log](#weekly-log)
  - [Week 1 — January 22](#week-1--january-22)

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

*Last updated: January 22*

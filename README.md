# XSEC

**XiangShan Security Ecosystem Chain**

Repository: <https://github.com/OpenXiangShan/XSEC.git>

---

## Overview

**XSEC** (pronounced **"X-Sec"** /eks-sek/) is the security ecosystem chain for the XiangShan processor. It spans the full stack from processor microarchitecture, on-chip interconnect, memory safety, and uncore security, to firmware, operating systems, virtualization, toolchains, and verification.

- **X** = XiangShan
- **S** = Security
- **E** = Ecosystem
- **C** = Chain

---

## Scope

XSEC covers the following areas:

| Area | Contents |
|------|----------|
| Processor Cores | XiangShan, NEMU, GEM5, Spike, QEMU |
| Memory Safety | Memory Encryption, IOPMP, IOMPT |
| Uncore Security | AIA, IOMMU, Debug, SCP |
| On-Chip Interconnect | NoC |
| Toolchains | GCC, LLVM |
| System Software | Linux, OpenSBI, KVM Tools |
| Verification | UVM, UCA, Formal, Fuzz, PoC, TPG, System Verification |

---

## Modules

### Processor & Simulation Models

| Module | Description |
|--------|-------------|
| **XiangShan** | High-performance RISC-V processor core |
| **NEMU** | Instruction-level simulator for functional verification and reference modeling |
| **GEM5** | Microarchitectural simulation for performance and security evaluation |
| **Spike** | Official RISC-V reference simulator for semantic comparison |
| **QEMU** | System-level emulation for running OpenSBI / Linux |

### Memory & I/O Security

| Module | Description |
|--------|-------------|
| **Memory Encryption** | Memory encryption for data confidentiality |
| **IOPMP** | I/O Physical Memory Protection against illegal DMA |
| **IOMPT** | I/O Memory Protection Table for fine-grained device memory access control |

### Uncore Security

| Module | Description |
|--------|-------------|
| **AIA** | RISC-V Advanced Interrupt Architecture with secure interrupt isolation |
| **IOMMU** | I/O Memory Management Unit for device address translation and isolation |
| **Debug** | Secure debug architecture and access control |
| **SCP** | System Control Processor for secure boot and power management |

### On-Chip Interconnect

| Module | Description |
|--------|-------------|
| **NoC** | Network-on-Chip with security domain isolation and access control |

### Toolchains

| Module | Description |
|--------|-------------|
| **GCC** | GNU toolchain with RISC-V security extension support |
| **LLVM** | LLVM toolchain with RISC-V security extension support |

### System Software

| Module | Description |
|--------|-------------|
| **Linux** | OS-level security mechanisms (page tables, privileges, isolation) |
| **OpenSBI** | Firmware-level secure boot and runtime services |
| **KVM Tools** | Virtualization tools for secure virtualization scenarios |

### Verification

| Module | Description |
|--------|-------------|
| **UVM** | Universal Verification Methodology for module-level and system-level verification |
| **UCA** | Microarchitectural checking and security property verification |
| **Formal** | Formal verification for proving security properties |
| **Fuzz** | Fuzz testing for discovering anomalies and vulnerabilities |
| **PoC** | Proof of Concept for validating security mechanism effectiveness |
| **TPG** | Test Pattern Generation for security-related coverage |
| **System Verification** | End-to-end system-level verification across hardware, firmware, OS, and virtualization |

---

## Repository Structure

```
XSEC/
├── xiangshan/            # XiangShan processor core
├── nemu/                 # NEMU simulator
├── gem5/                 # GEM5 simulation
├── spike/                # Spike reference model
├── qemu/                 # QEMU system emulation
├── memory-encryption/    # Memory encryption
├── iopmp/                # IOPMP
├── iompt/                # IOMPT
├── uncore/               # Uncore security
│   ├── aia/              # AIA interrupt architecture
│   ├── iommu/            # IOMMU
│   ├── debug/            # Secure debug
│   └── scp/              # SCP
├── noc/                  # NoC
├── gcc/                  # GCC toolchain
├── llvm/                 # LLVM toolchain
├── linux/                # Linux
├── opensbi/              # OpenSBI
├── kvm-tools/            # KVM tools
├── verification/         # Verification
│   ├── uvm/
│   ├── uca/
│   ├── formal/
│   ├── fuzz/
│   ├── poc/
│   ├── tpg/
│   └── system/           # System verification
└── docs/                 # Documentation
```

---

## Goals

- Build the security ecosystem chain for the XiangShan processor from hardware to software
- Cover memory, uncore, interconnect, firmware, OS, virtualization, and toolchains
- Provide comprehensive verification: UVM, UCA, Formal, Fuzz, PoC, TPG, System Verification
- Form a reproducible, extensible, and verifiable security ecosystem

---

## Getting Started

```bash
git clone https://github.com/OpenXiangShan/XSEC.git
cd XSEC
```

For build and run instructions, refer to the README in each subdirectory.

---

## License

See the LICENSE file in each subdirectory.

---

## Acknowledgments

Thanks to the OpenXiangShan community and all contributors.

---

**XSEC — XiangShan Security Ecosystem Chain**

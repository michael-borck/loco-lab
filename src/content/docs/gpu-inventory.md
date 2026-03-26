---
title: "GPU Inventory"
---

Every GPU currently in the LocoLab project, organised by machine. Cards move between machines as experiments require -- this is the current assignment.

For specifications, acquisition guidance, and generation-level analysis see the [Nvidia GPU Reference](nvidia-gpu-reference).

---

## Colmena

The benchmark lab. An 8-GPU enclosed mining rig running LocoBench. Cards here are chosen as **floor representatives** -- the worst card per VRAM tier, so results are honest baselines. Also hosts adapter training workloads and multi-GPU experiments.

| Card | VRAM | Bandwidth | Tier Role |
|------|------|-----------|-----------|
| GTX 1060 6 GB (x3) | 6 GB | 192 GB/s | Floor of 6 GB tier (Pascal, no Tensor Cores) |
| RTX 2060 Super (x3) | 8 GB | 448 GB/s | Floor of 8 GB Turing tier (Tensor Cores). Three cards for multi-GPU and result consistency validation |
| Tesla P100 | 16 GB | 732 GB/s | Adapter training (PEFT only, no Tensor Cores). High bandwidth for 16 GB |
| RTX 3090 | 24 GB | 936 GB/s | Reference ceiling -- 24 GB scaling data, not primary workload |
| RTX 4060 Ti | 16 GB | 288 GB/s | Floor of 16 GB consumer tier -- documents the bandwidth penalty |
| Tesla V100 | 32 GB | 900 GB/s | 32 GB server tier (Volta, HBM2, Tensor Cores) |

---

## Tortuga

Swappable bench cards. Cards rotate through Tortuga to fill out LocoBench tier coverage, particularly the older Maxwell and Pascal generations.

| Card | VRAM | Bandwidth | Tier Role |
|------|------|-----------|-----------|
| GTX 950 | 2 GB | 105 GB/s | Floor of 2 GB tier (Maxwell). TinyLlama 1.1B only. Quality cliff reference point |
| GTX 960 | 4 GB | 112 GB/s | Floor of 4 GB tier (Maxwell, Compute 5.2, Ollama only) |
| GTX 980 Ti | 6 GB | 336 GB/s | Floor of 6 GB Maxwell tier (Ollama only) |
| GTX Titan X | 12 GB | 336 GB/s | Floor of 12 GB Maxwell tier (Ollama only) |
| GTX 1050 Ti | 4 GB | 112 GB/s | Floor of 4 GB tier (Pascal, no Tensor Cores) |
| GTX 1060 3 GB | 3 GB | 192 GB/s | Floor of 3 GB tier (Pascal). Quality cliff reference point |
| GTX 1060 6 GB | 6 GB | 192 GB/s | Additional 6 GB Pascal card |

---

## Pulpo

Onboarding. New cards being integrated into the lab.

| Card | VRAM | Bandwidth | Tier Role |
|------|------|-----------|-----------|
| GTX 1070 | 8 GB | 256 GB/s | 8 GB Pascal (no Tensor Cores). Bandwidth comparison against 2060 Super |
| RTX 3050 | 8 GB | 224 GB/s | 8 GB Ampere. Lowest bandwidth Tensor Core card in the 8 GB tier |
| RTX 3060 AORUS Elite | 12 GB | 360 GB/s | Floor of 12 GB tier (Ampere, Tensor Cores) |

---

## Cerebro

Home machine. Not part of the on-campus lab infrastructure. Benchmarks run here as needed.

| Card | VRAM | Bandwidth | Tier Role |
|------|------|-----------|-----------|
| RTX 2060 Super (x2) | 8 GB | 448 GB/s | Development and testing |
| Tesla V100 | 16 GB | 900 GB/s | 16 GB server tier (Volta, HBM2, Tensor Cores). PCIe adapter with passive heatsink |

---

## Hormiga

Low-profile / office deployment.

| Card | VRAM | Bandwidth | Tier Role |
|------|------|-----------|-----------|
| GTX 1050 Ti LP | 4 GB | 112 GB/s | Low-profile 4 GB card for constrained chassis |

---

## Unassigned

| Card | VRAM | Bandwidth | Notes |
|------|------|-----------|-------|
| GTX 1650 OC LP | 4 GB | 128 GB/s | Turing, no Tensor Cores. Low-profile. No current assignment |

---

## Summary

| Machine | Cards | Primary Role |
|---------|-------|-------------|
| Colmena | 12 | Benchmarking, adapter training, multi-GPU |
| Tortuga | 7 | Swappable tier cards for LocoBench coverage |
| Pulpo | 3 | Onboarding new hardware |
| Cerebro | 3 | Development and benchmarking (home) |
| Hormiga | 1 | Office deployment |
| Unassigned | 1 | — |
| **Total** | **27** | |

---

*For GPU generation details and acquisition guidance see [Nvidia GPU Reference](nvidia-gpu-reference). For benchmarking methodology see the loco-bench documentation.*

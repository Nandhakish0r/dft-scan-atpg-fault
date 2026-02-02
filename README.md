# DFT Scan Chain Insertion and ATPG using Fault (Open-Source)

This repository presents a **complete RTL-to-ATPG Design for Testability (DFT) flow**
implemented using **open-source EDA tools**.  
The flow includes **synthesis, scan chain insertion, scan cut, ATPG, and fault coverage analysis**.

The design under test is a **4-bit synchronous counter**, implemented using the
**osu035 standard cell library** and tested using the **Fault DFT tool**.

---

## 📘 Course Information
- **Course:** ECS324 – VLSI Testing
- **Experiment:** Scan Insertion and ATPG using Fault
- **Author:** Nandakishor PB
- **Platform:** Ubuntu Linux
- **Tools:** OSS CAD Suite, Yosys, Fault

---

## 🎯 Objectives
- Convert RTL design into gate-level netlist
- Insert scan chains automatically
- Prepare sequential design for ATPG
- Generate and compact test vectors
- Measure fault coverage
- Understand all intermediate files generated

---

## 🛠 Tools & Libraries Used
- **OSS CAD Suite**
- **Yosys** – RTL synthesis
- **Fault** – Scan insertion, scan cut, ATPG
- **osu035 Standard Cell Library**
  - Liberty file (`.lib`)
  - Cell models (`.v`)

---

## 📂 Repository Structure

├──doc

├── screenshots

├── counter.v # RTL design

├── synth.ys # Yosys synthesis script

├── counter_trial.v # Synthesized gate-level netlist

├── oscu35_standandarcells.lib # Standard cell liberty file

├── osu035_stdcells.v # Cell models for ATPG

├── counter_scan1.v # Scan-inserted netlist

├── counter_scan_cut.v # Scan-cut netlist

├── patterns.tv.json # Final ATPG test vectors

├── patterns.raw_tv.json # Raw test vectors

├── coverage.yml # Fault coverage report

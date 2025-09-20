# 🚀 VSD Program: Open-Source VLSI Tool Setup

Welcome to my repository for the **VLSI System Design (VSD) Program**. This project documents the foundational work of setting up a robust, open-source development environment for VLSI design, covering key tools for synthesis and simulation.

This repository serves as a guide and record of the essential tools and configurations used throughout the program.

-----

## 🎯 System and Virtual Machine Configuration

For optimal performance, the development environment was configured on a Virtual Machine (VM) with the following specifications:

  * **Operating System:** 🐧 Ubuntu 20.04+ (64-bit)
  * **RAM:** 💾 6GB
  * **Storage:** 💿 50GB HDD
  * **vCPUs:** ⚡ 4

-----

## ⚙ Tool Installation and Overview

This project utilizes a suite of industry-standard, open-source tools to support a complete VLSI design flow. All tools were installed and verified on the specified VM.

| Tool | Primary Use | Installation Method |
| :--- | :--- | :--- |
| **Yosys** | RTL Synthesis | Compiled from source |
| **Icarus Verilog** | Verilog Simulation | Package Manager (`apt`) |
| **GTKWave** | Waveform Analysis | Package Manager (`apt`) |

-----

### 1\. Yosys - RTL Synthesis

Yosys is a comprehensive framework for Verilog RTL synthesis. It's a cornerstone tool for transforming high-level Verilog code into gate-level netlists. The installation involved cloning the repository, installing dependencies, and compiling the source.

<br>

**Installation Commands:**

```bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt-get install build-essential clang bison flex libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev
make
sudo make install
```

-----

### 2\. Icarus Verilog (Iverilog) - Verilog Simulator

Icarus Verilog is a powerful Verilog compiler and simulator used for functional verification of digital designs.

<br>

**Installation Command:**

```bash
sudo apt-get install iverilog
```

-----

### 3\. GTKWave - Waveform Viewer

GTKWave is a waveform viewer that allows for the visualization and analysis of simulation results, which is critical for debugging digital circuits.

<br>

**Installation Command:**

```bash
sudo apt-get install gtkwave
```

-----

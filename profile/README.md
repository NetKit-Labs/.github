# NetKit Labs

**Established NetKit Labs to develop embedded C/C++ software for MCU and embedded Linux platforms.**

[Website](https://netkit-labs.github.io/) · [Repositories](https://github.com/orgs/NetKit-Labs/repositories) · [Project guide](#featured-projects) · [Explore by topic](#explore-by-topic)

Our work spans bare-metal and Zephyr RTOS firmware on Arm Cortex-M/A, embedded Linux, audio DSP, TinyML inference runtimes, and FPGA-based neural network acceleration. The projects connect embedded software infrastructure with keyword spotting, speech commands, and efficient inference on microcontrollers, MPU hosts, and programmable logic.

---

## Focus Areas

* Embedded Software Development (C/C++)
* Arm Cortex-M/A Firmware
* Bare-Metal & Zephyr RTOS Systems
* Embedded Linux
* Audio DSP & Keyword Spotting
* Edge AI / TinyML
* Neural Network Inference Runtimes
* FPGA AI Accelerators
* Hardware/Software Co-Design

## Explore by Topic

| Area | Repository topics |
| --- | --- |
| Embedded C/C++ | [C++](https://github.com/search?q=org%3ANetKit-Labs+topic%3Acpp&type=repositories) · [C23](https://github.com/search?q=org%3ANetKit-Labs+topic%3Ac23&type=repositories) · [Embedded systems](https://github.com/search?q=org%3ANetKit-Labs+topic%3Aembedded-systems&type=repositories) |
| Arm firmware and bare metal | [Arm Cortex-M](https://github.com/search?q=org%3ANetKit-Labs+topic%3Acortex-m&type=repositories) · [Arm Cortex-A](https://github.com/search?q=org%3ANetKit-Labs+topic%3Acortex-a&type=repositories) · [Firmware](https://github.com/search?q=org%3ANetKit-Labs+topic%3Afirmware&type=repositories) · [Bare metal](https://github.com/search?q=org%3ANetKit-Labs+topic%3Abare-metal&type=repositories) |
| RTOS and real-time systems | [Zephyr](https://github.com/search?q=org%3ANetKit-Labs+topic%3Azephyr&type=repositories) · [RTOS](https://github.com/search?q=org%3ANetKit-Labs+topic%3Artos&type=repositories) · [Real-time](https://github.com/search?q=org%3ANetKit-Labs+topic%3Areal-time&type=repositories) |
| Embedded Linux and MPUs | [Embedded Linux](https://github.com/search?q=org%3ANetKit-Labs+topic%3Aembedded-linux&type=repositories) · [MPUs](https://github.com/search?q=org%3ANetKit-Labs+topic%3Ampu&type=repositories) |
| Audio and speech | [Audio processing](https://github.com/search?q=org%3ANetKit-Labs+topic%3Aaudio-processing&type=repositories) · [Keyword spotting](https://github.com/search?q=org%3ANetKit-Labs+topic%3Akeyword-spotting&type=repositories) · [Speech commands](https://github.com/search?q=org%3ANetKit-Labs+topic%3Aspeech-commands&type=repositories) |
| Edge AI and inference | [Edge AI](https://github.com/search?q=org%3ANetKit-Labs+topic%3Aedge-ai&type=repositories) · [TinyML](https://github.com/search?q=org%3ANetKit-Labs+topic%3Atinyml&type=repositories) · [Inference](https://github.com/search?q=org%3ANetKit-Labs+topic%3Ainference&type=repositories) · [Neural networks](https://github.com/search?q=org%3ANetKit-Labs+topic%3Aneural-network&type=repositories) |
| Memory and containers | [Memory management](https://github.com/search?q=org%3ANetKit-Labs+topic%3Amemory-management&type=repositories) · [Lock-free utilities](https://github.com/search?q=org%3ANetKit-Labs+topic%3Alock-free&type=repositories) · [Containers](https://github.com/search?q=org%3ANetKit-Labs+topic%3Acontainers&type=repositories) · [Static allocation](https://github.com/search?q=org%3ANetKit-Labs+topic%3Astatic-allocation&type=repositories) |
| FPGA and hardware acceleration | [FPGA](https://github.com/search?q=org%3ANetKit-Labs+topic%3Afpga&type=repositories) · [SystemVerilog](https://github.com/search?q=org%3ANetKit-Labs+topic%3Asystemverilog&type=repositories) · [NPU](https://github.com/search?q=org%3ANetKit-Labs+topic%3Anpu&type=repositories) · [Systolic arrays](https://github.com/search?q=org%3ANetKit-Labs+topic%3Asystolic-array&type=repositories) · [Zynq](https://github.com/search?q=org%3ANetKit-Labs+topic%3Azynq&type=repositories) |

---

## Featured Projects

### KWSKit — Real-time Keyword Spotting with Zephyr

Built a C++20 keyword-spotting application for the Arduino Nano 33 BLE Sense (nRF52840 / Arm Cortex-M4F), using Zephyr RTOS, CMSIS-DSP features, and int8 TensorFlow Lite Micro inference. Continuous 16 kHz microphone audio drives voice-triggered LED control.

Repository: [NetKit-Labs/kwskit](https://github.com/NetKit-Labs/kwskit)

Highlights include:

* Separate thread contexts for PDM capture, audio processing, keyword control, and telemetry
* Fixed application buffers, thread stacks, and a 64 KiB inference arena
* Nonblocking score delivery, bounded audio batches, and stale-result rejection
* Unit and regression tests, firmware CI, and recorded hardware validation
* Spoken-keyword operation and physical LED toggling verified on the Nano

---

### NetKit — Neural Network Inference Runtime for MCU and Embedded Linux

NetKit is a C++26 inference runtime with C++ and C23 APIs for MCU and embedded Linux targets. Float32 and INT8 paths support resource-constrained deployment, with optimized backends including CMSIS-NN, ESP-NN, NMSIS-NN, and XNNPACK.

Repository: [NetKit-Labs/netkit](https://github.com/NetKit-Labs/netkit)

Highlights include:

* C++ and C APIs over a shared runtime
* Float32 and INT8 quantized inference
* Explicit memory planning for embedded deployment
* Optimized kernels for Arm, Espressif, RISC-V, and host CPUs
* Peer benchmarks against established inference runtimes

---

### MemKit — Embedded Container Library for MCU and MPU Environments

MemKit is an embedded C++26 container library with C++ and C23 APIs over shared implementations, designed for bare-metal MCUs, RTOS firmware, and embedded Linux MPUs.

Repository: [NetKit-Labs/memkit](https://github.com/NetKit-Labs/memkit)

Features include:

* Ring buffers, maps, pools, and other embedded containers
* C++ lock-free queues and double buffering for task/ISR handoff
* Static and arena storage for MCU firmware
* Heap and virtual-memory arena backing for MPU hosts
* C and C++ APIs over shared container cores

---

### NPUKit — FPGA Neural Network Accelerator

NPUKit is a SystemVerilog INT8 neural network accelerator for the PYNQ-Z2 (AMD-Xilinx Zynq-7020). An 8×8 output-stationary systolic array performs matrix multiplication, with AXI control, DMA tile transfers, and transformer operations split between FPGA fabric and Python host software. Speech-command experiments explore embedded workloads on top of the accelerator.

Repository: [NetKit-Labs/npukit](https://github.com/NetKit-Labs/npukit)

Highlights include:

* 8×8 INT8 systolic GEMM array
* AXI4-Lite control and AXI DMA tile I/O
* On-fabric residual, GELU, RMSNorm, and Softmax operations
* Python host software for board control and inference
* Hardware/software co-design with speech-command workloads

---

## Technologies

**Languages**

* C
* C++
* SystemVerilog
* Python

**Platforms**

* Arm Cortex-M
* Arm Cortex-A
* Zephyr RTOS
* Embedded Linux
* AMD-Xilinx Zynq SoCs
* FPGA

**Domains**

* Embedded Systems
* Audio DSP
* Keyword Spotting & Speech Commands
* Edge AI / TinyML
* Neural Network Acceleration

---

## Connect

**James Lavrenz**

Embedded Software Engineer | C/C++ | Embedded Linux | RTOS | Arm Cortex-M/A | Edge AI

[Website](https://netkit-labs.github.io/) · [GitHub](https://github.com/jameslavrenz) · [LinkedIn](https://www.linkedin.com/in/jameslavrenz)

For project questions and bug reports, use the issue tracker in the relevant repository: [KWSKit](https://github.com/NetKit-Labs/kwskit/issues), [NetKit](https://github.com/NetKit-Labs/netkit/issues), [MemKit](https://github.com/NetKit-Labs/memkit/issues), or [NPUKit](https://github.com/NetKit-Labs/npukit/issues).

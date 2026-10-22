# NetKit Labs

**Open-source Embedded Software • Edge AI • FPGA AI Acceleration**

NetKit Labs is an independent research and development initiative focused on embedded software, Edge AI, digital signal processing, and FPGA acceleration for resource-constrained intelligent systems.

Our work spans bare-metal and Zephyr RTOS firmware on ARM Cortex-M, embedded Linux, audio DSP, TinyML inference runtimes, and FPGA-based neural network acceleration. The projects connect embedded software infrastructure with keyword spotting, speech commands, and efficient inference on microcontrollers, MPU hosts, and programmable logic.

---

## Focus Areas

* Embedded Software Development (C/C++)
* ARM Cortex-M Firmware
* Bare-Metal & Zephyr RTOS Systems
* Embedded Linux
* Audio DSP & Keyword Spotting
* Edge AI / TinyML
* Neural Network Inference Runtimes
* FPGA AI Accelerators
* Hardware/Software Co-Design

---

## Featured Projects

### KWSKit — Real-time Keyword Spotting with Zephyr

Built a C++20 keyword-spotting application for the Arduino Nano 33 BLE Sense (nRF52840 / ARM Cortex-M4F), using Zephyr RTOS, CMSIS-DSP features, and int8 TensorFlow Lite Micro inference. Continuous 16 kHz microphone audio drives voice-triggered LED control.

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

* ARM Cortex-M
* Zephyr RTOS
* Embedded Linux
* AMD-Xilinx Zynq SoCs
* FPGA

**Domains**

* Embedded Systems
* Audio DSP
* Keyword Spotting & Speech Commands
* TinyML
* Edge AI
* Neural Network Acceleration

---

## Mission

NetKit Labs develops practical open-source infrastructure for embedded systems and efficient AI inference. The focus is on reusable C/C++ libraries, Zephyr firmware, audio processing, and FPGA acceleration, supported by tests, benchmarks, and documented hardware results.

---

## Connect

**James Lavrenz**

Principal Embedded Software Engineer (Edge AI/TinyML) | Embedded AI | FPGA AI Acceleration

LinkedIn: https://www.linkedin.com/in/jameslavrenz

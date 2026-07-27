# NetKit Labs

**Open-source Embedded Software • Edge AI • FPGA AI Acceleration**

NetKit Labs is an independent research and development initiative focused on embedded software, Edge AI, digital signal processing, and FPGA acceleration for resource-constrained intelligent systems.

Our work spans bare-metal and RTOS firmware on ARM Cortex-M, embedded Linux, real-time DSP, TinyML inference runtimes, and FPGA-based neural network acceleration — practical open-source tools from microcontrollers to embedded Linux and programmable logic.

---

## Focus Areas

* Embedded Software Development (C/C++)
* ARM Cortex-M Firmware
* Bare-Metal & RTOS Systems
* Embedded Linux
* Digital Signal Processing (DSP)
* Edge AI / TinyML
* Neural Network Inference Runtimes
* FPGA AI Accelerators
* Hardware/Software Co-Design

---

## Featured Projects

### NetKit — Neural Network Inference Runtime for MCU and Embedded Linux

Built and open-sourced NetKit, a custom C++ inference runtime for MCU and embedded Linux targets, with optimized INT8 inference kernels achieving up to **10×** the performance of TensorFlow Lite for Microcontrollers (TFLM) reference implementations on selected operators. Float32 and INT8 paths are peer-benched across Arm MCU/MPU, Espressif, RISC-V, and host CPU backends (CMSIS-NN, ESP-NN, NMSIS-NN, XNNPACK).

Repository: [NetKit-Labs/netkit](https://github.com/NetKit-Labs/netkit)

Highlights include:

* Portable C++ implementation
* INT8 quantized inference
* Deterministic memory management
* Resource-constrained deployment
* Optimized inference kernels
* Up to **10× faster** than TensorFlow Lite for Microcontrollers (TFLM) reference kernels on selected operators

---

### MemKit — Embedded Container Library for MCU and MPU Environments

Open-sourced MemKit, an embedded systems container library written in C++ with native C and C++ APIs over shared implementations, designed specifically for resource-constrained MCU and MPU environments with predictable static, arena, and optional heap-backed storage.

Repository: [NetKit-Labs/memkit](https://github.com/NetKit-Labs/memkit)

Features include:

* STL-inspired interfaces
* Predictable memory usage
* Native C and C++ APIs
* No dynamic allocation requirements during runtime
* Designed for real-time embedded applications

---

### NpuKit — FPGA Neural Network Accelerator

Designed and implemented an FPGA-based INT8 neural network accelerator in SystemVerilog featuring a streaming output-stationary systolic-array architecture for matrix multiplication, enabling quantized Vision Transformer inference on an AMD-Xilinx Zynq-7000 SoC.

Repository: [NetKit-Labs/npukit](https://github.com/NetKit-Labs/npukit)

Highlights include:

* Output-stationary systolic-array architecture
* Streaming matrix multiplication engine
* Quantized neural network acceleration (INT8)
* AMD-Xilinx Zynq-7000 implementation
* Hardware/software co-design for embedded AI systems
* Host-scheduled tiny-ViT on MNIST with MCU-class DS-CNN peer benchmarks

---

## Technologies

**Languages**

* C
* C++
* SystemVerilog
* Python

**Platforms**

* ARM Cortex-M
* Embedded Linux
* AMD-Xilinx Zynq SoCs
* FPGA

**Domains**

* Embedded Systems
* DSP
* TinyML
* Edge AI
* Computer Vision
* Neural Network Acceleration

---

## Mission

NetKit Labs exists to advance open-source Embedded AI by developing practical software infrastructure and hardware acceleration techniques that bridge embedded systems and modern machine learning.

The long-term vision is to provide a complete software-to-silicon ecosystem for efficient AI inference on resource-constrained devices.

---

## Connect

**James Lavrenz**

Principal Embedded Software Engineer (Edge AI/TinyML) | Embedded AI | FPGA AI Acceleration

LinkedIn: https://www.linkedin.com/in/jameslavrenz

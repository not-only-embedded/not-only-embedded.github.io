---
layout: home
title: diff
---

**_diff_** is a **C++ dependency injection framework** designed for **embedded systems**, enabling modular, maintainable, and reusable software architecture assembled from independent components guided by **JSON configuration files**.  

### component model
- **regular components** - single C++ classes encapsulating specific functionality
- **interface components** - abstract classes defining functionality contracts, delivered as **header-only** libraries
- **modules** - physical representations shipped as **static, dynamic, or header-only** libraries
- independently versioned, built, and tested per module
- short **dependency chains** - components depend only on interfaces

### json topology
- **JSON files** describe component hierarchies, instances, and dependencies
- components instantiated and configured **at application startup**
- **runtime reconfiguration** without rebuilding
- multiple instances of the same component with **different configurations**
- automated component selection during **CI/CD pipeline** assembly

### platform support
- **Linux** (x86, ARM, RISC-V - gcc, clang)
- **Windows** (x86-32/64 - msvc)
- **QNX Neutrino** (ARM - qcc) & **VxWorks** (x86 - gcc)
- **bare-metal** (ARM - armcl, RISC-V - gcc)
- applicable to **SoCs, microcontrollers,** and **PLC controllers**

### development workflow
- **individual component testing** in isolation
- **integration testing** of component combinations
- off-the-shelf **component assembly** from reusable modules
- full **CI/CD pipeline** integration
- relies exclusively on **C++ standard library** - no external dependencies

### variants

<div class="variants" markdown="1">
**_diff first_**<br>
open-source variant, available on [GitHub](https://github.com/slawomir-niespodziany/diff)<br><br>
**_diff featured_**<br>commercial product offering greater flexibility with the support of additional tooling
</div>
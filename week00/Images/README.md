
# RISC-V SoC Tapeout Program VSD

## Tools Installation

#### <ins>All the instructions for installation of required tools can be found here:</ins>

### **System Requirements**
I have configured a **Virtual Machine (VM)** with the following specifications:

The link for Oracle Virtualbox : https://www.virtualbox.org/wiki/Downloads

<div align="center">

| **Specification** 💻    | **Details** 📋          |
|-----------------------|-----------------------|
| **Operating System** 🐧  | Ubuntu 20.04.3        |
| **RAM** 💾               | 5GB                   |
| **Storage** 💿           | 50GB HDD              |
| **vCPUs** ⚡             | 4                     |

</div>


---


### **TOOLS INSTALLATION **

#### <ins>**Yosys**</ins>
```bash
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ git submodule update --init --recursive
$ make 
$ sudo make install
```
![Alt Text](Images/yosys ss.jpeg)

#### <ins>**Iverilog**</ins>
```bash
$ sudo apt-get update
$ sudo apt-get install iverilog
```
![Alt Text](Images/iverilog.jpeg)

#### <ins>**gtkwave**</ins>
```bash
$ sudo apt-get update
$ sudo apt install gtkwave
```
![Alt Text](Images/gtk.jpeg)

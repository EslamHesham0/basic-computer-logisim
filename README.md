# Basic Computer Architecture - Logisim Implementation

## 📋 Project Overview

This project implements a **basic computer architecture** using Logisim, demonstrating fundamental concepts of computer organization and digital system design. The implementation follows the classic von Neumann architecture with a complete CPU, memory system, and control unit.

## 🏗️ Architecture Components

### Core Processing Unit
- **ALU (Arithmetic Logic Unit)**: Performs arithmetic and logical operations
  - Addition and Subtraction with carry/borrow
  - Logical operations (AND, OR, XOR, NOT)
  - Complement operations
  - 16-bit data path

### Register Set
- **AC (Accumulator)**: Primary register for arithmetic operations (16-bit)
- **PC (Program Counter)**: Stores the address of the next instruction (12-bit)
- **IR (Instruction Register)**: Holds the current instruction being executed (16-bit)
- **DR (Data Register)**: Temporary storage for data operations (16-bit)
- **AR (Address Register)**: Stores memory addresses for data access (12-bit)
- **TR (Temporary Register)**: Additional temporary storage (16-bit)

### Memory System
- **RAM**: Main memory with 12-bit addressing (4096 words)
- **16-bit data width** for instruction and data storage
- Separate address and data buses

### Control Unit
- **Instruction Decoder**: Decodes instruction opcodes
- **Timing Control**: Generates control signals for different timing phases (T0-T7)
- **Sequence Counter**: Manages instruction execution cycles
- **Control Logic**: Coordinates data flow between components

## 🔧 Features

### Instruction Execution
- **Fetch-Decode-Execute Cycle**: Complete implementation of the basic CPU cycle
- **Multiple Timing Phases**: T0 through T7 for complex instruction execution
- **Control Signal Generation**: Automated control of register loads, memory operations

### Data Path
- **16-bit Data Bus**: Handles instruction and data transfer
- **12-bit Address Bus**: Supports 4K memory addressing
- **Multiplexed Operations**: Efficient resource utilization

### ALU Operations
- Arithmetic: Addition, Subtraction
- Logical: AND, OR, XOR, Complement
- Flag Generation: Carry and overflow detection

## 🚀 Getting Started

### Prerequisites
- **Logisim 2.7.1** or compatible version
- Basic understanding of computer architecture concepts

### Installation & Usage
1. Download and install Logisim from [http://www.cburch.com/logisim/](http://www.cburch.com/logisim/)
2. Clone or download this repository
3. Open `basic-computer.circ` in Logisim
4. Use the simulation tools to:
   - Load programs into memory
   - Step through instruction execution
   - Observe register and memory changes
   - Test ALU operations

### Simulation Steps
1. **Load Program**: Use the RAM component to load instructions
2. **Reset System**: Initialize PC and control signals
3. **Run/Step**: Execute instructions manually or automatically
4. **Monitor**: Observe register contents and control signals

## 📊 Circuit Structure

### Main Circuit
- Central processing unit with interconnected components
- Memory interface and data bus system
- Control signal distribution network

### ALU Subcircuit
- Dedicated arithmetic and logic operations
- Input/output interfaces for AC and DR registers
- Operation selection through control signals

## 🎯 Learning Objectives

This implementation demonstrates:
- **Computer Organization**: How CPU components interact
- **Instruction Set Architecture**: Basic instruction execution
- **Digital Logic Design**: Gate-level implementation
- **Control Unit Design**: Sequencing and timing control
- **Memory Organization**: Address decoding and data access

## 🔬 Testing & Verification

### Test Scenarios
- Basic arithmetic operations (ADD, SUB)
- Logical operations (AND, OR, XOR)
- Memory load/store operations
- Program counter increment
- Instruction fetch and decode

### Debugging Features
- Visual signal tracing
- Register content monitoring
- Step-by-step execution
- Control signal observation

## 📚 Educational Value

Perfect for:
- **Computer Science Students**: Understanding CPU internals
- **Digital Logic Courses**: Practical circuit implementation
- **Computer Architecture Classes**: Hands-on learning
- **Self-Study**: Interactive exploration of computer systems

## 🛠️ Technical Specifications

- **Data Width**: 16 bits
- **Address Space**: 4096 words (12-bit addressing)
- **Register Count**: 6 primary registers
- **Instruction Phases**: 8 timing states (T0-T7)
- **ALU Operations**: 8 different operations
- **Clock Driven**: Synchronous operation

## 📖 Documentation

### Register Functions
- **AC**: Accumulates results of arithmetic operations
- **PC**: Points to next instruction location
- **IR**: Contains current instruction opcode and operand
- **DR**: Temporary data storage during operations
- **AR**: Memory addressing for load/store operations
- **TR**: Additional temporary storage as needed

### Control Signals
- **Load Signals**: Control register updates
- **Memory Signals**: Read/write operations
- **ALU Control**: Operation selection
- **Clock Signals**: Timing coordination

## 🤝 Contributing

This project serves as an educational reference. Improvements and optimizations are welcome:
- Enhanced instruction set
- Additional addressing modes
- Performance optimizations
- Documentation improvements


## 🏆 Acknowledgments

- Built using Logisim circuit simulation software
- Implements concepts from classic computer architecture textbooks
- Designed for educational demonstration of CPU fundamentals

---


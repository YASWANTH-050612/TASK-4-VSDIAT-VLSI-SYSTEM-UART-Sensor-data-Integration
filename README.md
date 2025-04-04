# TASK-4-VSDIAT-VLSI-SYSTEM-UART-Sensor-data-Integration

# UART Transmitter with Sensor Data Integration

## Objective

The objective of this task was to integrate a **UART transmitter** with a **sensor module** to enable the **FPGA** to transmit **real-time sensor data** to an external device via **UART communication**. This would allow for efficient data transfer from the FPGA to an external device for monitoring and control.

---

## Steps

### 1. Study the Existing Code

In this phase, I accessed the **uart_tx_sense** project from the **VSDSquadron_FM repository**. I carefully reviewed the **Verilog code** to understand the process of acquiring and transmitting sensor data through UART. The code describes how sensor data is read and then transmitted serially via UART.

**Key Points to Review:**
- The process of acquiring data from the sensor.
- The steps for transmitting this data via UART.
- The integration between the sensor module and the UART transmitter.

### 2. Design Documentation

#### Block Diagram

I developed a **block diagram** to depict how the **sensor module** is integrated with the **UART transmitter**. This diagram illustrates the flow of sensor data through the FPGA and shows how the data is processed and then transmitted via UART to an external device.

![Screenshot (2499)](https://github.com/user-attachments/assets/61eccb82-bd7b-4d59-94f2-3f1c501d86a7)


**Components Included in the Diagram:**
- **Sensor Module**: The input source that provides the sensor data.
- **FPGA Module**: The processing unit for the sensor data.
- **UART Transmitter**: The component responsible for sending the processed data to the external device.

#### Circuit Diagram

A **circuit diagram** was created to visualize the hardware setup. This diagram shows the connections between the **sensor** and the **FPGA** and the route the **FPGA’s UART TX pin** takes to connect to the receiving device (such as a PC or another UART-compatible device).

**Key Connections:**
- Sensor interface connected to the FPGA.
- FPGA UART TX pin connected to the receiving device.

### 3. Implementation

At this point, I have prepared the **circuit diagram** and **block diagram**, and the next step would involve implementing the hardware setup based on these diagrams. However, the actual hardware setup and bitstream loading onto the FPGA have not been completed yet due to some ongoing issues.

**Implementation Process (Planned):**
- Assemble the hardware setup as per the design.
- Load the synthesized Verilog code onto the FPGA using **Vivado**.

### 4. Testing and Verification

Although I have not yet completed the hardware setup, once the implementation is finished, I plan to simulate the sensor data (e.g., by adjusting environmental factors such as light or temperature). I will then monitor the transmitted data via a **serial terminal** to verify that the sensor data is correctly transmitted.

**Testing Tools to Be Used:**
- **PuTTY**: For monitoring the transmitted data on the serial terminal.
- **FPGA Debugging Tools**: For resolving any issues related to the sensor data transmission.

### 5. Documentation

I have compiled the findings so far, which include the **block diagram**, **circuit diagram**, and an overview of the steps taken. The final testing results, including code analysis, will be documented once the implementation and setup are complete.

---

## Challenges

- **Sensor Data Calibration**: Ensuring the sensor readings are accurate and reliable.
- **PC Issues**: There were some technical issues with uploading the bitstream to the FPGA. These issues have delayed the completion of the hardware setup.
- **UART Communication**: Ensuring stable and error-free data transmission is another challenge yet to be fully verified.

---

## Software Tools Used

- **Xilinx Vivado**: Used for FPGA design, synthesis, and programming.
- **PuTTY**: Will be used as a serial terminal to monitor and verify data transmission.
- **ModelSim/Vivado Simulator**: For simulating Verilog code before actual hardware testing.
- **FPGA Development Board** (Xilinx Spartan-6 or similar): Hardware used for the implementation.
- **JTAG Programmer**: Used to load the synthesized bitstream onto the FPGA.

---

## Conclusion

The task up to this point demonstrates the **initial design** of the integration between a **sensor module** and a **UART transmitter** on the FPGA. I have successfully developed the **block diagram** and **circuit diagram**, which form the foundation for the next steps in implementation and testing.

The actual hardware setup and bitstream loading have yet to be completed due to some technical challenges with my PC. However, the setup and verification will follow once these challenges are addressed.

---



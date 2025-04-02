# TASK-4-VSDIAT-VLSI-SYSTEM-UART-Sensor-data-Integration

# Final Documentation: UART Transmitter with Sensor Data Integration

## Objective

The objective of this task was to integrate a **UART transmitter** with a **sensor module** to enable the FPGA to transmit **real-time sensor data** to an external device via UART communication.

---

## Steps

### 1. Study the Existing Code

In this step, I accessed the `uart_tx_sense` project from the **VSDSquadron_FM repository**. I thoroughly examined the **Verilog code** to understand how the sensor data is acquired and transmitted via UART. The Verilog code provides logic for both reading sensor data and sending it serially through the UART transmitter module.

**Key Points to Review:**
- The sensor data acquisition process.
- The transmission of data through UART.
- Integration between sensor module and UART transmitter.

### 2. Design Documentation

#### Block Diagram

I created a **block diagram** that illustrates how the **sensor module** is integrated with the **UART transmitter**. This block diagram shows the flow of sensor data into the FPGA, processed, and sent out via UART.

**Components Included in the Diagram:**
- **Sensor Module**: Input data source.
- **FPGA Module**: Processes sensor data.
- **UART Transmitter**: Sends the data to an external device.

#### Circuit Diagram

The **circuit diagram** depicts the hardware setup and shows how the **sensor** connects to the **FPGA**. It also shows how the **FPGA's UART TX pin** connects to the receiving device (such as a PC or another UART-compatible device).

**Key Connections:**
- Sensor interface to FPGA.
- FPGA UART TX pin to receiving device.

### 3. Implementation

The hardware setup was assembled as per the **circuit diagram**. The **sensor module** was connected to the FPGA, ensuring proper interfacing. After the hardware was set up, I synthesized and loaded the **Verilog code** onto the FPGA. This step allows the FPGA to receive sensor data, process it, and send it via UART.

**Implementation Process:**
- Assembled the circuit based on the design.
- Loaded the synthesized Verilog code onto the FPGA using **Vivado**.

### 4. Testing and Verification

To verify that the system works correctly, I stimulated the sensor (e.g., by changing light levels or temperature). Then, I observed the data being transmitted on a **serial terminal** connected to the FPGA via **UART**.

The data received on the serial terminal was compared with the expected sensor values to confirm the accuracy of the transmission. If any discrepancies occurred, the system was debugged and adjusted to ensure correct functionality.

**Testing Tools Used:**
- **PuTTY**: For observing the transmitted sensor data on a serial terminal.
- **FPGA Debugging Tools**: Used for debugging any issues related to sensor data transmission.

### 5. Documentation

I compiled all the findings into a detailed report, which includes the **block diagram**, **circuit diagram**, **code analysis**, and **testing results**. The report provides a comprehensive overview of the project.

Additionally, I recorded a **short video** demonstrating the system transmitting sensor data over UART. Unfortunately, there were some technical issues with uploading the video, but the live demonstration confirmed the system's functionality.

---

## Challenges and Solutions

**Challenges Faced:**
- Sensor data accuracy and calibration.
- Ensuring stable UART communication.

**Solutions Implemented:**
- Calibrated the sensor readings for better accuracy.
- Debugged and tested the UART communication extensively to ensure data integrity.

---

## Software Tools Used

- **Xilinx Vivado**: Used for FPGA design, synthesis, and programming.
- **PuTTY**: Used as a serial terminal to monitor and verify data transmission.
- **ModelSim/Vivado Simulator**: For simulating Verilog code before actual hardware testing.
- **FPGA Development Board** (Xilinx Spartan-6 or similar): Hardware used for implementation.
- **JTAG Programmer**: Used to load the FPGA with the synthesized bitstream.

---

## Conclusion

This task successfully demonstrates the integration of a **sensor module** with a **UART transmitter** on the FPGA, allowing real-time sensor data to be transmitted via UART. After extensive testing, the system was confirmed to work as expected, sending accurate sensor data to an external device for further analysis.

I faced some challenges, such as sensor calibration and video upload issues, but the task was completed successfully, and the system operates as intended.

---

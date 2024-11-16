# Heart-Rate-Monitor-Microprocessor
A Microprocessor Project: Heart Rate and Heart Rate Zone Monitor

* Unfortunately, the Assembly code for this system has gone missing. A high level break down of the code logic can be found within the report at: https://github.com/mtwang0912/Heart-Rate-Monitor-Microprocessor/blob/main/Minnie_Wang_Lab3_G1_Jan_2024.pdf

## Main Features:
- Heart Rate and Heart Rate Zone Monitoring: The project developed a prototype capable of calculating heart rate (HR) and heart rate zones (HRZ) based on user input and biometric data.
- User Interaction: Included age input via a keypad, HR and HRZ display on an LCD, and data export to a text file via UART.
- Data Processing: Implemented HR calculations using R-R interval measurements and a Finite Impulse Response (FIR) filter for noise reduction.
- Performance Testing: Evaluated the prototype for accuracy and response, particularly focusing on the device's reliability under both stationary and moving conditions.
- Affordability and Memory Efficiency: The project highlighted the device’s cost-effectiveness compared to market alternatives and its minimal use of memory resources.

## Technologies Used:
- Microcontroller: PIC18F87K22 was used as the core processing unit, integrated into an EasyPIC PRO v7 development board.
- Biometric Sensor: Grove Ear-clip Heart Rate Sensor (GHRS) for detecting heartbeats through photoplethysmography.
- Display and Input Components:
  - LCD: 2x16 Liquid Crystal Display for output.
  - Keypad: 4x4 keypad for user input.
- Communication Module: UART serial communication for data transmission to a PC.

## Software Design:
- Top-Down Modular Design: Separated subroutines into modules for improved readability and debugging.
- Polling Mechanism: Employed a polling loop for detecting heartbeats through the sensor.
- Error Handling:
  - Considered timer overflow and potential pulse detection inaccuracies.
  - Adjusted FIR filter behavior to reduce initial measurement errors.

## Performance Metrics:
- Lin’s Concordance Correlation Coefficient (LCCC): Assessed the correlation between the prototype’s HR output and standard measurements.
- Error Quantification: Measured mean and average error rates.


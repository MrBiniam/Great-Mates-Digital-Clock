# Great Mates Digital Clock

## Project Overview

The **Great Mates Digital Clock** is a real-time digital clock project built using an **Arduino Nano**, **TM1637 7-segment display**, and **DS1307 RTC (Real-Time Clock) module**. This project demonstrates how to use these components to display the current time in hours and minutes, making it a simple yet functional digital clock for embedded systems.

The project is implemented using the **Wokwi platform**, an online simulation environment for building and testing Arduino projects.

## Project Demo

You can see a working simulation of this project on the [Wokwi Digital Clock Simulation](https://wokwi.com/projects/).

### Digital Images:
![Digital Image 1](https://github.com/user-attachments/assets/5af6eefa-48df-4d85-ad5e-bd5bdc75df96)
![Digital Image 2](https://github.com/user-attachments/assets/0deeeff5-942c-478f-b76b-a6c09a2911e4)

## Libraries Used

This project relies on the following libraries:

- **SevenSegmentTM1637 (v1.0.0)**: Used to interface with the TM1637 7-segment display and display the time.
- **RTclib (v1.0.0)**: Provides functions to interact with the DS1307 RTC module for retrieving the current date and time.

### Installation Instructions for Libraries:

1. Open the **Arduino IDE**.
2. Go to **Sketch > Include Library > Manage Libraries**.
3. In the Library Manager, search for the following libraries:
   - `SevenSegmentTM1637`
   - `RTClib`
4. Click **Install** for both libraries.

## Components Used

- **Arduino Nano**: The microcontroller that handles the logic, controls the display, and communicates with the RTC module.
  - Pin connections:
    - Pin 2: Connected to the CLK pin of the 7-segment display.
    - Pin 3: Connected to the DIO pin of the 7-segment display.
    - Pin A4: Connected to the SDA pin of the RTC module.
    - Pin A5: Connected to the SCL pin of the RTC module.
    - GND and 5V: Connected to respective pins on the display and RTC module.

- **TM1637 7-Segment Display**: A 4-digit display used to show the time in hours and minutes.
  - Connections:
    - CLK: Pin 2 of the Arduino Nano.
    - DIO: Pin 3 of the Arduino Nano.
    - VCC: 5V from the Arduino Nano.
    - GND: GND from the Arduino Nano.

- **DS1307 RTC Module**: Provides accurate timekeeping.
  - Connections:
    - SDA: Pin A4 of the Arduino Nano.
    - SCL: Pin A5 of the Arduino Nano.
    - VCC: 5V from the Arduino Nano.
    - GND: GND from the Arduino Nano.

## Circuit Diagram

Below is a simplified description of the circuit connections:

- **Arduino Nano (pins: 2, 3, A4, A5)**
- **TM1637 7-segment display (pins: CLK, DIO, VCC, GND)**
- **DS1307 RTC Module (pins: SDA, SCL, VCC, GND)**

## How It Works

- **RTC Setup**: The DS1307 RTC module is initialized to retrieve the current date and time.
- **Display Time**: The current time is fetched from the RTC and displayed on the TM1637 7-segment display in **HH:MM** format.
- **Real-time Operation**: The clock updates every second, ensuring the display shows the accurate time.

## How to Run the Project

### Prerequisites:
- **Arduino IDE** installed on your computer.
- **Arduino Nano** or compatible board.
- **DS1307 RTC Module** and **TM1637 7-segment display** for hardware setup.

### Steps to Run:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/MrBiniam/Great-Mates-Digital-Clock.git
2. Open the project in Arduino IDE:
         Open the .ino file in the Arduino IDE after cloning the repository.

Upload to your Arduino Nano:
      Connect the Arduino Nano to your computer.
      Select the correct board and port in the Tools menu.
      Click Upload to flash the code to the Arduino Nano.
      Watch the clock work: The time will be displayed on the 7-segment display, updating every second.

Dependencies
SevenSegmentTM1637: Version 1.0.0
RTClib: Version 1.0.0
These libraries are required to compile the code successfully.

Contributions
Feel free to contribute to this project! You can submit a pull request with improvements, bug fixes, or new features.

License
This project is licensed under the MIT License.

### Key Additions:
- Added **Steps to Run** with instructions to clone the repository, open it in the Arduino IDE, upload the code, and watch the clock work.
- Included **Dependencies** and **License** sections.

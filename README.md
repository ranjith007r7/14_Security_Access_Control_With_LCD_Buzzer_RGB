# 14_Security_Access_Control_With_LCD_Buzzer_RGB
# RGB LED Security Access Control System with Keypad and LCD

This Arduino project implements a security access control system using a keypad, RGB LED, and LCD display. The system provides visual and auditory feedback to the user based on the entered passcode.

## Components Used
- Arduino board
- 4x4 keypad
- RGB LED
- Buzzer
- 16x2 LCD display (with I2C interface)

## Description
The system operates as follows:
1. **Initialization**: Upon startup, the system initializes the keypad, RGB LED, buzzer, and LCD display. The RGB LED is set to show green to indicate readiness.
2. **User Input**: The user enters a passcode using the keypad and presses '#' to submit.
3. **Feedback Mechanism**:
    - If the entered passcode is correct, the RGB LED turns blue, the LCD displays "Access Granted," and the buzzer sounds two beeps.
    - If the entered passcode is incorrect, the RGB LED turns red, the LCD displays "Access Denied," and the buzzer remains silent.
4. **Reset**: After processing each passcode entry, the system resets to the ready state (green LED) and prompts the user to enter a new passcode.

## Files
- **security_access_control.ino**: Arduino sketch containing the code for the security access control system.
- **README.md**: This README file providing an overview of the project.

## Installation and Setup
1. Connect the components according to the circuit diagram.
2. Upload the `security_access_control.ino` sketch to the Arduino board.
3. Open the serial monitor to view system messages and prompts.
4. Enter the passcode using the keypad and observe the feedback on the RGB LED and LCD display.

## Circuit Diagram
*(Include a circuit diagram here if available)*

## Dependencies
- **Keypad Library**: Used to interface with the 4x4 keypad.
- **LiquidCrystal_I2C Library**: Required for controlling the LCD display via I2C interface.

## Note
Ensure that the keypad wiring and library setup match your specific configuration. Adjust pin assignments and library inclusions accordingly if needed.


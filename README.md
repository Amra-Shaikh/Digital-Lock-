# Digital Lock

## Project Overview

The **Digital Lock** project aimed to develop a secure digital lock system that operates through an Arduino microcontroller and is controlled via a keypad-based code entry system. The goal was to enhance the security of physical spaces by replacing traditional mechanical locks with a modern and customizable digital solution. Users enter a predefined code on the keypad; if the code matches, the door unlocks; if it doesn’t, the lock remains secure.

This digital lock system represents a fusion of hardware and software, allowing users to control access to rooms, lockers, or safes through a reliable mechanism.

## Technologies Used

- **Arduino Microcontroller**: The core component that processes inputs from the keypad and controls the locking mechanism.
- **Keypad**: A physical 4x4 keypad used for code entry, allowing users to input numeric values.
- **Servo Motor**: Controls the physical locking and unlocking mechanism of the door, rotating based on the input code.
- **C/C++ (Arduino IDE)**: The programming language used for input validation and controlling the servo motor.
- **Buzzer and LEDs**: Provide visual and auditory feedback based on correct or incorrect code entries. The buzzer sounds an alarm after multiple incorrect attempts.

## Key Features

- **Keypad-Based Entry**: The system utilizes a physical keypad for code entry, comparing the input to a pre-programmed code in the Arduino's memory. A match unlocks the door; otherwise, it stays locked.

- **Secure Locking Mechanism**: The servo motor connected to the Arduino physically locks and unlocks the door. The correct code causes the motor to rotate and unlock; an incorrect code keeps it locked.

- **Incorrect Code Detection and Alarm**: After a specified number of wrong code entries (e.g., 3 attempts), the system triggers an alarm using a buzzer, adding an extra security layer.

- **Customizable Code**: Users can easily change the security code by modifying the Arduino program, allowing for personalization according to preferences or security needs.

- **LED Feedback**: Integrated LEDs provide visual feedback: a green LED lights up for correct codes, while a red LED flashes for incorrect entries or during multiple failed attempts.

- **Low Power Consumption**: The system is power-efficient, relying on an Arduino and basic electronic components, and can be powered by batteries, ensuring functionality during outages or in remote locations.

## Challenges Faced

- **Keypad Input Validation**: Ensuring correct interpretation of keypad input was challenging due to quick or incomplete key presses. This was addressed by implementing debouncing logic in the code.

- **Servo Motor Calibration**: Precise rotation of the servo motor for locking and unlocking required calibration. Initial versions experienced over-rotation or insufficient rotation, which was resolved by fine-tuning the motor’s angles.

- **Security Considerations**: Ensuring the lock remained secure against multiple incorrect attempts was critical. I programmed the system to activate a buzzer alarm after several failed attempts, enhancing deterrence against brute force attacks.

## Final Outcome

The **Digital Lock** system functioned effectively, providing a simple yet efficient solution for securing physical spaces. The system accurately identified correct and incorrect codes, activating the servo motor to lock or unlock the door accordingly. The buzzer alarm for multiple incorrect attempts added an additional security layer, making unauthorized access more challenging.

This digital lock is suitable for applications where physical security is crucial, such as lockers, office doors, or safes. Its customization options allow for various use cases, including potential expansions like adding a Wi-Fi module for remote access.

## Conclusion

The **Digital Lock** project offered valuable hands-on experience with microcontrollers, electronic components, and Arduino programming. It demonstrated how simple electronic systems can enhance daily security. The integration of hardware (keypad, servo motor) and software (Arduino code) showcased my ability to combine multiple technologies into a functional, practical solution. This project highlights my understanding of secure systems, real-world implementation, and the importance of creating reliable, user-friendly interfaces.

# bldc-speed-controller
Arduino-based sensorless BLDC motor speed controller implementing PWM speed control and back-EMF feedback, tested on a standalone BLDC motor.
This project focuses on the design and implementation of a sensorless Brushless DC (BLDC) motor speed controller using an Arduino microcontroller. The objective of the project was to develop a standalone controller capable of regulating the speed of a BLDC motor without the use of physical position sensors, relying instead on back electromotive force (back-EMF) feedback and PWM-based control techniques.

The controller uses an Arduino (ATmega328P-based board) to generate PWM signals that drive a three-phase MOSFET bridge circuit, enabling electronic commutation of the BLDC motor. Motor speed is controlled by adjusting the PWM duty cycle, while back-EMF signals from the motor phases are monitored to determine rotor position and ensure proper commutation timing. This approach eliminates the need for Hall sensors, reducing system complexity and cost.

The hardware design includes a MOSFET driver stage, voltage regulation circuitry, and protection components such as flyback diodes to safely handle inductive loads. A comparator circuit is used to process the back-EMF signals and assist in detecting zero-crossing events required for sensorless operation. The controller was designed to operate from a 12V DC supply and was tested on a standalone BLDC motor under varying speed conditions.

The firmware was developed using the Arduino IDE and implements:

PWM generation for speed control

Basic startup and commutation logic

Back-EMF-based feedback for sensorless operation

Adjustable speed control using an external input (e.g., potentiometer)

This project demonstrates practical knowledge of BLDC motor control principles, power electronics, embedded systems, and microcontroller-based motor control, and serves as an educational implementation of a sensorless BLDC speed controller.

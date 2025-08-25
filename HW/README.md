# \# ATmega128A Security System Development Board

# 

# \## 🔎 Overview

# The \*\*ATmega128A Security System Board\*\* is a multi-purpose embedded platform designed for \*\*learning, prototyping, and smart access control systems\*\*.  

# It combines \*\*classic AVR development features\*\* with \*\*security-oriented peripherals\*\* such as keypad password entry, shock/vibration sensing, Bluetooth communication, and servo-based locking mechanisms.

# 

# ---

# 

# \## 📑 Design Resources

# \- \*\*Schematics\*\*: \[Atmega.pdf](Atmega.pdf) (KiCad 9.0.4)

# 

# ---

# 

# \## ⚙️ Key Components \& Features

# 

# \### 1. Microcontroller (MCU)

# \- \*\*Model\*\*: ATmega128A-AU  

# \- \*\*Role\*\*: 8-bit AVR microcontroller, serving as the “brain” of the board.  

# \- \*\*GPIO Access\*\*: Ports A–G exposed via connectors for easy module expansion.

# 

# ---

# 

# \### 2. Power Supply

# \- \*\*Input\*\*: 12V via Barrel Jack (J1)  

# \- \*\*Regulators\*\*:  

# &nbsp; - TPS562201-5.0 (U1) → regulated \*\*5V\*\*  

# &nbsp; - TPS562201-3.3 (U2) → regulated \*\*3.3V\*\*  

# \- \*\*Reset\*\*: Push-button (SW2) for manual MCU reset  

# \- \*\*Design Goal\*\*: Provides stable dual-voltage support for mixed-voltage peripherals.

# 

# ---

# 

# \### 3. Communication Interfaces

# \- \*\*USB-to-Serial\*\*: FT232RL (U3) for USB ↔ UART communication (PC connection, debugging, firmware upload).  

# \- \*\*ISP (In-System Programming)\*\*: 6-pin ISP header (J5) for direct programming with AVR programmer.  

# \- \*\*Bluetooth (J2)\*\*: HC-06 module for \*\*wireless data transmission\*\* (remote monitoring \& control).

# 

# ---

# 

# \### 4. Clock \& Reset

# \- \*\*Crystal Oscillator\*\*: 16 MHz (Y1) for precise MCU operation.  

# \- \*\*Reset Circuit\*\*: Dedicated reset button for system restart.

# 

# ---

# 

# \### 5. User Interface \& Expansion

# \- \*\*LEDs\*\*: 4× user LEDs (D1–D4) for program status and debugging.  

# \- \*\*Expansion Ports\*\*: Multiple GPIO connectors (J3, J4, J6, J7, J8, J9).  

# \- \*\*LCD (J4)\*\*: Displays password input results, error messages, and lockout countdowns.  

# \- \*\*Keypad (J5)\*\*: Used for \*\*password entry and modification\*\*.  

# 

# ---

# 

# \## 🔐 Security-Oriented Features

# 

# | Module        | Functionality |

# |---------------|---------------|

# | \*\*Keypad (J5)\*\* | Enter/change password; authenticates user input |

# | \*\*LCD (J4)\*\* | Displays password status, errors, and lockout timer |

# | \*\*Servo Motor\*\* | Unlocks when password is correct; remains locked on failure |

# | \*\*Buzzer (BZ1)\*\* | Alerts on wrong password attempts or vibration detection |

# | \*\*SW-420 Sensor (J1)\*\* | Detects external shock/vibration for tamper alerts |

# | \*\*HC-06 Bluetooth (J2)\*\* | Enables wireless data exchange with smartphone/PC |

# 

# ---

# 

# \## ✅ Summary

# This board is designed not only for \*\*general AVR prototyping\*\*, but also as a \*\*practical security system prototype\*\*, featuring:

# \- \*\*Multi-layered access control\*\* (Keypad + LCD feedback + Servo lock)  

# \- \*\*Tamper detection\*\* (Shock/vibration sensor with buzzer alerts)  

# \- \*\*Remote connectivity\*\* (Bluetooth HC-06 for monitoring \& updates)  

# \- \*\*Educational value\*\*: Learn real-world embedded security design principles  

# 

# ---

# 

# \## 📦 Example Applications

# \- Smart door lock prototype  

# \- IoT-enabled access control system  

# \- Embedded security teaching platform  

# \- Password-protected equipment locker  

# 

# ---

# 

# \## 📸 PCB Preview (Optional)

# | Top View | Bottom View | Assembled |

# |----------|-------------|-----------|

# | !\[Top](docs/images/top.jpg) | !\[Bottom](docs/images/bottom.jpg) | !\[Assembled](docs/images/assembled.jpg) |

# 

# \*(Replace with actual photos of your board)\*

# 

# ---

# 

# \## 📧 Contact

# If you build on this board, feel free to share your projects or improvements!




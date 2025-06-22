# PLC-Based-Automated-Conveyor-and-Filling-System
### PLC-Based Automated Conveyor and Filling System

This repository contains a detailed implementation of a Programmable Logic Controller (PLC) program designed for an automated conveyor system managing the sorting and filling of boxes labeled with color-specific indicators. The logic ensures precise control of conveyor movements and selective dispensing of products (pecans and walnuts) based on label detection, utilizing digital sensors and actuators.

#### Project Overview:

* **Objective:** Automate conveyor operations to accurately sort boxes by label color (red or blue), dispense corresponding nuts (pecans or walnuts), and manage conveyor operations efficiently.
* **Components:** Proximity switch, level sensor, color detection photo eyes, conveyor motor, and product-specific hopper actuators.

#### Implementation and Key Features:

* **Sensor-Based Detection and Sorting:**

  * **Proximity Switch:** Detects the presence of boxes on the conveyor.
  * **Level Switch:** Indicates when boxes are filled to the required level.
  * **Color Photo Eyes:** Distinguishes box labels (red for pecans, blue for walnuts).

* **Actuation and Feedback:**

  * **Conveyor Motor Control:** Stops when boxes are in position for filling, resumes movement once filled.
  * **Product Hopper Solenoids:** Selectively dispenses pecans or walnuts based on detected label color, ensuring precise product handling.

* **PLC I/O Assignment:**

  * **Inputs:**

    * I:0/0: Proximity switch (box presence).
    * I:0/1: Level switch (box fill detection).
    * I:0/2: Red photo eye (pecan identification).
    * I:0/3: Blue photo eye (walnut identification).
  * **Outputs:**

    * O:0/0: Conveyor motor activation.
    * O:0/1: Walnut hopper solenoid.
    * O:0/2: Pecan hopper solenoid.

#### Test Criteria and Performance Evaluation:

* Comprehensive testing procedures validate system behaviors:

  * Immediate conveyor activation and correct initial hopper states.
  * Accurate box detection halting conveyor for filling operations.
  * Precise product dispensing controlled by label color detection.
  * Automatic conveyor restart upon successful box filling.
  * Robust performance in various simulated sensor conditions.

#### Strengths and Learning Points:

* **Efficient Control Logic:** Clear and maintainable PLC logic enhances system reliability and performance.
* **Automated Product Sorting:** Demonstrates real-world sorting and dispensing automation applicable in packaging industries.
* **Detailed Error Handling:** Logic design prevents product wastage, overfilling, and operational delays.

#### Future Development:

* Incorporation of advanced vision systems for enhanced label detection accuracy.
* Integration with automated inventory management systems.
* Implementation of additional safety features and emergency stop mechanisms.

This project demonstrates robust industrial automation practices through effective PLC programming, ensuring precise control, operational efficiency, and adaptability for real-world conveyor-based sorting and filling systems.

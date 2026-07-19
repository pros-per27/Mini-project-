# Smart Device Management System

A Python-based Object-Oriented Programming (OOP) mini-project designed to simulate a management framework for smart home devices[span_2](start_span)[span_2](end_span). This project showcases foundational and advanced OOP principles including inheritance, encapsulation, and polymorphism[span_3](start_span)[span_3](end_span).

## 📌 Project Overview
The **Smart Device Management System** simulates software developed for a technology company to manage various smart home utilities[span_4](start_span)[span_4](end_span). The system handles universal device properties (like power status and unique IDs) while accommodating specialized capabilities for different device types via a simple, interactive terminal menu interface[span_5](start_span)[span_5](end_span).

This project was developed for the **EL 162 / 234 Object Oriented Programming** course at the University of Mines and Technology (UMaT) under the supervision of Dr. Matthew Cobbinah[span_6](start_span)[span_6](end_span).

---

## 🛠️ Key Features & OOP Concepts Demonstrated

* **Encapsulation:** Sensitive attributes such as `device_id` and `power_status` are kept private[span_7](start_span)[span_7](end_span). Access and modifications are strictly controlled using getters, setters, and Python property decorators (`@property`) with data validation[span_8](start_span)[span_8](end_span).
* **Inheritance & Reusability:** A robust parent class (`SmartDevice`) passes shared attributes and methods down to specialized child classes using `super()` initialization[span_9](start_span)[span_9](end_span).
* **Polymorphic Device Architecture:**
  * **`SmartDevice` (Parent):** Manages basic identity, state changes (`turn_on`/`turn_off`), and generalized info display[span_10](start_span)[span_10](end_span).
  * **`TemperatureSensor` (Child):** Adds temperature tracking and reading capabilities[span_11](start_span)[span_11](end_span).
  * **`SecurityCamera` (Child):** Tracks and toggles live recording states (`start_recording`/`stop_recording`)[span_12](start_span)[span_12](end_span).
  * **`SmartLight` (Child):** Manages dimming adjustments with input validation constraining levels between 0 and 100[span_13](start_span)[span_13](end_span).
* **Menu-Driven CLI Interface:** A user-friendly, loop-controlled terminal menu that allows real-time execution and monitoring of all device behaviors[span_14](start_span)[span_14](end_span).

---

## 📂 Repository Structure

```text
smart-device-management-system/
│
├── main.py            # Main application script containing classes and the CLI loop
├── README.md          # Project documentation and setup guide
└── .gitignore         # Standard Git ignore file

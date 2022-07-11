# The Serial Monitor
---
- Part of the **Arduino IDE**
- Clicking on the rightmost icon in the toolbar
- *Acts as a communication channel*
- **Information** is sent through the *USB link between computer and the Arduino*.
- *Communication initiated* by `Serial.begin(9600)`
	- 9600 is dependent on what channel the monitor is on
- `Serial.println` – a built‐in function to send a message to the Serial Monitor
- A **single argument** – usually a variable
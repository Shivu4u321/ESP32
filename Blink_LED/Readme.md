**objective: Turn an LED ON and OFF. **

_Procedure:_

1. Connect the ESP32 Wroom to PC using USB cable.
2. Open the Arduino software.
3. Create New project: File -> new Sketch.
4. Connect the **Anode** (hint: long needle) of **LED** to **D5** of **ESP32** and **Cathode** to **ground**.
   <img width="272" alt="image" src="https://github.com/user-attachments/assets/d798e26d-d314-4aec-ae22-a4f423e6cafe" />


5. Copy the below code and paste in New Sketch.

-------------------------------------------

int LED=5; <br/>
// The setup function runs once when you press reset or power the board <br/>
void setup() {<br/>
// initialize digital pin LED_BUILTIN as an output.<br/>
  pinMode(LED, OUTPUT);<br/>
}<br/>

// the loop function runs over and over again forever  <br/>
void loop() { <br/>
  digitalWrite(LED, HIGH);  // turn the LED on (HIGH is the voltage level) <br/>
  delay(100);                      // wait for a second <br/>
  digitalWrite(LED, LOW);   // turn the LED off by making the voltage LOW <br/>
  delay(100);                      // wait for a second <br/>
} <br/>

---------------------------------------
6. Select the Comport and Board as shown below:<br/>
   **Comport Selection:**<br/>
   <img width="557" alt="image" src="https://github.com/user-attachments/assets/c21e3c1a-4f2e-4aa3-8dc9-8c42bbe5780b" />

   **Board selection:**<br/>
   <img width="932" alt="image" src="https://github.com/user-attachments/assets/77cc1dcc-14eb-4fa9-8f7d-f66a07b236a4" />
7. Click on verify:
   <img width="323" alt="image" src="https://github.com/user-attachments/assets/d6d0ac27-25d6-4e97-a5b3-4938ebbae01d" />
8. Click on Upload:
   <img width="381" alt="image" src="https://github.com/user-attachments/assets/c44d4fc5-3338-48db-9798-7443970af85a" />
9. On old boards you need to press reset/Boot button to see the LED blinking:
    

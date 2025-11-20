# Design-and-Simulation-of-an-Piano-Circuit-using-IC555

## 📌 Experiment 10: Piano Tone Generator Circuit Design

### **Aim**
Design the schematic and PCB layout of an electronic piano tone generator circuit using Autodesk EAGLE and generate Gerber files for PCB manufacturing.

---

## 🧰 Equipment Required
### **Hardware**
- Personal Computer (PC)

### **Software**
- Autodesk EAGLE PCB Design Suite

---

## 📝 Procedure

### **1️⃣ Create a New Project**
- Open **EAGLE** and create a new project.
- Inside the project, create a **new schematic (.sch)** file.

### **2️⃣ Add Components**
- Add components from EAGLE libraries:
  - 555 Timer IC / Microcontroller
  - Resistors
  - Capacitors
  - Push buttons (piano keys)
  - Piezo buzzer / speaker
  - Power connector
- Use the **Add (✚)** tool to place parts on the schematic.

### **3️⃣ Make Electrical Connections**
- Use the **Net** tool to:
  - Connect each push button to its respective resistor.
  - Connect timing components to the 555 timer/MCU.
  - Connect output to the audio buzzer.
- Label nets for clarity.

### **4️⃣ Run ERC (Electrical Rule Check)**
- Perform **ERC** to find wiring errors.
- Fix all warnings and errors before proceeding.

### **5️⃣ Switch to Board Layout**
- Click **“Switch to Board”** to generate the PCB layout.
- Components from the schematic appear on the board.

### **6️⃣ Arrange Components & Route Tracks**
- Align push buttons in a straight row like piano keys.
- Place resistors and timing components near the 555 timer for short traces.
- Route tracks using the **Route** tool.
- Ensure clean ground routing for noise-free audio output.

### **7️⃣ Run DRC (Design Rule Check)**
- Perform **DRC** to ensure:
  - Correct clearance
  - Track width validity
  - Proper pad spacing  
- Fix all errors and save your board design.

### **8️⃣ Generate Gerber Files**
- Go to **File → CAM Processor**.
- Generate Gerber files for:
  - Top copper
  - Bottom copper
  - Silkscreen
  - Solder mask
  - NC drill
- Export and save all manufacturing files.

### **9️⃣ Save & Backup**
- Store your:
  - `.sch`
  - `.brd`
  - Gerber files  
in your project directory.

---

## 📚 Theory

The piano tone generator circuit works by producing different audio frequencies corresponding to musical notes.  
This can be done using:

### **✔ 555 Timer in Astable Mode**
- Each key (push button) selects a different resistor.
- Changing the resistor changes the RC timing.
- This changes the oscillation frequency.
- The piezo speaker outputs the corresponding note.

### **✔ Microcontroller-based Design**
- Each key press triggers a programmed PWM frequency.
- The MCU outputs the musical note digitally.

This circuit demonstrates frequency generation, sound synthesis, and basic PCB design concepts.

---

## ⚙ Working

- When the circuit is powered ON, the 555 timer generates a continuous oscillation.
- Each piano key (button) selects a unique resistor value.
- Changing the resistor changes the output frequency.
- The buzzer produces the corresponding musical tone.
- Releasing the key breaks the timing network and stops the tone.

---
## Output Files
This project includes:
### Schematic Diagram  
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2d296750-322a-4bc4-8b1b-9ed8d3e6f9b7" />

### PCB Layout  
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0a0551fd-32cf-481b-aab9-733fc374b1da" />

### Gerber Files (Manufacturing Ready)

### Final project
<img width="1034" height="706" alt="image" src="https://github.com/user-attachments/assets/679785a5-6e90-4efb-b74a-f62aee4e5f72" />

---

## ✅ Result
The **Piano Tone Generator circuit** schematic and PCB were successfully designed in **EAGLE**, and Gerber files were generated for fabrication.


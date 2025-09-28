# Low Power SRAM Design using Cadence Virtuoso

## 📌 Overview
This project focuses on the design and verification of a **Low-Power 10T (LP10T) SRAM cell** using **Cadence Virtuoso**.  
The design was first implemented in **GPDK90nm** technology and later migrated to **GPDK45nm**, resulting in improved power and performance characteristics.

---

## 🛠️ Tools & Technology
- **EDA Tool**: Cadence Virtuoso  
- **Technology Node**:  
  - GPDK90nm (initial implementation)  
  - GPDK45nm (final implementation)  
- **Design Type**: LP10T SRAM Cell  

---

## 🔄 Implementation Flow
1. **Design in GPDK90nm**
   - Implemented LP10T SRAM cell.  
   - Verified functionality with custom test cases.  
   - Achieved a maximum output voltage of **~850mV for 1V input**.  

2. **Migration to GPDK45nm**
   - Re-implemented design at 45nm technology node.  
   - Observed improved results:  
     - Maximum output voltage: **~780mV for 1V input**.  
   - Better trade-off between **power efficiency** and **performance**.  

---

## 🧪 Verification Methodology
Two **custom test cases** were developed to validate functionality and stability.

### Custom Case 1
Hold → Write '1' → Hold → Read → Hold → Read → Hold → Write '0' → Hold → Read

### Custom Case 2
Hold → Write '0' → Hold → Read → Hold → Read → Hold → Write '1' → Hold → Read


✅ These cases ensure proper **read/write functionality** and confirm **data retention** under multiple operations.

---

## 📊 Results
| Technology Node | Input Voltage | Max Output Voltage |
|-----------------|---------------|--------------------|
| GPDK90nm        | 1V            | ~850mV             |
| GPDK45nm        | 1V            | ~780mV             |

- **Observation**: The LP10T SRAM cell in **45nm** shows better power efficiency and reduced voltage degradation compared to 90nm.  

---

## 📷 Project Snapshots

### 🔹 Schematics
- GPDK90 Schematic  
  ![GPDK90 schematic](images/GPDK90%20schematic.png)  

- Testing Schematic for GPDK90  
  ![Testing Schematic for GPDK90](images/Testing%20Schematic%20for%20GPDK90.png)  

- GPDK45 Schematic  
  ![GPDK45 schematic](images/GPDK45%20schematic.png)  

---

### 🔹 Simulation Results (GPDK90)
- Case 1  
  ![GPDK90 Case 1](images/GPDK90%20case%201.png)  
  ![GPDK90 Case 1 with values](images/GPDK90%20case%201%20with%20values.png)  

- Case 2  
  ![GPDK90 Case 2](images/GPDK90%20case%202.png)  
  ![GPDK90 Case 2 with values](images/GPDK90%20case%202%20with%20values.png)  

- Overall Values  
  ![GPDK90 values](images/GPDK90%20values.png)  

---

### 🔹 Simulation Results (GPDK45)
- Case 1  
  ![GPDK45 Case 1](images/GPDK45%20case%201.png)  
  ![GPDK45 Case 1 with values](images/GPDK45%20case%201%20with%20values.png)  

- Case 2  
  ![GPDK45 Case 2](images/GPDK45%20case%202.png)  
  ![GPDK45 Case 2 with values](images/GPDK45%20case%202%20with%20values.png)  

- Overall Values  
  ![GPDK45 values](images/GPDK45%20values.png)  

---

## 🚀 Next Steps
- Perform **Static Noise Margin (SNM)** analysis for read/write stability.  
- Optimize transistor sizing for further voltage retention.  
- Test under **different PVT corners** for robustness.  

---

## 📚 References
- Cadence Virtuoso Documentation  
- Research papers on Low-Power SRAM design and 10T cell structures  

---

## 👨‍💻 Author
Project by: Kamisetty Sai Sravan  

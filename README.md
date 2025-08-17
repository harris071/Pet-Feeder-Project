# Automated Pet Feeder Project

## Overview
This project is a **simulation and design** of a low-cost, automated pet feeder system for a local animal shelter.  
The feeder is programmable to dispense food at scheduled times, monitor whether food has been consumed, and send alerts if any issue occurs (e.g., food not dispensed, pet not eating).  

This repository is organized according to the **Problem-Solving Process** taught in the Introduction to Information Technology unit.

---

## Features
- Dispenses food for cats and dogs at scheduled times.
- Monitors bowl weight before and after feeding.
- Detects if the food bin is empty.
- Waits 10 minutes to check if food is eaten.
- Sends alerts if:
  - Food bin is empty.
  - Pet does not eat after 10 minutes.
- Simple, modular design suitable for **Arduino / Raspberry Pi** implementation.

---

## Repository Structure
```
pet-feeder-project/
│── Step1_Analysis/
│     └── problem_analysis.pdf
│── Step2_Data/
│     └── data_table.xlsx
│── Step3_Flowchart/
│     ├── pet_feeder_flowchart.drawio
│     └── pet_feeder_flowchart.png
│── Step4_Word_Code/
│     └── word_code.txt
│── Step5_Testing/
│     └── test_results.pdf
│── Logic_Circuit/
│     ├── logic_circuit.png
│     └── logic_equations.txt
│── README.md
```

---

##  System Logic

### Flowchart
The system logic follows these steps:
1. Check current time.
2. If it’s feeding time → check food bin.
3. If food is available → activate servo to dispense.
4. Wait 10 minutes.
5. Check bowl weight & pet presence.
6. If food not eaten → send alert.  
7. Else → log "Food eaten".


---

## Testing Scenarios
- **Case 1:** Pet eats as expected → Log event.
- **Case 2:** Pet does not eat → Alert staff.
- **Case 3:** Food bin empty → Alert staff.
- **Case 4:** Early check (not feeding time) → No action.

---

## Future Improvements
- Mobile app notifications instead of simple buzzer/LED alerts.
- Camera integration for monitoring pets.
- Multiple feeding times per day.
- Battery backup for power outages.

---

## Author
- **Harris Siddiqui**  
u3310684@uni.canberra.edu.au | Student at University of Canberra  

---

## License
This project is created for academic purposes under the University of Canberra’s **Introduction to IT (4478/8936)** course.  

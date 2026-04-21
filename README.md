🔧 4-bit Full-Custom ALU – CMOS vs Transmission Gate
Full-custom 4-bit ALU designed in 45nm technology using Cadence Virtuoso.
This project compares Static CMOS and Transmission Gate (TG) logic styles in terms of Power, Performance, and Area (PPA).

📌 Project Overview
The goal of this project was to design a transistor-level ALU and evaluate engineering trade-offs between two implementation styles:
•	Static CMOS - robust and reliable
•	Transmission Gate - optimized for area and power
The comparison includes both pre-layout and post-layout (PEX) simulations.

🧠 ALU Architecture
The ALU is composed of:
•	Logic Unit - XOR-based operations
•	Arithmetic Unit - Full Adders (FA)
•	Multiplexer (MUX) - operation selection
The design was implemented hierarchically at the transistor level.

🛠 Design Flow
•	Schematic Design
•	Logic Implementation (XOR, MUX, FA)
•	Layout Design
•	Physical Verification (DRC / LVS)
•	Parasitic Extraction (PEX)
•	Pre-Layout & Post-Layout Simulations

⚙️ CMOS Implementation
•	Complementary pull-up / pull-down networks
•	Full voltage swing
•	High noise margins
•	Robust but larger area and higher power

⚡ Transmission Gate Implementation
•	Parallel NMOS + PMOS pass transistors
•	Reduced transistor count
•	Smaller area and lower power
•	More sensitive to parasitic effects

📊 PPA Results
Pre-Layout:
•	TG showed faster delay and lower power
Post-Layout:
•	Area: ↓ ~38% (TG)
•	Power: ↓ ~30% (TG)
•	Performance: CMOS faster due to parasitics
•	PDP: Improved with TG

⚠️ Parasitic Effects (Post-Layout)
Post-layout simulations include real physical effects:
•	Metal resistance
•	Parasitic capacitance
•	Coupling capacitance
•	Contacts / vias resistance
These significantly impact delay and power, especially in TG logic.

🔬 Robustness Analysis
•	PVT Corners: Verified across process, voltage, temperature
•	Monte Carlo Simulation:
o	100% Yield
o	No functional failures

⚖️ Trade-Off Analysis
•	Transmission Gate:
o	Smaller area
o	Lower power
o	Higher sensitivity to parasitics
•	Static CMOS:
o	Better post-layout performance
o	More robust
o	Larger and more power-consuming

🎯 Conclusion
This project demonstrates that:
•	Engineering design involves trade-offs
•	TG improves area and power efficiency
•	CMOS provides better post-layout robustness
•	Post-layout simulation is critical in VLSI design

📁 Files
- 📄 [Project Report (PDF)](./ALU_Project_Report.pdf)


📌 Overview

This project is a Mini Inverter PCB designed using KiCad that converts 12V DC into AC output using a push-pull topology. The design is centered around the IR2153 gate driver IC and IRLZ34N MOSFETs, driving a center-tapped transformer to generate an alternating waveform.

The project demonstrates practical implementation of power electronics design, including switching circuits, transformer interfacing, PCB layout considerations, and thermal management.

⚙️ Working Principle

DC Input Supply
A 12V DC source powers the circuit.
Oscillator & Driver (IR2153)
The IR2153 generates alternating gate signals.
These signals control switching of MOSFETs.
MOSFET Switching Stage
Two IRLZ34N MOSFETs switch alternately.
This creates an alternating current through the transformer primary.
Transformer Operation
A center-tapped transformer converts the switching waveform into AC.
The output is taken from the secondary winding.
Output
AC voltage is available across the transformer output terminals.


🧩 Components Used & Their Purpose

🔌 Power Section

Battery / DC Input (12V)
Provides input power to the circuit.
Terminal Block / Connector
Used to connect external power supply safely.

🧠 Control Section
IR2153 (Gate Driver IC)
Generates oscillating signals.
Drives MOSFET gates in push-pull configuration.
Timing Resistor & Capacitor
Sets switching frequency of IR2153.

⚡ Switching Section
IRLZ34N MOSFETs (x2)
Act as high-speed switches.
Alternately drive current through transformer primary.
Gate Resistors
Control gate charging/discharging speed.
Reduce noise and oscillations.

🔋 Passive Components
Resistors
Used for biasing, timing, and current limiting.
Capacitors
Power filtering
Noise reduction
Timing control

🔄 Protection Components
Diodes (e.g., 1N4007)
Protect circuit from reverse currents and voltage spikes.

🔁 Transformer
Center-Tapped Transformer
Converts DC switching into AC output.
Key component for voltage conversion.

💡 Indicators
LED + Resistor
Indicates power ON status.

🖥️ PCB Design Features
Designed in KiCad
Compact layout with functional block separation
Thick traces for high-current paths
Basic thermal considerations for MOSFETs
3D visualization included

⚠️ Important Notes
-Output is square wave AC, not pure sine wave
-Not suitable for sensitive electronics
-Proper heatsinking required for MOSFETs under load
-Ensure correct transformer rating before use

🚀 Future Improvements
-Improved PCB routing for power efficiency
-Better thermal management design
-Addition of protection circuits (fuse, reverse polarity)
-Conversion to pure sine wave inverter

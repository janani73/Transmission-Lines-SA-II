# Transmission-Lines-SA-II

# SCADA: Supervisory Control and Data Acquisition

# Introduction

SCADA is an industrial automation control system used for gathering real-time data from remote locations and controlling equipment from a centralized system. It plays a vital role in power transmission systems, where it's used to monitor line status, measure voltages/currents, detect faults, and issue control commands.

![image](https://github.com/user-attachments/assets/c04fd2a0-7696-4909-a991-0572c4f9c049)

# Key Features:

Continuous monitoring of electrical parameters (voltage, current, frequency).

Control of switches, circuit breakers, and capacitor banks.

Alarm systems and fault detection.

Historical data logging and trend analysis.

# Architecture of SCADA in Power Transmission

![image](https://github.com/user-attachments/assets/cae3c577-c698-4da1-9297-f766a2b1b286)

# MTU (Master Terminal Unit):

Located at the control center.

Collects and processes data from RTUs.

# RTU (Remote Terminal Unit):

Placed at substations or field locations.

Collects data from sensors and sends it to the MTU.

# PLC (Programmable Logic Controller):

Handles automation logic (e.g., trip breakers on fault detection).

# HMI (Human-Machine Interface):

Visual interface for human operators to monitor and control equipment.

# Communication Infrastructure:

Wired (fiber optics, coaxial cables) or wireless (radio, satellite).

Protocols like Modbus, DNP3, IEC 60870-5-104.

# Key Formulas Used in SCADA (with Examples)

# Ohm’s Law

𝑉=𝐼×𝑅

Application: To detect voltage drop across transmission lines.

Example:

𝐼=250 

𝑅=0.2Ω

Voltage drop 

𝑉=250×0.2=50𝑉

![image](https://github.com/user-attachments/assets/fd2642b9-3ec1-483d-a1a7-b2e589ca17fe)

# Real Power (P)

𝑃=𝑉×𝐼×cos(𝜙)

Application: Measures actual power consumed/delivered.

Example:

V=132kV

I=200Acos(𝜙)=0.9

P=132,000×200×0.9=23.76MW

# Apparent Power (S)

S=V×I

Application: Full capacity of the transmission line including losses.

S=132,000×200=26.4MVA

# Reactive Power (Q)

Q=V×I×sin(ϕ)

𝜙=cos−1(0.9)=25.84∘⇒sin(𝜙)=0.4359
 
Q=132,000×200×0.4359≈11.5MVAR

# Power Factor (PF)

PF=𝑃/𝑆=23.76/26.4≈0.9

# Benefits of SCADA in Transmission

✅ Faster fault detection and isolation

✅ Remote operation reduces need for field visits

✅ Prevents blackout through early warnings

✅ Improves grid efficiency and load management

✅ Enables real-time data analytics and forecasting

# SCADA in Action: Real-Life Example 

In a high-voltage transmission network, SCADA plays a vital role in preventing system overloads and blackouts. Consider a 220 kV transmission line that normally operates at 500 A. During a peak demand hour,the 

line current spikes to 600 A due to unexpected load increase. The SCADA system, via its RTU at the substation, continuously monitors the current and voltage. Once the overload threshold is detected, the SCADA 

system instantly calculates the power flow using real-time data:

P=V×I×cos(ϕ)=220,000×600×0.85=112.2MW

This exceeds the rated capacity of 100 MW. The SCADA control logic automatically initiates a corrective action—sending signals to remotely controlled circuit breakers to shed non-critical loads or reroute power

through alternative lines. An alarm is also raised in the control center, alerting operators to verify and confirm actions. Simultaneously, the event is logged for historical analysis and performance review.

This real-time decision-making minimizes the risk of line failure, prevents cascading outages, and ensures continued supply to critical areas. Such automation through SCADA enhances grid reliability, reduces 

downtime, and supports efficient energy management in modern power systems.










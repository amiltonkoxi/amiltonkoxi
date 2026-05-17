<div align="center">

# Amilton Koxi

<sub>**R&D Engineer** &nbsp; · &nbsp; Embedded Systems &nbsp; · &nbsp; FPGA &nbsp; · &nbsp; Edge AI</sub>

<sub>Debrecen, HU &nbsp; · &nbsp; <a href="mailto:amiltonkoxi2023@gmail.com">amiltonkoxi2023@gmail.com</a> &nbsp; · &nbsp; <a href="https://www.linkedin.com/in/amiltonkoxi/">LinkedIn</a></sub>

</div>

<br/>

<div align="center">
  <img src="./media/signal-path.svg" width="100%" alt="Signal path from sensor to browser"/>
</div>

<br/>

I work on embedded systems where the constraints actually matter. Tight memory, noisy signals, strict timing, lossy radio. Most of my work lives between the sensor pin and the screen, in places where there is no rollback if you get it wrong.

The diagram above is the kind of system I build. Real sensors. Real FPGA. Real wireless. Anomaly detection that runs on the edge because the cloud is not always there, and even when it is, latency and reliability often say otherwise.

<br/>

---

### Now &nbsp;·&nbsp; <sub>Q2 2026</sub>

```
[ active ]   FMEAD FPGA           multi modal anomaly detector on Nexys 4 DDR
[ active ]   MSc final defense    University of Debrecen · embedded systems track
[ pending ]  PhD interview prep   post quantum cryptography on FPGA
[ pending ]  EnCLOD hackathon     traffic engineering · team Ngola Labs
```

<br/>

---

### Selected work

<br/>

**`FMEAD FPGA`** &nbsp; *Field Multi modal Edge Anomaly Detector*

A real time edge platform that detects abnormal physical events directly on FPGA hardware. Fuses motion, environmental, acoustic, and thermal signals. Runs anomaly scoring entirely on the device. Exposes a live dashboard over Wi Fi without a cloud roundtrip. Built on Nexys 4 DDR with MicroBlaze, custom VHDL IPs, ADXL362, BME280, PDM microphone, and ESP32 bridge.

The hard parts were not the algorithms. They were the AXI bring up, the polled SPI budget, the BRAM constraints, and the ESP32 AT command state machine that had to survive bad signal conditions.

→ &nbsp;[`amiltonkoxi/FMEAD-FPGA`](https://github.com/amiltonkoxi/FMEAD-FPGA) &nbsp; · &nbsp; `VHDL` `C` `MicroBlaze` `Edge AI`

<br/>

**`WSN Swarm Anomaly Detection`** &nbsp; *MSc thesis · 2nd place TDK 2026 · OTDK nomination*

Three tier wireless sensor network with ESP32 edge nodes, Raspberry Pi gateway, and fog server. Runs EWMA and Page Hinkley change detectors with PSO tuned thresholds. Validated over 72 hours across 30 random seeds. Tracked detection rate, detection delay, false positive rate, and average power per hour as primary metrics.

The point was not to invent new statistics. It was to prove that swarm intelligence can reliably tune anomaly detection in real, noisy, distributed sensing environments.

→ &nbsp;`ESP32` `Python` `PSO` `WSN`

<br/>

**`SentinelNet`** &nbsp; *1st place · GroundUP_eu Industrial Edge AI Hackathon 2026*

AI powered CBRNE early warning platform built in a constrained time window. Edge sensing layer, classification pipeline, and operator dashboard for civil protection scenarios. Designed and delivered with a small team under hackathon conditions.

→ &nbsp;`Python` `Edge AI` `IoT`

<br/>

---

### How I work

**Hardware first.** I do not trust a system until I see real signals on a scope, real packets on the wire, and real numbers from real sensors. Simulations are useful, but they are not the system.

**Measure before guessing.** Most embedded bugs are not algorithmic. They are timing, alignment, voltage, or a missed handshake. Instrument first, theorize later.

**Constraints sharpen design.** Limited BRAM forces better data structures. Tight CPU budget forces better algorithms. The microcontroller is not a limitation. It is a filter for sloppy thinking.

**Ship the smallest thing that works.** Bring up one sensor cleanly before adding a second. Get one bit on the dashboard before designing the whole UI. Compound the wins.

**Document the trade off, not just the choice.** Every decision in embedded design closes some doors and opens others. The value is in being explicit about which.

<br/>

---

### Stack

```
hardware       FPGA · Nexys 4 DDR · MicroBlaze · STM32 · ESP32 · LoRa · Raspberry Pi
firmware       C · C++ · bare metal · RTOS · UART · SPI · I2C · interrupt driven design
fpga           VHDL · AXI · Vivado · Vitis · custom IP integration
intelligence   Python · NumPy · scikit-learn · signal DSP · edge inference
data           Power BI · Azure SQL · time series analysis
research       wireless sensor networks · anomaly detection · post quantum primitives
```

<br/>

---

### Background

```
2024 — 2026    MSc Computer Science Engineering        University of Debrecen, HU
2022 — 2024    MSc Infocommunication Technologies      SPbPU, Russia
2017 — 2021    BSc Infocommunication Technologies      SPbPU, Russia
```

<br/>

```
2026   1st place    GroundUP_eu Industrial Edge AI Hackathon
2026   2nd place    Student Research Conference TDK · OTDK nomination
2025   Award        TalentUD Excellence Initiative
2024   1st place    Student Research Award · Russia
```

<br/>

---

<div align="center">

<sub>Open to <b>research collaboration</b>, <b>embedded R&D positions</b>, and <b>FPGA based projects</b>.</sub>

<br/>

<sub>Reach me at <a href="mailto:amiltonkoxi2023@gmail.com">amiltonkoxi2023@gmail.com</a> or on <a href="https://www.linkedin.com/in/amiltonkoxi/">LinkedIn</a>.</sub>

</div>

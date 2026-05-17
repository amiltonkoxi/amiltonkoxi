<!-- =========================================================
     AMILTON KOXI · GitHub Profile README
     Design system: Tokyo Night
     Embedded Systems · FPGA · Edge AI · Intelligent Sensing
     ========================================================= -->

<div align="center">
  <img src="./media/banner.svg" width="100%" alt="Amilton Koxi · Embedded Systems · FPGA · Edge AI"/>
</div>

<br/>

<div align="center">
  <a href="https://github.com/amiltonkoxi">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=900&color=7AA2F7&center=true&vCenter=true&width=820&lines=Embedded+Systems+Engineer.;FPGA+%C2%B7+MicroBlaze+%C2%B7+Real+time+firmware.;From+sensor+pin+to+web+dashboard.;Hardware+first.+Research+driven."
         alt="Animated technical tagline"/>
  </a>
</div>

<br/>

<div align="center">

**I design intelligent embedded systems that survive real hardware, real noise, real constraints.**

</div>

<br/>

<div align="center">
  <a href="https://github.com/amiltonkoxi?tab=followers">
    <img src="https://img.shields.io/github/followers/amiltonkoxi?style=for-the-badge&logo=github&logoColor=white&label=Followers&labelColor=1A1B26&color=7AA2F7" alt="GitHub followers"/>
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=amiltonkoxi&style=for-the-badge&color=BB9AF7&base=1A1B26&label=Profile+views" alt="Profile views"/>
  &nbsp;
  <a href="https://www.linkedin.com/in/amiltonkoxi/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-7AA2F7?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=1A1B26" alt="LinkedIn"/>
  </a>
  &nbsp;
  <a href="mailto:amiltonkoxi2023@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-BB9AF7?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1A1B26" alt="Email"/>
  </a>
</div>

<br/>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`01` &nbsp; whoami

<table>
<tr>
<td width="62%" valign="top">

```yaml
name:        Amilton Koxi
role:        R&D Engineer · Embedded Systems · FPGA
focus:       Edge AI · Intelligent Sensing · Real time firmware
languages:   C · C++ · Python · VHDL
hardware:    Nexys 4 DDR · MicroBlaze · STM32 · ESP32 · LoRa
tools:       Vivado · Vitis · Git · Power BI · Azure SQL
education:   MSc Computer Science Engineering
research:    PhD candidate · Post quantum hardware acceleration
mindset:     Hardware first · System level thinking
open_to:     Research collaboration · Embedded R&D · FPGA projects
```

</td>
<td width="38%" valign="top">

### Why my work matters

Software demos are easy. Real systems are not.

I work on the parts most demos hide. Tight memory. Noisy signals. Strict timing. Hardware bring up. Lossy radio links. Microcontrollers that won't forgive a single wasted cycle.

That is where engineering actually happens, and that is where I want to be.

</td>
</tr>
</table>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`02` &nbsp; Currently

<table>
<tr>
<td width="33%" valign="top">

### `●` Building
**FMEAD FPGA**

Multi modal edge anomaly detector running on Nexys 4 DDR. MicroBlaze, real sensors, local feedback, Wi Fi telemetry.

`In progress`

</td>
<td width="33%" valign="top">

### `●` Researching
**Post quantum hardware**

FPGA oriented acceleration of cryptographic primitives for connected embedded systems.

`PhD direction`

</td>
<td width="33%" valign="top">

### `●` Exploring
**Reliable edge sensing**

Adaptive anomaly detection across edge, gateway, and fog layers in wireless sensor networks.

`Research`

</td>
</tr>
</table>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`03` &nbsp; Featured Work

<div align="center">

# FMEAD FPGA
### FPGA Multi Modal Edge Anomaly Detector

`VHDL` &nbsp;·&nbsp; `Bare metal C` &nbsp;·&nbsp; `MicroBlaze` &nbsp;·&nbsp; `Nexys 4 DDR` &nbsp;·&nbsp; `Edge AI`

</div>

<br/>

A real time edge platform that detects abnormal physical events directly on FPGA based hardware. It fuses motion, environmental, acoustic, and thermal signals, then exposes system status through local displays and a browser dashboard over Wi Fi.

The idea is simple. Detect meaningful events close to the sensors. No remote computer. No cloud roundtrip.

<br/>

<div align="center">
  <img src="./media/fmead-architecture.svg" width="100%" alt="FMEAD FPGA system architecture"/>
</div>

<br/>

<table>
<tr>
<td width="50%" valign="top">

#### What it does
- Reads motion data from an ADXL362 accelerometer
- Reads environmental data from a BME280 sensor
- Monitors FPGA die temperature through XADC
- Detects acoustic events from a PDM microphone
- Drives a 7 segment display and OLED for local status
- Serves a live dashboard through an ESP32 Wi Fi link
- Runs anomaly scoring entirely on the FPGA platform

</td>
<td width="50%" valign="top">

#### Engineering focus
- Sensor bring up over SPI and I2C
- AXI integration with MicroBlaze soft core
- Bare metal firmware with strict timing
- Custom VHDL peripheral integration
- Display refresh aligned with bus activity
- Memory safe dashboard payloads
- Embedded anomaly scoring without floats where possible

</td>
</tr>
</table>

<details>
<summary><b>&nbsp;Constraints I had to engineer around</b></summary>

<br/>

| Constraint | What it forced |
|---|---|
| Limited BRAM | Compact buffers, zero copy paths, tight telemetry frames |
| MicroBlaze budget | Polled SPI tuned per sensor, no busy waits where avoidable |
| Display timing | Refresh scheduled around AXI traffic to avoid flicker |
| Noisy real world data | Software filtering before any anomaly decision |
| ESP32 AT command limits | Strict state machine for socket and HTTP handling |
| HTML dashboard memory | Static page, minimal payloads, no per request allocation |

</details>

<br/>

<p align="right">
  <a href="https://github.com/amiltonkoxi/FMEAD-FPGA">
    <img src="https://img.shields.io/badge/Open%20repository-7AA2F7?style=for-the-badge&logo=github&logoColor=white&labelColor=1A1B26" alt="Open repository"/>
  </a>
</p>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`04` &nbsp; Engineering Portfolio

<table>
<tr>
<td width="50%" valign="top">

### SentinelNet
AI powered CBRNE edge platform for early threat detection and civil protection scenarios. Awarded 1st place at an international hackathon.

`Python` &nbsp; `Edge AI` &nbsp; `IoT` &nbsp; `Data`

</td>
<td width="50%" valign="top">

### WSN Swarm Anomaly Detection
Wireless sensor network anomaly detection with EWMA, Page Hinkley statistics, and PSO tuned thresholds across edge, gateway, and fog layers.

`ESP32` &nbsp; `Python` &nbsp; `C` &nbsp; `WSN`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### LoRa Telemetry System
Long range low power telemetry with sensor nodes, gateway, MQTT bridging, and link quality evaluation under real field conditions.

`LoRa` &nbsp; `MQTT` &nbsp; `STM32` &nbsp; `Embedded C`

</td>
<td width="50%" valign="top">

### 3D Motion Web Dashboard
Real time visualization of accelerometer data over Wi Fi, from FPGA hardware to a browser based 3D dashboard.

`JavaScript` &nbsp; `WebSocket` &nbsp; `ESP32` &nbsp; `Three.js`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### Nutriparse Reader
Computer vision pipeline for reading and parsing nutrition labels, designed with constrained inference in mind.

`Python` &nbsp; `OpenCV` &nbsp; `Computer Vision`

</td>
<td width="50%" valign="top">

### Banknote Detection
Vision based banknote recognition prototype focused on embedded deployment and lightweight image processing.

`Python` &nbsp; `OpenCV` &nbsp; `Machine Learning`

</td>
</tr>
</table>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`05` &nbsp; Technical Stack

<table>
<tr>
<td width="25%" valign="top" align="center">

#### Hardware
<br/>

![FPGA](https://img.shields.io/badge/FPGA-7AA2F7?style=flat-square&logoColor=white&labelColor=1A1B26)
![MicroBlaze](https://img.shields.io/badge/MicroBlaze-7DCFFF?style=flat-square&logoColor=white&labelColor=1A1B26)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white&labelColor=1A1B26)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white&labelColor=1A1B26)
![LoRa](https://img.shields.io/badge/LoRa-009688?style=flat-square&logoColor=white&labelColor=1A1B26)

</td>
<td width="25%" valign="top" align="center">

#### Firmware
<br/>

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black&labelColor=1A1B26)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white&labelColor=1A1B26)
![Bare metal](https://img.shields.io/badge/Bare%20metal-BB9AF7?style=flat-square&logoColor=white&labelColor=1A1B26)
![RTOS](https://img.shields.io/badge/RTOS-9ECE6A?style=flat-square&logoColor=white&labelColor=1A1B26)
![UART](https://img.shields.io/badge/UART%20%C2%B7%20SPI%20%C2%B7%20I2C-7DCFFF?style=flat-square&logoColor=white&labelColor=1A1B26)

</td>
<td width="25%" valign="top" align="center">

#### FPGA
<br/>

![VHDL](https://img.shields.io/badge/VHDL-7AA2F7?style=flat-square&logoColor=white&labelColor=1A1B26)
![AXI](https://img.shields.io/badge/AXI-BB9AF7?style=flat-square&logoColor=white&labelColor=1A1B26)
![Vivado](https://img.shields.io/badge/Vivado-FA7343?style=flat-square&logoColor=white&labelColor=1A1B26)
![Vitis](https://img.shields.io/badge/Vitis-EF4444?style=flat-square&logoColor=white&labelColor=1A1B26)
![Custom IP](https://img.shields.io/badge/Custom%20IP-9ECE6A?style=flat-square&logoColor=white&labelColor=1A1B26)

</td>
<td width="25%" valign="top" align="center">

#### Intelligence
<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white&labelColor=1A1B26)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white&labelColor=1A1B26)
![scikit](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white&labelColor=1A1B26)
![Edge AI](https://img.shields.io/badge/Edge%20AI-BB9AF7?style=flat-square&logoColor=white&labelColor=1A1B26)
![Signal DSP](https://img.shields.io/badge/Signal%20DSP-7DCFFF?style=flat-square&logoColor=white&labelColor=1A1B26)

</td>
</tr>
</table>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`06` &nbsp; Engineering Footprint

<div align="center">
  <img src="./media/engineering-footprint.svg" width="100%" alt="Engineering footprint dashboard with project counts, hardware platforms, recognitions, and language distribution"/>
</div>

<br/>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=amiltonkoxi&theme=tokyonight&no-frame=true&no-bg=true&column=7&margin-w=10&margin-h=10&title=Commits,Followers,Repositories,Experience,Stars,Issues,PullRequest" alt="GitHub trophies"/>
</div>

<br/>

<div align="center">
  <a href="https://github.com/amiltonkoxi">
    <img height="160" src="https://streak-stats.demolab.com/?user=amiltonkoxi&theme=tokyonight&background=1A1B26&ring=7AA2F7&fire=BB9AF7&currStreakLabel=7AA2F7&border=2D3047&hide_border=false&dates=C0CAF5&sideLabels=C0CAF5&currStreakNum=C0CAF5&sideNums=C0CAF5" alt="GitHub streak"/>
  </a>
  <a href="https://github.com/amiltonkoxi">
    <img height="160" src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=amiltonkoxi&theme=tokyonight&utcOffset=2" alt="Productive time distribution"/>
  </a>
</div>

<br/>

<div align="center">
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=amiltonkoxi&theme=tokyo-night&bg_color=1A1B26&color=7AA2F7&line=BB9AF7&point=7DCFFF&hide_border=false&border_color=2D3047&area=true" alt="Contribution graph"/>
</div>

<br/>

<div align="center">
<sub>Most of my hardware work lives outside GitHub. Bitstreams, lab measurements, signal traces, and academic deliverables don't fit a commit graph. The real footprint is in the projects above.</sub>
</div>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`07` &nbsp; Research Interests

<table>
<tr>
<td width="50%" valign="top">

### Edge Intelligence
On device anomaly detection under strict memory, timing, and energy budgets.

### FPGA Acceleration
Hardware acceleration of signal processing, embedded intelligence, and security primitives.

</td>
<td width="50%" valign="top">

### Wireless Sensor Networks
Reliable distributed sensing across edge, gateway, and fog architectures.

### Embedded Security
Post quantum cryptography and secure communication for IoT and connected systems.

</td>
</tr>
</table>

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`08` &nbsp; Recognition

```diff
+ 2026   1st place   International Edge AI Hackathon         SentinelNet
+ 2026   2nd place   Student Research Conference (TDK)       OTDK nomination
+ 2025   Award       Excellence Initiative scholarship       Research recognition
+ 2024   1st place   Student Research Award                  Wireless systems research
```

<div align="center">
  <img src="./media/divider.svg" width="100%" alt=""/>
</div>

<div align="center">

## Let's build systems that run on real hardware.

Open to **research collaboration**, **embedded R&D work**, **FPGA based projects**, and **long term technical opportunities**.

<br/>

<a href="https://www.linkedin.com/in/amiltonkoxi/">
  <img src="https://img.shields.io/badge/LinkedIn-Amilton%20Koxi-7AA2F7?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=1A1B26" alt="LinkedIn"/>
</a>
&nbsp;
<a href="mailto:amiltonkoxi2023@gmail.com">
  <img src="https://img.shields.io/badge/Email-Contact%20Me-BB9AF7?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1A1B26" alt="Email"/>
</a>
&nbsp;
<a href="https://github.com/amiltonkoxi">
  <img src="https://img.shields.io/badge/GitHub-amiltonkoxi-7DCFFF?style=for-the-badge&logo=github&logoColor=white&labelColor=1A1B26" alt="GitHub"/>
</a>

<br/><br/>

<sub>
<b>Embedded systems</b> &nbsp;·&nbsp; <b>FPGA</b> &nbsp;·&nbsp; <b>Edge AI</b> &nbsp;·&nbsp; <b>Wireless sensor networks</b> &nbsp;·&nbsp; <b>Research prototypes</b>
</sub>

<br/><br/>

<sub><i>Built with care. Tokyo Night palette. No em dashes were harmed.</i></sub>

</div>

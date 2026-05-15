<!-- =========================================================
     AMILTON KOXI · Personal Portfolio
     Design system: Tokyo Night
     Profile README · Embedded Systems · FPGA · Edge AI
     ========================================================= -->

<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Amilton Koxi · Embedded Systems · FPGA · Edge AI"/>
</div>

<br/>

<div align="center">
  <a href="https://github.com/amiltonkoxi">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3200&pause=1000&color=7AA2F7&center=true&vCenter=true&width=720&lines=Systems+that+sense%2C+decide%2C+and+run+close+to+hardware.;FPGA+%C2%B7+MicroBlaze+%C2%B7+Real-time+firmware+%C2%B7+Edge+intelligence.;From+sensor+pin+to+web+dashboard%2C+end+to+end."
         alt="Rotating tagline"/>
  </a>
</div>

<br/>

<div align="center">

I build embedded and FPGA based intelligent systems where sensing, firmware, hardware interfaces, and edge decision logic must work together under real constraints.

</div>

<br/>

<div align="center">
  <a href="https://www.linkedin.com/in/amiltonkoxi/"><kbd>&nbsp;&nbsp;<b>LinkedIn</b>&nbsp;&nbsp;</kbd></a>
  &nbsp;
  <a href="https://github.com/amiltonkoxi"><kbd>&nbsp;&nbsp;<b>GitHub</b>&nbsp;&nbsp;</kbd></a>
  &nbsp;
  <a href="#"><kbd>&nbsp;&nbsp;<b>Portfolio</b>&nbsp;&nbsp;</kbd></a>
  &nbsp;
  <a href="mailto:amiltonkoxi2023@gmail.com"><kbd>&nbsp;&nbsp;<b>Email</b>&nbsp;&nbsp;</kbd></a>
</div>

<br/>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`01` &nbsp; Profile

```yaml
name:        Amilton Koxi
role:        R&D Engineer
focus:       Embedded systems · FPGA · edge AI · intelligent sensing
languages:   C · C++ · Python · VHDL
hardware:    Nexys 4 DDR · MicroBlaze · STM32 · ESP32 · LoRa
tools:       Vivado · Vitis · Git · Power BI · Azure SQL
mindset:     Hardware first · research driven · system level thinking
open_to:     Research collaboration · embedded R&D · FPGA projects
```

I work on practical intelligent systems where software alone is not enough. My projects combine sensors, firmware, FPGA logic, communication modules, dashboards, and real time decision logic.

I am especially interested in systems that must survive real engineering limits: small memory, noisy signals, strict timing, hardware bring up, unreliable communication, and limited processing power.

The part many demos hide is usually the part I enjoy most.

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`02` &nbsp; Current Focus

<table>
<tr>
<td width="33%" valign="top">

### Building

**FMEAD FPGA**

A multi modal edge anomaly detector running on a Nexys 4 DDR board with MicroBlaze, sensors, local display feedback, and Wi Fi telemetry.

</td>
<td width="33%" valign="top">

### Researching

**Post quantum hardware acceleration**

FPGA oriented acceleration of cryptographic primitives for IoT and connected embedded systems.

</td>
<td width="33%" valign="top">

### Exploring

**Reliable edge sensing**

Adaptive anomaly detection for wireless sensor networks across edge, gateway, and fog layers.

</td>
</tr>
</table>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`03` &nbsp; Flagship Project

# FMEAD FPGA

**FPGA Multi Modal Edge Anomaly Detector**  
Nexys 4 DDR · MicroBlaze · VHDL · Bare metal C · Edge AI

FMEAD FPGA is a real time edge sensing platform that detects abnormal events directly on FPGA based embedded hardware. It combines motion, environmental, acoustic, and thermal signals, then exposes system status through local displays and a Wi Fi dashboard.

The goal is simple: detect meaningful physical events without depending on a remote computer or cloud service.

<br/>

<div align="center">
  <img src="./assets/fmead-architecture.svg" width="100%" alt="FMEAD FPGA system architecture"/>
</div>

<br/>

<table>
<tr>
<td width="58%" valign="top">

### What it does

- Reads motion data from an ADXL362 accelerometer
- Reads environmental data from a BME280 sensor
- Monitors FPGA temperature through XADC
- Detects simple acoustic events from a PDM microphone
- Displays local state using 7 segment display and OLED support
- Serves a browser dashboard through an ESP32 Wi Fi module
- Runs anomaly logic directly on the embedded FPGA platform

</td>
<td width="42%" valign="top">

### Engineering focus

- Sensor bring up over SPI and I2C
- AXI integration with MicroBlaze
- Bare metal firmware design
- Custom VHDL peripheral integration
- Real time display refresh
- Memory safe dashboard handling
- Embedded anomaly scoring

</td>
</tr>
</table>

<br/>

<table>
<tr>
<td width="50%" valign="top">

### Main constraints

- Limited BRAM
- Limited MicroBlaze processing budget
- Timing sensitive display updates
- Noisy real world sensor data
- ESP32 AT command limitations
- HTML dashboard memory pressure

</td>
<td width="50%" valign="top">

### Stack

`VHDL` &nbsp; `C` &nbsp; `MicroBlaze`  
`AXI` &nbsp; `SPI` &nbsp; `I2C` &nbsp; `UART`  
`Vivado` &nbsp; `Vitis` &nbsp; `ESP32 AT`  
`Nexys 4 DDR` &nbsp; `Bare metal firmware`

</td>
</tr>
</table>

<p align="right">
  <a href="https://github.com/amiltonkoxi/FMEAD-FPGA">
    <kbd>&nbsp;&nbsp;Open repository&nbsp;&nbsp;<b>→</b>&nbsp;&nbsp;</kbd>
  </a>
</p>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`04` &nbsp; Selected Projects

<table>
<tr>
<td width="50%" valign="top">

### FMEAD FPGA

Multi modal edge anomaly detector built on Nexys 4 DDR using MicroBlaze, VHDL peripherals, sensors, displays, and Wi Fi telemetry.

**Stack**  
`VHDL` `C` `MicroBlaze` `AXI` `ESP32`

</td>
<td width="50%" valign="top">

### SentinelNet

AI powered CBRNE edge platform for early threat detection and civil protection scenarios. Developed during an international hackathon.

**Stack**  
`Python` `Edge AI` `IoT` `Data Analysis`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### WSN Swarm Anomaly Detection

Wireless sensor network anomaly detection using EWMA, Page Hinkley statistics, and PSO based tuning across edge, gateway, and fog layers.

**Stack**  
`ESP32` `Python` `C` `WSN` `Anomaly Detection`

</td>
<td width="50%" valign="top">

### LoRa Communication System

Long range low power telemetry experiments with sensor nodes, gateway communication, MQTT bridging, and link quality evaluation.

**Stack**  
`LoRa` `MQTT` `STM32` `Embedded C`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### Nutriparse Reader

Computer vision pipeline for reading and parsing nutrition labels, designed with low resource inference in mind.

**Stack**  
`Python` `OpenCV` `Computer Vision`

</td>
<td width="50%" valign="top">

### Banknote Detection

Vision based banknote recognition prototype with a focus on embedded deployment and lightweight image processing.

**Stack**  
`Python` `OpenCV` `Machine Learning`

</td>
</tr>
</table>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`05` &nbsp; Technical Stack

<div align="center">
  <img src="./assets/tech-stack.svg" width="100%" alt="Technical stack overview"/>
</div>

<br/>

<table>
<tr>
<td width="25%" valign="top">

### Hardware

`FPGA`  
`MicroBlaze`  
`STM32`  
`ESP32`  
`Sensors`  
`LoRa`

</td>
<td width="25%" valign="top">

### Firmware

`C`  
`C++`  
`Bare metal`  
`Drivers`  
`UART`  
`SPI`  
`I2C`

</td>
<td width="25%" valign="top">

### FPGA

`VHDL`  
`AXI`  
`Vivado`  
`Vitis`  
`Custom IP`  
`Timing`

</td>
<td width="25%" valign="top">

### Intelligence

`Python`  
`Anomaly Detection`  
`Edge AI`  
`Signal Processing`  
`Data Analysis`  
`Visualization`

</td>
</tr>
</table>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`06` &nbsp; Research Interests

<table>
<tr>
<td width="50%" valign="top">

### Edge Intelligence

On device anomaly detection under strict memory, timing, and energy constraints.

### FPGA Acceleration

Hardware acceleration for signal processing, embedded intelligence, and security primitives.

</td>
<td width="50%" valign="top">

### Wireless Sensor Networks

Reliable sensing across distributed edge, gateway, and fog architectures.

### Embedded Security

Post quantum cryptography and secure communication for IoT and connected systems.

</td>
</tr>
</table>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`07` &nbsp; Selected Achievements

```diff
+ 2026   1st place · International edge AI hackathon · SentinelNet
+ 2026   2nd place · Student research conference · OTDK nomination
+ 2025   Excellence scholarship · Academic and research recognition
+ 2024   1st place · Student research award
```

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

## &nbsp;`08` &nbsp; Public Engineering Work

<table>
<tr>
<td width="50%" valign="top">

### Main Repository

**FMEAD FPGA**  
FPGA based multi modal edge anomaly detector with MicroBlaze, VHDL peripherals, sensors, displays, and Wi Fi telemetry.

<a href="https://github.com/amiltonkoxi/FMEAD-FPGA">
  <kbd>&nbsp;&nbsp;View repository&nbsp;&nbsp;→&nbsp;&nbsp;</kbd>
</a>

</td>
<td width="50%" valign="top">

### GitHub Focus

My public GitHub is focused on selected technical projects, documentation, embedded experiments, and research prototypes.

Most of my FPGA and research work is developed in private or research repositories.

</td>
</tr>
</table>

<br/>

<!-- ANIMATED STATS · live GitHub metrics -->
<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=amiltonkoxi&show_icons=true&hide=stars&theme=tokyonight&hide_border=true&bg_color=1A1B26&title_color=7AA2F7&icon_color=BB9AF7&text_color=A9B1D6&include_all_commits=true&count_private=true" alt="GitHub statistics"/>
  &nbsp;
  <img height="165" src="https://streak-stats.demolab.com?user=amiltonkoxi&theme=tokyonight&hide_border=true&background=1A1B26&ring=7AA2F7&fire=BB9AF7&currStreakLabel=7AA2F7&sideLabels=A9B1D6&dates=565F89" alt="GitHub streak"/>
</div>

<br/>

<!-- ANIMATED ACTIVITY GRAPH · contribution timeline -->
<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=amiltonkoxi&bg_color=1A1B26&color=7AA2F7&line=BB9AF7&point=9ECE6A&area=true&hide_border=true&custom_title=Contribution%20Activity" width="98%" alt="Contribution activity"/>
</div>

<br/>

<!-- SNAKE ANIMATION · contributions eaten over time -->
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/amiltonkoxi/amiltonkoxi/output/github-contribution-grid-snake-dark.svg"/>
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/amiltonkoxi/amiltonkoxi/output/github-contribution-grid-snake.svg"/>
    <img alt="GitHub contribution snake animation" src="https://raw.githubusercontent.com/amiltonkoxi/amiltonkoxi/output/github-contribution-grid-snake-dark.svg"/>
  </picture>
</div>

<sub>
Most of my embedded, FPGA, and research work is developed in private or academic repositories. The public projects shown here are a selected technical snapshot.
</sub>

<div align="center">
  <img src="./assets/divider.svg" width="100%" alt=""/>
</div>

<div align="center">

## Let's build systems that run on real hardware.

I am open to research collaboration, embedded R&D work, FPGA based projects, and long term technical opportunities.

<br/>

<a href="https://www.linkedin.com/in/amiltonkoxi/"><kbd>&nbsp;&nbsp;<b>LinkedIn</b>&nbsp;&nbsp;</kbd></a>
&nbsp;
<a href="mailto:amiltonkoxi2023@gmail.com"><kbd>&nbsp;&nbsp;<b>Email</b>&nbsp;&nbsp;</kbd></a>
&nbsp;
<a href="https://github.com/amiltonkoxi"><kbd>&nbsp;&nbsp;<b>GitHub</b>&nbsp;&nbsp;</kbd></a>

</div>

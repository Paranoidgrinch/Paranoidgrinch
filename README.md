<div align="center">


  
  <a href="./bab_readme_banner.mp4">
    <img
      src="./bab_readme_banner.gif"
      width="100%"
      alt="Animated Bureaucrats and Broomsticks card banner"
    >
  </a>

  <br><br>

  <h1>
    Hi, I'm
    <a href="https://github.com/Paranoidgrinch">@Paranoidgrinch</a>
  </h1>

  <h3>
    Systems programmer building deterministic roguelike infrastructure
    and scientific software.
  </h3>

  <p>
    I develop software for game systems, accelerator mass spectrometry,<br>
    Gaussian optics, and laboratory automation.
  </p>

  <p>
    <a href="https://moonvineforge.com">
      <img
        src="https://moonvineforge.com/assets/moonvine-forge-logo.jpg"
        width="28"
        alt="Moonvine Forge Studios logo"
      >
    </a>
    &nbsp;
    <a href="https://moonvineforge.com">
      <strong>Moonvine Forge Studios</strong>
    </a>
  </p>

  <br>
<p>
  <a href="https://github.com/Paranoidgrinch/RogueDeck-Core">
      <img
        src="https://img.shields.io/github/stars/Paranoidgrinch/RogueDeck-Core?style=for-the-badge&logo=github&logoColor=white&label=STAR%20ROGUEDECK%20CORE&color=512BD4"
        height="32"
        alt="Star RogueDeck Core"
      >
    </a>
</p>
  <p>
    <a href="https://committers.top/germany">
      <img
        src="https://user-badge.committers.top/germany/Paranoidgrinch.svg"
        height="38"
        alt="Paranoidgrinch on committers.top Germany"
      >
    </a>
  </p>

  <p>
    <a href="https://studio.moonvineforge.com">
      <img
        src="https://img.shields.io/badge/OPEN-ROGUEDECK%20STUDIO-6B7D58?style=for-the-badge"
        height="32"
        alt="Open RogueDeck Studio"
      >
    </a>
  </p>

  

</div>

---

## RogueDeck

### [RogueDeck Core](https://github.com/Paranoidgrinch/RogueDeck-Core)

**A complete, deterministic C#/.NET engine foundation for roguelike deckbuilders.**

RogueDeck separates rules, content and presentation. Cards, statuses, resources, triggers, targets,
run events and maps are composed from reusable systems instead of accumulating hardcoded exceptions.

> Build the mechanic. Keep the core clean.

- deterministic combat, seeded runs, snapshots and replay
- modular effect programs, triggers, modifiers and interceptors
- combat and run systems for parties, relics, events, shops, branching maps and meta progression
- versioned JSON content, Godot integration and extensive automated testing

[![CI](https://github.com/Paranoidgrinch/RogueDeck-Core/actions/workflows/ci.yml/badge.svg)](https://github.com/Paranoidgrinch/RogueDeck-Core/actions/workflows/ci.yml)
![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Status](https://img.shields.io/badge/core-v1_complete-3FB950?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-394B59?style=flat-square)

### [RogueDeck Studio](https://studio.moonvineforge.com)

**Forge a whole roguelike in the browser — no account, setup or code required.**

Author heroes, cards, enemies, encounters, statuses, relics, events, shops, meta rules and branching
maps; playtest the result immediately; then export the complete game as one versioned JSON blueprint
for a Godot/.NET frontend or another RogueDeck host.

**[Open RogueDeck Studio →](https://studio.moonvineforge.com)**

<sub>
RogueDeck grew out of
<a href="https://github.com/Paranoidgrinch/bureaucrats-and-broomsticks-v2">Bureaucrats &amp; Broomsticks</a>,
the original playable Python systems prototype that exposed the limits of hardcoded combat logic.
</sub>

---

## Science and engineering

I work in **accelerator mass spectrometry (AMS)**, where I transport and cool negative-ion beams,
overlap them with high-power laser light and automate the hardware around the experiment.

### Accelerator mass spectrometry and laser photodetachment

- rare-isotope measurements and molecular-anion beams
- high-power laser photodetachment and laser-based isobar suppression
- ion–laser beam overlap, beam transport and diagnostics
- RFQ ion cooling, injection and extraction
- automated experimental control and reproducible measurement workflows

### Ion optics, RFQ systems and Gaussian laser propagation

- SIMION particle-trajectory simulations and automated parameter scans
- electrostatic lenses, deflectors and electrode geometries
- RF matching and resonant LC systems
- Gaussian-beam transport through long beamlines and constrained apertures

### [Gaussian Beamline Designer](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer)

A released PyQt5 desktop application for designing and evaluating paraxial Gaussian laser beamlines.
It propagates elliptical beams independently in both axes through free space, thin or thick lenses,
apertures, mirrors and restricted beam-tube regions. Projects and simulation results can be exported
as JSON, CSV and PNG.

[![Release](https://img.shields.io/badge/release-v1.0.0-3FB950?style=flat-square)](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer/releases/latest)
[![Tests](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer/actions/workflows/tests.yml/badge.svg)](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer/actions/workflows/tests.yml)
![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat-square&logo=python&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-394B59?style=flat-square)

### Experimental automation

- Beckhoff PLC systems, TwinCAT and IEC 61131-3 Structured Text
- Python and PyQt5 control interfaces
- LabVIEW and instrument communication
- MQTT and Raspberry Pi monitoring
- serial and TCP/IP hardware control

### Molecular-anion calculations

I use PySCF and automated Python workflows to investigate:

- electron affinities and dissociation energies
- molecular geometries and electronic structure
- rotational constants and vibrational properties
- photodetachment channels and experimentally promising molecular anions

### Related research software

| Project | Focus |
| --- | --- |
| [**FLAVIA**](https://github.com/Paranoidgrinch/FLAVIA-alpha-1.1-Fully-integrated-Laser-Anion-Variables-for-AMS-) | Integrated controls and tools for laser–anion experiments in AMS |
| [**Verdi V18 Controller**](https://github.com/Paranoidgrinch/VerdiV18) | Python/PyQt5 control and monitoring for a high-power Verdi laser |
| [**RFQ resonance control**](https://github.com/Paranoidgrinch/LC-Circuit-flashing) | Remote monitoring and adjustment of the ion cooler's resonant LC-matching system |
| [**Beckhoff CX7080 + MQTT**](https://github.com/Paranoidgrinch/Beckhoff-CX7080-MQTT) | PLC communication and laboratory-system integration |

---

## Toolset

### Game and software development

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_10-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Blazor](https://img.shields.io/badge/Blazor-WebAssembly-512BD4?style=flat-square&logo=blazor&logoColor=white)
![Godot](https://img.shields.io/badge/Godot-.NET-478CBF?style=flat-square&logo=godotengine&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-292929?style=flat-square&logo=json&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)

### Scientific computing and simulation

![PySCF](https://img.shields.io/badge/PySCF-Electronic_Structure-4A5568?style=flat-square)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![SIMION](https://img.shields.io/badge/SIMION_8.1-Ion_Optics-5C677D?style=flat-square)
![Lua](https://img.shields.io/badge/Lua-SIMION_Automation-2C2D72?style=flat-square&logo=lua&logoColor=white)
![Fusion 360](https://img.shields.io/badge/Fusion_360-CAD-EF7C00?style=flat-square&logo=autodesk&logoColor=white)

### Automation and instrumentation

![LabVIEW](https://img.shields.io/badge/LabVIEW-Instrument_Control-F2C811?style=flat-square)
![PyQt5](https://img.shields.io/badge/PyQt5-Control_Interfaces-41CD52?style=flat-square&logo=qt&logoColor=white)
![Beckhoff](https://img.shields.io/badge/Beckhoff-PLC_Automation-D71920?style=flat-square)
![TwinCAT](https://img.shields.io/badge/TwinCAT_3-Control_Systems-C8102E?style=flat-square)
![Structured Text](https://img.shields.io/badge/IEC_61131--3-Structured_Text-44546A?style=flat-square)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![RS-232](https://img.shields.io/badge/RS--232-Serial_Control-44546A?style=flat-square)
![TCP/IP](https://img.shields.io/badge/TCP%2FIP-Instrument_Control-44546A?style=flat-square)

---

<div align="center">

I like systems that remain understandable when the interactions become complicated — whether they
move cards through a combat queue or ions through a beamline.

<br>

[**RogueDeck Studio**](https://studio.moonvineforge.com) ·
[**Moonvine Forge**](https://moonvineforge.com) ·
[**GitHub**](https://github.com/Paranoidgrinch)

</div>

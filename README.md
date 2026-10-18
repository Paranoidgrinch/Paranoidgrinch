<!-- One animated card on each side, cropped from bab_readme_banner.mp4. -->
<table align="center" width="100%">
  <tr>
    <td align="center" valign="middle" width="22%">
      <img src="./bnb_card_left.gif" width="100%" alt="Animated Bureaucrats &amp; Broomsticks card back — left">
    </td>
    <td align="center" valign="middle" width="56%">
      <h2>Hi, I'm <a href="https://github.com/Paranoidgrinch">@Paranoidgrinch</a></h2>
      <p><strong>Game systems &amp; scientific software</strong></p>
      <p>I build a deterministic engine for roguelike deckbuilders — and the software that runs and models laser-assisted accelerator mass spectrometry.</p>
      <p><a href="https://moonvineforge.com"><strong>Moonvine Forge Studios</strong></a></p>
      <p><a href="https://github.com/Paranoidgrinch/RogueDeck-Core"><img alt="Star RogueDeck Core" src="https://img.shields.io/github/stars/Paranoidgrinch/RogueDeck-Core?style=for-the-badge&amp;logo=github&amp;logoColor=white&amp;label=ROGUEDECK%20CORE&amp;color=512BD4"></a></p>
      <p><a href="https://studio.moonvineforge.com"><img alt="Open RogueDeck Studio" src="https://img.shields.io/badge/OPEN-ROGUEDECK%20STUDIO-6B7D58?style=for-the-badge"></a></p>
    </td>
    <td align="center" valign="middle" width="22%">
      <img src="./bnb_card_right.gif" width="100%" alt="Animated Bureaucrats &amp; Broomsticks card back — right">
    </td>
  </tr>
</table>

<p align="center">
  <a href="https://committers.top/germany"><img src="https://user-badge.committers.top/germany/Paranoidgrinch.svg" height="24" alt="GitHub public-commit ranking in Germany"></a>
</p>

---

## 🎴 Games — RogueDeck

### [RogueDeck Core](https://github.com/Paranoidgrinch/RogueDeck-Core)

**A deterministic C#/.NET engine for roguelike deckbuilders, independent of any game UI.**

Mechanics are composed from effect programs and typed events instead of a growing pile of card-specific
exceptions. The same seed and the same decisions always produce the same run — so every run can be
snapshotted, hashed, replayed and tested.

- **Combat engine:** effects, triggers, targets, statuses, resources and modifier/interceptor pipelines.
- **Run engine:** characters, decks, relics, encounters, events, shops and generated branching maps across acts.
- **Tooling:** a scenario DSL, an automated play bot with run replay, fuzzing and ~2,700 tests in CI.

[![CI](https://github.com/Paranoidgrinch/RogueDeck-Core/actions/workflows/ci.yml/badge.svg)](https://github.com/Paranoidgrinch/RogueDeck-Core/actions/workflows/ci.yml)
![.NET](https://img.shields.io/badge/.NET-10-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![License](https://img.shields.io/badge/license-PolyForm%20Noncommercial-394B59?style=flat-square)

### [RogueDeck Studio](https://studio.moonvineforge.com) — build a deckbuilder without code

**Design and playtest a complete roguelike deckbuilder in your browser.** Create cards, characters, enemies,
encounters, relics, events, shops and maps; play them on the real engine; export the result as a versioned
JSON blueprint that any RogueDeck host can run.

[**Open RogueDeck Studio →**](https://studio.moonvineforge.com)

### Bureaucrats & Broomsticks — the game built on RogueDeck

A satirical fantasy roguelike deckbuilder about magic, paperwork and deeply questionable career choices —
five acts from the City Offices to the Divine Ledger. The game is split across four repositories:

| Repository | Role |
| --- | --- |
| [**RogueDeck-Core**](https://github.com/Paranoidgrinch/RogueDeck-Core) | the rules: combat and run engine, bot, replay |
| [**bnb-content**](https://github.com/Paranoidgrinch/bnb-content) | the game itself as data — converts and validates the content into `game.roguedeck.json` |
| [**bnb-godot**](https://github.com/Paranoidgrinch/bnb-godot) | the Godot 4 (.NET) frontend: screens, cards, art, music, bug reports |
| [**bnb-runs**](https://github.com/Paranoidgrinch/bnb-runs) | every playtest run, recorded as seed + decisions and replayable step for step |

<sub>It started as <a href="https://github.com/Paranoidgrinch/bureaucrats-and-broomsticks-v2">a hardcoded Python terminal prototype</a> — its limits are why RogueDeck exists.</sub>

---

## 🔬 Science — laser-assisted AMS at CologneAMS

My research at **CologneAMS** brings together ion-beam physics, high-power lasers and experimental
automation. For **²⁶Al AMS**, I investigate selective photodetachment of the interfering **MgO⁻** while
transmitting **AlO⁻**, using a helium-filled RFQ ion cooler and a continuous-wave **532 nm laser**. The
central trade-off: suppress the molecular isobar without losing the ions the measurement needs.

I model collision-induced losses and ion transport through the RFQ, simulate electrostatic ion optics in
**SIMION**, and evaluate ion–laser overlap and beamline transmission — and I write the software that runs the
experiment and computes the molecular data it depends on.

### [OpenEA Benchmark](https://github.com/Paranoidgrinch/openea-benchmark) — two atoms in, electron affinity out

Photodetachment only works if you know the electron affinity — and for most diatomic molecules nobody has
measured it. **OpenEA computes the adiabatic electron affinity EA₀ of a diatomic molecule from nothing but its
two element symbols**, fully automatically and without reference data.

It discovers the competing electronic states of neutral and anion, builds CCSD(T) potential curves, goes to
the complete-basis-set limit and adds core-valence, relativistic, spin–orbit, post-CCSD(T), multireference and
zero-point corrections only where diagnostics call for them. The result is an evidence-based interval — or
`UNBOUND`, or `UNRESOLVED` with the reason.

| | OH | CN | NO | O₂ | ClO | AlO | C₂ | N₂ |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **OpenEA (eV)** | 1.828 | 3.861 | 0.022 | 0.444 | 2.279 | 2.613 | 3.286 | `UNBOUND` |
| **Experiment (eV)** | 1.828 | 3.862 | 0.026 | 0.448 | 2.276 | 2.60 | 3.269 | unbound |

Built entirely on open-source quantum chemistry: **PySCF**, **CCpy** and **OpenMolcas**. Transition-metal and
heavy-element molecules are the next validation step.

[**Explore OpenEA Benchmark →**](https://github.com/Paranoidgrinch/openea-benchmark)
![Python](https://img.shields.io/badge/Python-quantum%20chemistry-3776AB?style=flat-square&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/status-validation-D29922?style=flat-square)
![License](https://img.shields.io/badge/license-GPL--3.0-394B59?style=flat-square)

<sub>Its predecessor, <a href="https://github.com/Paranoidgrinch/diatomic-ea"><strong>DiatomicEA</strong></a>, is a released desktop app that estimates EAs from a fixed DFT ensemble with calibrated prediction intervals — fast, but limited by DFT. OpenEA replaces that with state-resolved coupled-cluster theory.</sub>

### [FLAVIA](https://github.com/Paranoidgrinch/FLAVIA-alpha-1.1-Fully-integrated-Laser-Anion-Variables-for-AMS-) — control system for the laser-AMS beamline

**FLAVIA (Fully integrated Laser-Anion Variables for AMS) runs the experimental setup I work on.** One PyQt5
application controls the ion source, ion optics, analyzing magnet, RFQ ion cooler, Faraday cups, current
measurement, vacuum monitoring and the legacy Tandetron controls — over MQTT (Beckhoff PLC), TCP/IP and serial
devices. It records 1D/2D beam scans, saves and restores complete machine configurations, and tracks sample
exposure.

[![FLAVIA](https://img.shields.io/badge/explore-FLAVIA-3FB950?style=flat-square)](https://github.com/Paranoidgrinch/FLAVIA-alpha-1.1-Fully-integrated-Laser-Anion-Variables-for-AMS-)
![Python](https://img.shields.io/badge/Python-PyQt5-3776AB?style=flat-square&logo=python&logoColor=white)
![License](https://img.shields.io/badge/license-GPL--3.0-394B59?style=flat-square)

### [Gaussian Beamline Designer](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer)

**A released PyQt5 application for paraxial laser-beam design.** It propagates elliptical Gaussian beams
independently in x and y through lenses, mirrors, apertures and beam tubes using ABCD optics, with
reproducible JSON projects and CSV/PNG exports.

[![Release](https://img.shields.io/badge/release-v1.0.0-3FB950?style=flat-square)](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer/releases/latest)
[![Tests](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer/actions/workflows/tests.yml/badge.svg)](https://github.com/Paranoidgrinch/Gaussian-Beamline-Designer/actions/workflows/tests.yml)
![License](https://img.shields.io/badge/license-MIT-394B59?style=flat-square)

### More lab tools

| Project | What it does |
| --- | --- |
| [**SIRIUS**](https://github.com/Paranoidgrinch/SIRIUS) / [**mcsirius**](https://github.com/Paranoidgrinch/mcsirius) | Automated, physics-informed beam tuning on top of FLAVIA — full beamline / source-to-Cup-1. |
| [**Verdi V18 Controller**](https://github.com/Paranoidgrinch/VerdiV18) | Remote control and monitoring for the 532 nm high-power CW laser. |
| [**RFQ resonance control**](https://github.com/Paranoidgrinch/LC-Circuit-flashing) | Raspberry Pi software that tunes the LC matching of the RFQ to resonance. |
| [**Beckhoff CX7080 + MQTT**](https://github.com/Paranoidgrinch/Beckhoff-CX7080-MQTT) | TwinCAT PLC programs that publish the ion-cooler hardware over MQTT. |

---

## Toolset

| Area | Languages, frameworks & tools |
| --- | --- |
| **Game systems** | C#, .NET 10, Godot 4, Blazor WebAssembly, JSON, GitHub Actions |
| **Scientific computing** | Python, PySCF, CCpy, OpenMolcas, NumPy, SIMION, Lua, PyQt5 |
| **Instrumentation** | TwinCAT 3, IEC 61131-3, LabVIEW, MQTT, Raspberry Pi, serial, TCP/IP |

<p align="center">
  I like building systems that can be tested and understood — whether they resolve combat events or steer ions through an accelerator.<br>
  <a href="https://studio.moonvineforge.com">RogueDeck Studio</a> ·
  <a href="https://moonvineforge.com">Moonvine Forge</a> ·
  <a href="https://github.com/Paranoidgrinch">GitHub</a>
</p>

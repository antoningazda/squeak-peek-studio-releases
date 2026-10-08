<div align="center">

<img src="https://antoningazda.github.io/squeak-peek-studio-releases/assets/logo.png" alt="Squeak Peek Studio" width="140">

# Squeak Peek Studio

**Detect, classify, review and listen to ultrasonic vocalizations (USVs) of laboratory rodents**
— a desktop application with a matching headless CLI.

[![Latest release](https://img.shields.io/github/v/release/antoningazda/squeak-peek-studio-releases?label=latest&style=for-the-badge&color=009688)](https://github.com/antoningazda/squeak-peek-studio-releases/releases/latest)
[![Documentation](https://img.shields.io/badge/docs-read-ff7043?style=for-the-badge)](https://antoningazda.github.io/squeak-peek-studio-releases/)
[![Downloads](https://img.shields.io/github/downloads/antoningazda/squeak-peek-studio-releases/total?style=for-the-badge&color=607d8b)](https://github.com/antoningazda/squeak-peek-studio-releases/releases)

</div>

## ⬇️ Download

| Platform | Installer | |
|---|---|---|
| **macOS** 12+ | [`SqueakPeekStudio-macOS.dmg`](https://github.com/antoningazda/squeak-peek-studio-releases/releases/latest/download/SqueakPeekStudio-macOS.dmg) | Open, drag to Applications |
| **Windows** 10/11 | [`SqueakPeekStudio-windows-Setup.exe`](https://github.com/antoningazda/squeak-peek-studio-releases/releases/latest/download/SqueakPeekStudio-windows-Setup.exe) | Installer · or the portable [`.zip`](https://github.com/antoningazda/squeak-peek-studio-releases/releases/latest/download/SqueakPeekStudio-windows.zip) |
| **Linux** 64-bit | [`SqueakPeekStudio-linux.tar.gz`](https://github.com/antoningazda/squeak-peek-studio-releases/releases/latest/download/SqueakPeekStudio-linux.tar.gz) | Extract and run |

The links always point at the **[latest release](https://github.com/antoningazda/squeak-peek-studio-releases/releases/latest)**
(release notes and older versions: [all releases](https://github.com/antoningazda/squeak-peek-studio-releases/releases)).
No Python needed.

> [!NOTE]
> The builds are not yet code-signed, so macOS and Windows warn on first
> launch. The [install guide](https://antoningazda.github.io/squeak-peek-studio-releases/install/)
> shows how to open the app anyway.

## 📖 Documentation

**<https://antoningazda.github.io/squeak-peek-studio-releases/>**

| Start here | Go deeper |
|---|---|
| [Install](https://antoningazda.github.io/squeak-peek-studio-releases/install/) — per-platform steps, first launch | [Methods](https://antoningazda.github.io/squeak-peek-studio-releases/methods/) — how each detector works and how to tune it |
| [Quickstart](https://antoningazda.github.io/squeak-peek-studio-releases/quickstart/) — first detection in about five minutes | [Training models](https://antoningazda.github.io/squeak-peek-studio-releases/training/) — ML / CNN detectors, call-type classifier |
| [User guide](https://antoningazda.github.io/squeak-peek-studio-releases/guide/) — every tab of the app | [File formats](https://antoningazda.github.io/squeak-peek-studio-releases/file-formats/) — labels, settings, model folders |
| [CLI reference](https://antoningazda.github.io/squeak-peek-studio-releases/cli/) · [CLI workflows](https://antoningazda.github.io/squeak-peek-studio-releases/workflows/) | [Troubleshooting](https://antoningazda.github.io/squeak-peek-studio-releases/troubleshooting/) |

## What it does

Rats and mice talk in the 40–120 kHz band, far above human hearing. Squeak
Peek Studio turns raw high-sample-rate WAV recordings into a scrollable
spectrogram, a list of detected calls, call types assigned by a trained
model, an interface for accepting or correcting each one, and audio you can
hear.

| | |
|---|---|
| 🔎 **Detect** | Five engines — PSD, BSCD, RBD, a Random Forest frame classifier and a Faster R-CNN box detector. Run several at once and compare. |
| 🏷️ **Classify** | Two-stage model: a CNN separates USV from noise, a Random Forest assigns the call type and flags uncertain calls for review. Train your own on your labels. |
| ✅ **Review** | Step through calls one key at a time, accept or reject each detection and call type, correct mistakes, export. |
| 🎧 **Listen** | Pitch-shifted sonification brings 70 kHz calls into your headphones; export video with the spectrogram and sonified audio. |
| 📊 **Measure** | Score any label set against reference labels — TP / FP / FN, precision, recall, F1. |
| ⚙️ **Automate** | Everything the GUI does, `squeak-peek-cli` does headlessly over whole folders. |

## Credits

A Python reimplementation and extension of the MATLAB application developed
by **Ing. Antonín Gazda** as a Master's thesis at the **Czech Technical
University in Prague, Faculty of Electrical Engineering (FEL)** (May 2025),
in collaboration with the **National Institute of Mental Health (NUDZ)**.
[Thesis record →](https://dspace.cvut.cz/entities/publication/dede5152-081b-41cf-a4ba-55dacad884d5)

If you use Squeak Peek Studio in published work, please cite the thesis.
Questions and bug reports: [antonin.gazda@gmail.com](mailto:antonin.gazda@gmail.com).
MIT licensed.

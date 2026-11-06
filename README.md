# VSroom (v1.0)

**VSroom** is a lightweight, simplified vocal synthesis application designed to revive legacy voicebanks—specifically **EVA-10** and **LUMIOUS LUMI**—alongside new additions, giving them a distinct, standalone home. 

Even though most people on GitHub share the inside code, mine is just an HTML to Python wrapper and it's very simple. In the website world many people steal codes, and I haven't found out how to stop someone from right-clicking yet, so I can't put it on a site.

---

## 🎤 Supported Voicebanks

| Voicebank | Status |
| :--- | :--- |
| **EVA-10** | Revived |
| **LUMIOUS LUMI** | Revived |
| **Hana** | New |

### Language Support
* **Chinese**
* **Japanese**
* **Khmer**
* **English**

---

## ⚙️ Core Mechanics & Technical Limitations

VSroom is built with explicit functional constraints for focused, simplified rendering. Please keep the following operational rules in mind:

### 1. Single Singer Rule
* **One Voicebank per Sequence:** UST project files must contain instructions for only **one singer at a time**. Attempting to run multi-voice UST files will result in rendering issues or engine errors.

### 2. Track & Stem Export
* **No Multi-Track Stems:** The engine does not handle internal multi-track mixing. 
* To compose a song with background vocals, harmonies, or a chorus, **export separate `.wav` files** for each track/melody line and blend them in your DAW.

### 3. Fixed Pitch Processing (No Pitch Bends)
* **Pitch Bends Ignored:** VSroom bypasses custom UST pitch curves, portamento, and pitch-bend data entirely.
* **Standard Note Playback:** Any note with pitch-bend automation (such as a downward drop or slide) will play strictly at its base pitch value without the bend effect.

---

## 🛠 Usage Guidelines

1. Load your single-singer `.ust` file into VSroom.
2. Select one of the available voicebanks (EVA-10, LUMIOUS LUMI, or Hana).
3. Export your rendered `.wav` stem.
4. Repeat for additional layers (harmonies/lead) and import into your preferred audio editing software.
(or just mess around)


---

## 🙏 Acknowledgments

* **pywebview** – For providing the lightweight native window bridge that safely wraps web code into a desktop application.

* **PyInstaller** – For packing everything into a clean standalone .exe.
* **UTAU** – For pioneering the `.ust` file format that powers VSroom's sequence input.

---

## ⚠️ Repository & Forking Rules

> **PLEASE READ BEFORE FORKING:**
> Public forks of this repository are **strictly prohibited** without reviewing and agreeing to the Fork Terms of Service. Because the distribution build utilizes compiled executable wrappers to protect source files, unauthorized cloning, decompilation, or redistribution of underlying assets is not permitted.

---

## 🔮 Future Vision

VSroom started as a lightweight project, but we hope to continue developing it into a much bigger platform for legacy and custom voicebanks. Thank you for using and supporting VSroom!

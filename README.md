# Whammonizer-H9-Whammy-midi-controller
# Whammonizer  Whammonizer is an open-source MIDI foot controller designed to control Eventide H9 and Digitech Whammy 5 pedals.  Dual mode operation, instant visual feedback, and performance-oriented workflow make it ideal for live musicians. 

# 🎛️ Whammonizer

**Whammonizer** is a DIY MIDI foot controller designed to control both an  
**Eventide H9** and a **Digitech Whammy 5**, with a simple, robust, and performance-oriented interface.

The project is based on an **Arduino Uno**, features **8 footswitches**, **8 LEDs**, a **16×2 LCD**,  
and communicates via **MIDI DIN**.

---

## ✨ Features

### 🎹 H9 Mode
- 8 footswitches → 8 harmonizer presets
- Each footswitch sends **4 simultaneous Control Change messages** currently setup on the Quadravox algorithm en the 4 different pich settings sending values to cc 22,23,27,28
- CC values remain active after the button is pressed
- **Preset names displayed** on the LCD
- LEDs indicate the active preset

### 🎸 Whammy Mode
- **Digitech Whammy 5** control via **Program Change**
- Direct access to Whammy / Harmony modes
- **Real Whammy preset names** shown on the LCD
- LEDs synchronized with the selected preset

### 🔀 Mode Switching
- Long press **FS1 + FS5 (2 seconds)**:
  - toggles between **H9 Mode** and **Whammy Mode**
  - fast LED blinking confirms the mode change
  - LCD message: `Mode: H9` or `Mode: Whammy`

---

## 🧱 Hardware

- Arduino Uno
- 8 × momentary footswitches
- 8 × LEDs (with resistors)
- 16×2 I2C LCD (72 × 25 mm)
- 5-pin MIDI DIN output
- MIDI resistors (220 Ω)
- **MP1584** buck converter (9V → 5V)
- **Hammond 1590DD** enclosure (188 × 120 × 37 mm)

---

## 🔌 Main Connections

- Footswitches: matrix scanning (2 rows × 4 columns)
- LEDs: A0, A1, A2, A3, 10, 11, 12, 13
- MIDI OUT: DIN 5-pin
- LCD: I2C (SDA / SCL)

---

## 🖥️ User Interface

- Two rows of 4 footswitches
- Centered LCD screen
- LED rows:
  - below the top footswitch row
  - above the bottom footswitch row
- Layout optimized for live performance

---

## 🧪 Project Status

✅ Fully functional  
✅ Tested with Eventide H9 and Digitech Whammy 5  
✅ Ready for enclosure integration  
✅ Documented for open-source sharing  




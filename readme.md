# 3.3V MicroSD Card SPI Breakout Board

A compact, high-performance, 2-layer **MicroSD Card Breakout Board** designed in KiCad for embedded microcontrollers using the **SPI (Serial Peripheral Interface)** bus.

Designed specifically for 3.3V native logic ecosystems (STM32, ESP32, RP2040, SAMD, Nordic, etc.), this module provides clean power decoupling, signal pull-ups, and a low-EMI ground plane layout.

---

## Board Renders

| Top View | Bottom View |
| :---: | :---: |
| ![3D Top Render](Images/3d_render_top.png) | ![3D Bottom Render](Images/3d_render_bottom.png) |

---

## Key Features

* **Native 3.3V Operation:** Designed without slow active/passive level shifters, maximizing SPI bus speeds (up to 25 MHz) with zero signal propagation delay.
* **Transient Power Decoupling:** Dedicated 10 uF bulk ceramic cap (C1) and 100 nF high-frequency ceramic cap (C2) positioned directly adjacent to the SD socket's VDD pin (Pin 4) to handle flash memory write current spikes (up to 200 mA).
* **Bus Stability:** Integrated 10k Ohm pull-up resistors on signal lines to prevent floating inputs and accidental bus writes during microcontroller startup/reset.
* **Card Detection:** Mechanically broken-out Card Detect (CD_DET) line to trigger hardware interrupts on card insertion/removal.
* **Optimized 2-Layer Signal Integrity:** Signal routing optimized for continuous return paths over an unbroken bottom Ground plane, minimizing EMI and clock ringing.
* **Standard 2.54mm Header:** 1x7 pin header footprint for breadboard prototyping or jumper wiring.

---

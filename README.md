# EngineLab

**A virtual engine lab in your browser:** you can do the experiment, explore 26 engines in 3D, and build and tune your own engine in a 3D garage. It works in English, Arabic and Hindi, on phones and computers, and also offline once installed.

**Open it:** https://moha701.github.io/enginelab/

Created by **Mohammed Hamed Al-Shabibi** (Instagram [@mhmd8p2](https://instagram.com/mhmd8p2)), University of Technology and Applied Sciences – Ibra.

---

## What you can do

| | |
|---|---|
| **Do the lab** | The CT 150 four-stroke petrol engine experiment on the CT 159 test stand, step by step. You prepare the stand, start the engine, load it with the brake, time the fuel and record your readings. The observation table, graphs and worked calculations fill in as you go, and you can export a lab report (print, Excel or web page). |
| **Learn the engines** | 26 engines in 3D: inline, V, W and boxer car engines, diesel, Wankel, two-stroke, opposed-piston, radial, turbofan, liquid rocket, steam, Stirling, electric motor and hydrogen fuel cell. Every moving part is animated and the sound is made live from the engine's firing order. |
| **Build in the garage** | Fit turbos, superchargers, carburettors, cams, heads, exhausts, nitrous, gearboxes and race internals. Every part card shows a picture of the part, and the part glows in the 3D view when you fit it. Then run the dyno, read the gauges and drive it (0–100 km/h, ¼ mile). |
| **See inside the cylinder** | Under the 3D view: the cylinder's p–V diagram (normal and log scale) and pressure against crank angle, worked out one degree at a time and live as you rev. A dot follows piston 1 in the 3D view. Knock shows as ringing on the trace (and a ping in the sound), a misfire as a missing burn. Below it: where the fuel's energy goes and where the friction is. The other engines show their own diagram (indicator diagram for steam, Stirling loop, fuel-cell curve…). Press **p–V** under the 3D view for a small live trace on top of the engine. |
| **See inside in 3D** | In **Strokes** view the gas in every cylinder is coloured by the cycle model: blue fresh air, a flame front spreading from the plug, burned gas cooling as it expands. Sparks and diesel sprays flash at the right moment and each cylinder lights up as it fires. **Step** freezes the engine so you can move one degree at a time, with an explanation of each stroke you can listen to. **Forces** draws the gas, rod, side-thrust and crank forces on the cylinder you tap. Drag the cut in **Cutaway**. The p–V panel also shows the valve-timing dial and the engine sound as a live spectrum. |
| **Heat and stress** | **Heat** turns the 3D view into a thermal camera with coolant and oil flowing through the engine; **Stress** shows how close each part is to breaking. A thermal model (thermostat, radiator, fan, oil cooler) runs live, and **Start from cold** in the Condition tab shows a real cold start: fast idle, rough running and white vapour until it warms. |
| **Dyno day** | Pick the weather and altitude (a 45 °C Muscat summer, a cool morning, Jebel Shams at 3000 m, or your own) and see the measured power next to the SAE J1349 and DIN 70020 corrected figures. The ECU tab shows each fuel's properties. |
| **Find faults** | Switch on real faults (vacuum leak, worn rings, blown head gasket, stretched timing chain…) and diagnose them from the gauges, the sound, the exhaust smoke and the OBD-II codes. Or play **Mystery fault**: the garage hides one fault and you find it. |
| **Teacher mode** | The teacher sets the class experiment, sees the answers and checks students' tables. |
| **All calculations** | Every formula the site uses, with symbols, units and live worked examples. |

## How to use the garage

1. Pick an engine with the buttons above the 3D view.
2. Press **Start**, then hold **GAS** (or the space bar) to rev it.
3. Add parts in the panel on the right. **Simple** shows the main parts and **All parts** shows every option. You can search any part by name.
4. Press **Run dyno pull** to see the power and torque curves, or press **Drive**.
5. Scroll down to **Inside the cylinder** to watch the pressure in the cylinder, or press **p–V** under the 3D view.
6. Turn on **Gauges** under the 3D view to watch boost, lambda, exhaust temperature, oil pressure, coolant and more.

If you get lost in the 3D view, press **⟲ Reset view**, or use the **3/4 · Front · Side · Top** buttons.

## Good to know

- **Simplified models:** the numbers come from real engineering relations with simplified assumptions. They are good for learning and comparing, but they are not manufacturer data.
- **No sound recordings:** the engine sounds are made live from each engine's firing order and exhaust. The one exception is the turbo flutter, which uses the author's own recording.
- **Saved builds:** **Save build** keeps one garage build on your device, and **Copy share link** puts a build into a link.
- **Fresh start:** every engine opens in stock form. Settings never carry over hidden from one engine to another.

## Running it locally

EngineLab is one self-contained `index.html` file, so just open it in a modern browser. To install it as an app with offline use, serve the folder over `http` (for example `python3 -m http.server`) and use the browser's **Install** option. The service worker is `sw.js` and the manifest is `manifest.webmanifest`.

Built with [three.js](https://threejs.org/) for the 3D view and the Web Audio API (AudioWorklet) for the sound.

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
| **Find faults** | Switch on real faults (vacuum leak, worn rings, blown head gasket, stretched timing chain…) and diagnose them from the gauges, the sound, the exhaust smoke and the OBD-II codes. Or play **Mystery fault**: the garage hides one fault and you find it. |
| **Teacher mode** | The teacher sets the class experiment, sees the answers and checks students' tables. |
| **All calculations** | Every formula the site uses, with symbols, units and live worked examples. |

## How to use the garage

1. Pick an engine with the buttons above the 3D view.
2. Press **Start**, then hold **GAS** (or the space bar) to rev it.
3. Add parts in the panel on the right. **Simple** shows the main parts and **All parts** shows every option. You can search any part by name.
4. Press **Run dyno pull** to see the power and torque curves, or press **Drive**.
5. Turn on **Gauges** under the 3D view to watch boost, lambda, exhaust temperature, oil pressure, coolant and more.

If you get lost in the 3D view, press **⟲ Reset view**, or use the **3/4 · Front · Side · Top** buttons.

## Good to know

- **Simplified models:** the numbers come from real engineering relations with simplified assumptions. They are good for learning and comparing, but they are not manufacturer data.
- **No sound recordings:** the engine sounds are made live from each engine's firing order and exhaust. The one exception is the turbo flutter, which uses the author's own recording.
- **Saved builds:** **Save build** keeps one garage build on your device, and **Copy share link** puts a build into a link.
- **Fresh start:** every engine opens in stock form. Settings never carry over hidden from one engine to another.

## Running it locally

EngineLab is one self-contained `index.html` file, so just open it in a modern browser. To install it as an app with offline use, serve the folder over `http` (for example `python3 -m http.server`) and use the browser's **Install** option. The service worker is `sw.js` and the manifest is `manifest.webmanifest`.

Built with [three.js](https://threejs.org/) for the 3D view and the Web Audio API (AudioWorklet) for the sound.

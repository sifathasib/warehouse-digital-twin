# 🚚 3D Warehouse Digital Twin & Yard Fleet Tracking Simulation

A real-time, interactive 3D logistics yard and warehouse simulation built with **Three.js**, procedural vehicle geometry, autonomous pathfinding, and a live IoT-style digital twin telemetry dashboard.

---

## 🌟 Live Demo

👉 **[View Live Simulation](https://sifathasib.github.io/warehouse-digital-twin/)**

---

## 📦 Features

### 1. 3D Yard & Infrastructure
* **10 Numbered Parking Bays (`Bay 01` to `Bay 10`)**: Arranged in two opposing rows with safety boundary stripes and road decals.
* **Warehouse Facility**:
  * 3 Dedicated **Loading Docks (`D01`, `D02`, `D03`)**.
  * **Interior Storage Aisles**: Heavy-duty industrial racking (Safety Orange uprights) holding realistic pallet crates.
  * **Translucent Skylight Roof**: Toggleable between "Cutaway view" (to monitor interior rack inventory from above) and "Solid exterior".
* **Animated Security Gates**: Rotating gate barrier arms that automatically open for approaching vehicles.
* **Road & Lane Markings**: Yellow/white centerlines guiding trucks into parking aisles and docks.

### 2. Autonomous Fleet Simulation
* **Procedural 3D Semi-Trucks**: Detailed cabs, aerodynamic windshields, grilles, exhaust pipes, headlights, rotating wheels, and cargo trailers in various fleet colors.
* **State Machine & Path Navigation**:
  * `ARRIVING`: Trucks enter through the main security gate.
  * `NAVIGATING`: Autonomous steering and waypoint following through designated road corridors with glowing GPS trajectory lines.
  * `PARKED`: Reverse-parking into assigned bays (`Bay 01` – `Bay 10`).
  * `AT_DOCK` / `UNLOADING`: Reversing into loading docks. An autonomous forklift / AGV automatically unloads pallets from the trailer into the warehouse racks.
  * `DEPARTING`: Exiting through the designated exit gate.
* **Drone Follow Camera Mode**: Click "Follow Truck" to chase active trucks from an aerial drone perspective.

### 3. Interactive Cyber-Dashboard (HUD)
* **Real-time Telemetry**: Active fleet count, parking bay occupancy %, warehouse rack capacity, and live facility time.
* **Dispatch Controls**: Spawn delivery trucks, manually dispatch any vehicle to any bay/dock, or toggle the 24/7 autonomous traffic loop.
* **Speed Multipliers**: Switch between `1x`, `2x`, and `4x` simulation speeds.
* **Day / Night Lighting**: Switch between sunny daylight and cinematic night floodlight mode.

---

## 🛠️ Built With

* [Three.js](https://threejs.org/) - 3D WebGL rendering engine
* [OrbitControls](https://threejs.org/docs/#examples/en/controls/OrbitControls) - 3D camera navigation
* [Tailwind CSS](https://tailwindcss.com/) - Modern HUD styling
* [Lucide Icons](https://lucide.dev/) - Dashboard icons

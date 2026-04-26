# 📱 Campus Navigation App (VIT Pune)

A **mobile-first campus navigation system** built with **React Native (Expo)** that uses **graph algorithms (Dijkstra)** to compute optimal paths and visualize them in real time with smooth animations.

---

## 🚀 Features

### 🧭 Graph-Based Navigation
- Uses **Dijkstra’s algorithm** (fully local, no backend required)
- Instant route calculation

### 🗺️ Interactive Map
- Built with `react-native-maps`
- Smooth polyline route rendering

### 🔺 Animated Direction Arrow
- Moves smoothly along the computed path
- Rotates dynamically based on direction

### 🎥 Camera Control
- Optional **follow mode** (like Google Maps)
- Adjustable zoom & UI offset

### 📍 Markers
- Start point → 🟢  
- End point → 🔴  
- Nearby nodes shown dynamically

### 🔽 Custom Dropdown UI
- Fully custom (no native picker issues)
- Dark theme consistent with app

### 📊 Algorithm Visualization
- Step-by-step **Dijkstra execution**
- Toggle between:
  - Controls view
  - Algorithm steps view

---

## 🧠 Tech Stack

- **Frontend:** React Native (Expo)  
- **Maps:** react-native-maps  
- **Logic:** Pure JavaScript (local graph engine)  
- **UI:** Custom-built components  

---

## 📁 Project Structure

```
campus-nav/
│
├── App.js
│
├── data/
│   └── graph.js        # Nodes + edges (campus map)
│
├── services/
│   ├── router.js       # Route handler
│   └── dijkstra.js     # Algorithm logic
│
├── assets/
│
├── package.json
└── app.json
```

---

## ⚙️ Installation & Setup

### 1. Install dependencies
```bash
npm install
```

### 2. Install maps
```bash
npx expo install react-native-maps
```

### 3. Run the app
```bash
npx expo start -c
```

---

## 📱 Running the App

- Press **`a`** → Android emulator  
- Press **`i`** → iOS simulator (Mac only)  
- Or scan QR using **Expo Go**

---

## 🎮 How to Use

1. Select **Start Node**
2. Select **End Node**
3. Tap **Find Route**

### 🎬 What happens next:
- Route is drawn on the map  
- Arrow animates along the path  
- Dijkstra steps shown in visualization panel  

---

## ⚡ Key Concepts

### 🧩 Graph Representation
- **Nodes** = Locations (`lat`, `lng`)
- **Edges** = Connections between nodes

### 🧭 Pathfinding
- Dijkstra computes shortest path
- Path converted into coordinates for map rendering

### 🎞️ Animation
- Path split into smooth segments
- Arrow moves frame-by-frame
- Rotation based on angle between points

---

## 🎯 Customizations

### 🔍 Adjust Zoom
```js
latitudeDelta / longitudeDelta
```

### 📍 Shift Map Position
```js
latitude +/- small offset
```

### 🎥 Camera Follow Toggle
```js
followCamera = true / false
```

### 🐢 Change Arrow Speed
```js
frame % N   // Increase N = slower animation
```

---

## 🚀 Future Enhancements

- 🧭 Turn-by-turn navigation (voice)
- 📍 Real GPS integration
- 🗺️ Offline map tiles
- 👆 Tap-to-select nodes
- 📊 Advanced algorithms (A*, K-shortest paths)
- 📱 Draggable bottom sheet UI

---

## 💡 Notes

- Fully **offline-capable**
- **No backend required**
- Optimized for **campus-scale navigation**

---

## 👨‍💻 Author

Built as part of an **Advanced DSA + Mobile Systems Project**  
at **VIT Pune**

---

## ⭐ If you like this project

Give it a ⭐ and take it to the next level 🚀

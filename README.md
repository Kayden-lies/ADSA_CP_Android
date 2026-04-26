📱 Campus Navigation App (VIT Pune)
A mobile-first campus navigation system built with React Native (Expo) that uses graph algorithms (Dijkstra) to compute optimal paths and visualize them in real time with smooth animations.

🚀 Features


🧭 Graph-Based Navigation

Uses Dijkstra’s algorithm (local, no backend required)
Instant route calculation



🗺️ Interactive Map

Built with react-native-maps
Smooth polyline rendering



🔺 Animated Direction Arrow

Moves along route smoothly
Rotates based on direction



🎥 Camera Control

Optional follow mode (like Google Maps)
Adjustable zoom & offset for UI



📍 Markers

Start (🟢) and End (🔴) points
Nearby nodes dynamically displayed



🔽 Custom Dropdown UI

Fully styled (no native picker issues)
Dark theme consistent with app



📊 Algorithm Visualization

Step-by-step Dijkstra execution shown
Toggle between controls and steps




🧠 Tech Stack

Frontend: React Native (Expo)
Maps: react-native-maps
Logic: Pure JavaScript (local graph engine)
UI: Custom components (no native picker)


📁 Project Structure
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


⚙️ Installation & Setup
1. Install dependencies
npm install

2. Install maps
npx expo install react-native-maps

3. Run the app
npx expo start -c


📱 Running the App

Press a → Android emulator
Press i → iOS simulator (Mac only)
Or scan QR using Expo Go


🎮 How to Use

Select Start Node
Select End Node
Tap Find Route
Watch:

Route drawn on map
Arrow animating with direction
Steps displayed in terminal view




⚡ Key Concepts
Graph Representation

Nodes = locations (lat, lng)
Edges = connections between nodes

Pathfinding

Dijkstra algorithm computes shortest path
Path converted into coordinates for map

Animation

Path interpolated into smooth segments
Arrow moves frame-by-frame
Rotation based on angle between points


🎯 Customizations
🔍 Adjust Zoom
latitudeDelta / longitudeDelta

📍 Shift Map Position
latitude +/- small offset

🎥 Camera Follow Toggle
followCamera state

🐢 Change Arrow Speed
frame % N (increase N = slower)


🚀 Future Enhancements

🧭 Turn-by-turn navigation (voice)
📍 Real GPS integration
🗺️ Offline maps
👆 Tap-to-select nodes
📊 Advanced algorithm visualization (A*, K-shortest)
📱 Draggable bottom sheet UI


💡 Notes

Fully offline-capable
No backend required
Designed for campus-scale navigation


👨‍💻 Author
Built as part of an advanced DSA + Mobile Systems project
at VIT Pune

⭐ If you like this project
Give it a ⭐ and take it to the next level 🚀

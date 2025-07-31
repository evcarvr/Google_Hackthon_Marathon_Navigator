# Google_Hackthon_Marathon_Navigator
Interactive route planner and GPS-based marathon navigator with waypoint tracking and real-time feedback.

# 🏃‍♀️ Marathon Navigation App

A step-by-step navigation tool that helps **Authors** create a walking route and **Participants** follow it with real-time guidance, deviation alerts, and completion confirmation.

---

## 📌 Project Overview

The **Marathon Navigation App** allows a user (Author) to define a custom path using waypoints on a map, and another user (Participant) to navigate along the same route using live visual guidance and feedback. It ensures the user follows the intended path and notifies them if they stray too far or reach the destination.

---

## 👤 Author Role (Route Creator)

The **Author** is responsible for planning the path that the **Participant** will walk.

### What the Author Can Do

1. **➕ Add Waypoints**  
   - Tap (on mobile) or click (on desktop) anywhere on the map to place a waypoint.  
   - Each point is automatically connected to form a route.

2. **📝 Add Notes (Optional)**  
   - Click a waypoint to add a note (e.g., “Café here” or “Steep stairs”).

3. **🗑️ Delete a Waypoint**  
   - Double-tap (on mobile) or double-click (on desktop) directly on a waypoint marker to delete it.  
   - The path recalculates immediately after deletion.

4. **📍 Adjust Waypoint Position (Drag & Drop)**  
   - Click and drag any waypoint marker to a new location.  
   - The route updates automatically in real time.

5. **🚮 Clear Entire Route**  
   - Click the “Clear Route” button to remove all waypoints and the route.

6. **💾 Save Route**  
   - Once at least two waypoints are placed, click “Save Path” to store your route.

7. **📂 Load Route**  
   - Use “Load Path” to reopen or edit a previously saved route.

8. **🔗 Generate Shareable Link**  
   - After saving the route, a shareable link is generated.  
   - This link can be sent to Participants to follow the navigation path.

---

## 🧍 Participant Role (Route Follower)

The **Participant** uses the shared path to physically navigate through the route.

### How the Participant Navigates

1. **▶️ Start Navigation**  
   - Click on “Start Navigation” to begin the guided experience.

2. **📍 Begin at the First Waypoint Only**  
   - Navigation starts only when you are near the first waypoint.  
   - If you're too far, navigation cannot begin.

3. **➡️ Follow Waypoints in Sequence**  
   - You must follow the waypoints in the order they were created.  
   - Skipping ahead or taking shortcuts is not allowed.

4. **🧭 Live Guidance**  
   - A highlighted path guides you from one waypoint to the next.  
   - Popups or instructions appear as you approach each waypoint.

5. **⚠️ Route Deviation Warning**  
   - If you stray too far from the path, a popup alert will notify you.  
   - The alert disappears once you return to the correct route.

6. **✅ Completion**  
   - Navigation ends automatically when all waypoints are visited and the destination is reached.  
   - A confirmation message appears: **“You have arrived at your destination.”**

---

## 🛠️ Tech Stack

- JavaScript / HTML / CSS
- Google Maps JavaScript API
- Geolocation API

---

## 📂 Folder Structure

├── index.html        # Main interface
├── style.css         # UI styling
├── script.js         # Core logic (waypoints, navigation, alerts)
├── savedRoutes.js    # Saved path handling
└── assets/           # Icons or assets (optional)

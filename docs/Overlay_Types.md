# 🧿 Overlay Types – VisionFrame Tactical

This document outlines the augmented reality overlay system used by VisionFrame Tactical, including HUD zones, iconography, tag coloring, and mission-specific visual modes.

---

## 🔍 Overlay Zones (HUD Layout)
## 🔍 Overlay Zones (HUD Layout)

```
+----------------------------+
|        UPPER ZONE         |  ← Squad Status, Alerts
|----------------------------|
|       CENTRAL ZONE        |  ← Real-World + Tactical Highlights (Unobstructed)
|----------------------------|
|        LOWER ZONE         |  ← Navigation, Commands, Threat Distance
+----------------------------+
```
- **Upper Zone**: Displays health/vitals of squad, command alerts, objective reminders
- **Central Zone**: Displays real-time overlays directly on world objects (enemy tags, terrain intel)
- **Lower Zone**: Renders compass, meters-to-target, minimap, command menus

---

## 🟥 Color Coding (Threats & Conditions)

| Color         | Meaning                               |
|---------------|----------------------------------------|
| 🔴 Red        | Confirmed high-level threat            |
| 🟠 Orange     | Active target, moderate threat         |
| 🟡 Yellow     | Possible contact / sensor ping         |
| 🟢 Green      | Friendly / Verified squad member       |
| 🔵 Blue       | Navigation waypoint or safe zone       |
| ⚪ White       | Unknown / Unclassified / Civilian      |
| 🟣 Purple     | VIP / High-importance entity (Tagged)  |

---

## 🧠 Overlay Types

### 1. **Threat Tagging**
- Color-coded bounding box over target
- Distance in meters shown beneath box
- Flashing if threat is actively engaging

### 2. **Navigation Mode**
- Floating waypoints visible through terrain
- Solid arrow indicators (semi-transparent)
- Current GPS coordinates in corner

### 3. **Squad Status**
- Vital bars show color-shifted pulse (e.g., green to red)
- Outline flashes if under fire or critical health
- Triage icon appears if medevac needed

### 4. **Environmental Awareness**
- Wind speed, direction arrows, barometric pressure
- Optional tree/building transparency (toggleable)
- Map terrain heatmap overlay for ambush risk

### 5. **Command Feed**
- Real-time text feed (orders, recon info, AI flags)
- Displays per role (Commander, Recon, Medic, etc.)
- Optional voice-to-text overlay for silent ops

---

## ⚙️ Customization Modes

Each role (e.g., medic, recon, air support) can load a pre-configured overlay profile, adjusting:

- Color contrast and brightness
- Overlay positioning (left-dominant, right-dominant)
- Icon scale and density
- Voice cues vs. text overlays

---

## 🛡 Overlay Clarity & Safety

- Central FOV is **always kept clear** of overlays for safety
- Peripheral zones are used for icons, minimaps, and nav
- Brightness adapts to light conditions and NV compatibility

> VisionFrame overlays are mission-adaptive, role-specific, and FOV-conscious — enabling precision without distraction.

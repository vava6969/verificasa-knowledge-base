# 3D / 360° virtual tours

VerifiCasa creates the 3D tours for its listings in-house. Andrei built the scanning system himself.

## How it works today

- Built for **iOS** with **Swift + ARKit + RoomPlan** (LiDAR scanning).
- Photo stitching uses **OpenCV** and **ARKit**.
- Each tour is about **50 MB**.
- Panorama stitching is planned to run **server-side on VerifiCasa's own VPS** (CPU-only, ~2 TB storage). Buying a GPU is ruled out as too expensive.
- A Base44 app, **"VerifiCasa Tur 360°"**, is used for browsing and starting 360° tours.

## Known issues

- Current tours can look **ghosty and blurry**. They don't yet have the smooth "look-around" quality of photo-stitched competitors like Travvir.

## Direction

- One app that does **both scanning (creating tours) and viewing (browsing others' tours)**, plus a **web version**.
- Grow into a **Matterport / Teleport-style all-in-one tool** for agencies. All of these would sit in one section on the property page:
  - 3D tour
  - 2D tour
  - Dollhouse view
  - Floor plans and 3D floor plans
  - Measurements
  - Document scanner
  - Document signature
- Andrei is getting the **full Swift source code from the developer** to improve it further.

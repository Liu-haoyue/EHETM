# [CVPR 2026] High-Quality and Efficient Turbulence Mitigation with Events
## ⭐ News
This repository will contain the official implementation and dataset for our project.

The code and dataset will be released soon.

---

## 📌 Overview

## 📦 Dataset

We present **CTTH and LATH**, **two event–frame paired datasets** for turbulence imaging research, covering both **thermal** and **atmospheric** cases. We offer both **Baidu Cloud Drive** ([Download Link](https://pan.baidu.com/s/xxxx), code: xxxx). Dataset structure is organized as:

```
Dataset/
├── CTTH/
│   ├── Dynamic_Object/
│   │   ├── Train/
│   │   │   ├── seq_000/
│   │   │   │   ├── GT/
│   │   │   │   │   ├── frames/
│   │   │   │   │   ├── events/
│   │   │   │   │   ├── frame_timestamp.txt
│   │   │   │   │   └── event_timestamp.txt
│   │   │   │   ├── Turb/
│   │   │   │   │   ├── frames/
│   │   │   │   │   ├── events/
│   │   │   │   │   ├── frame_timestamp.txt
│   │   │   │   │   └── event_timestamp.txt
│   │   │   │   └── Flow/
│   │   │   └── ...
│   │   └── Test/
│   │       ├── seq_000/
│   │       └── ...
│   │
│   ├── Static/
│   │   ├── Train/
│   │   │   ├── seq_000/
│   │   │   │   ├── turb/
│   │   │   │   ├── event/
│   │   │   │   ├── frame_timestamp.txt
│   │   │   │   ├── event_timestamp.txt
│   │   │   │   └── gt.jpg
│   │   │   └── ...
│   │   └── Test/
│   │       ├── seq_000/
│   │       └── ...
│
├── LATH/
│   ├── seq_000/
│   │   ├── turb/
│   │   ├── events/
│   │   ├── frame_timestamp.txt
│   │   └── event_timestamp.txt
│   └── ...
```

### 🔥 CTTH: Close-range Thermal Turbulence Hybrid Dataset

<table align="center">
  <tr>
    <th>GT</th>
    <th>Turbulent Video</th>
    <th>Events</th>
    <th>GT</th>
    <th>Turbulent Video</th>
    <th>Events</th>
  </tr>
  <tr>
    <td><img src="assets/dynamic1_GT.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/dynamic1_Turb.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/dynamic1_event.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/dynamic2_gt.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/dynamic2_turb.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/dynamic2_event.gif" width="120" height="120" style="object-fit: cover;"></td>
  </tr>
  <tr>
    <td><img src="assets/static1_GT.png" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/static1_turb.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/static1_events.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/static2_GT.png" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/static2_turb.gif" width="120" height="120" style="object-fit: cover;"></td>
    <td><img src="assets/static2_events.gif" width="120" height="120" style="object-fit: cover;"></td>
  </tr>
</table>

<p align="center">
  <em>Each group shows ground truth, turbulent observation, and corresponding events.</em>
</p>

The CTTH dataset is designed to capture:

- 🚗 Dynamic object
- 🏙️ Static background structures
- 🎯 Corresponding ground-truth references

This enables rigorous evaluation of turbulence mitigation under **real static and dynamic-object scenes**.

---

### 🌫️ LATH: Long-range Atmospheric Turbulence Hybrid Dataset

<table align="center">
  <!-- 列标题 -->
  <tr>
    <th>Turbulent Video</th>
    <th>Events</th>
    <th>Turbulent Video</th>
    <th>Events</th>
  </tr>

  <!-- 第一行内容 -->
  <tr>
    <td><img src="assets/3.5km_turb.gif" width="180" height="180" style="object-fit: cover;"></td>
    <td><img src="assets/3.5km_event.gif" width="180" height="180" style="object-fit: cover;"></td>
    <td><img src="assets/5km_turb.gif" width="180" height="180" style="object-fit: cover;"></td>
    <td><img src="assets/5km_Event_video.gif" width="180" height="180" style="object-fit: cover;"></td>
  </tr>

  <!-- 第一行的分组说明 -->
  <tr>
    <td colspan="2" align="center"><em>3.5Km, Building</em></td>
    <td colspan="2" align="center"><em>5Km, Signs and Moving Cars</em></td>
  </tr>

  <!-- 第二行内容 -->
  <tr>
    <td><img src="assets/6.5km_turb.gif" width="180" height="180" style="object-fit: cover;"></td>
    <td><img src="assets/6.5km_Event_video.gif" width="180" height="180" style="object-fit: cover;"></td>
    <td><img src="assets/8km_turb.gif" width="180" height="180" style="object-fit: cover;"></td>
    <td><img src="assets/8km_Event_video.gif" width="180" height="180" style="object-fit: cover;"></td>
  </tr>

  <!-- 第二行的分组说明 -->
  <tr>
    <td colspan="2" align="center"><em>6.5Km, Heavy Traffic</em></td>
    <td colspan="2" align="center"><em>8Km, Bridge</em></td>
  </tr>
</table>

<p align="center">
  <em>Examples of atmospheric turbulence under different shooting distances.</em>
</p>

The LATH dataset captures turbulence effects across **various imaging distances and scenes**, including:

- 🌉 Long-range imaging
- 🏞️ Diverse environmental structures

This provides a valuable benchmark for evaluating **generalization under real-world atmospheric turbulence**.

---

This dataset is designed to support:
- **Turbulence mitigation**
- **Event-based video/image restoration**
---

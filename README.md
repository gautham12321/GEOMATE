# 🛰️ GEOMATE: LiDAR, GPS & 360° Camera Integration

This project is a mobile mapping system designed to integrate three key devices for precise survey data collection:  
1. **ZF Profiler LiDAR**  
2. **NovAtel GPS Receiver**  
3. **Ladybug 360° Camera**

The system coordinates these devices to create accurate, synchronized survey data, ideal for mapping large areas and collecting high-quality 3D spatial data.

## 🔧 Project Components

### 1. **ZF Profiler LiDAR**
The ZF Profiler LiDAR captures detailed point cloud data for 3D mapping and terrain modeling.  
- The LiDAR data is stored in `.zfs` files.
- Data is accessed and managed via FTP.

### 2. **NovAtel GPS Receiver**
The NovAtel GPS provides accurate positioning data that is used to georeference the LiDAR scans.
- Commands are sent via the ICOM2 port (IP: `192.168.1.105`, Port: `3002`).
- GPS data is recorded in `.gps` files.

### 3. **Ladybug 360° Camera**
The Ladybug camera captures high-resolution, 360-degree imagery to complement the LiDAR data.  
- Controlled using the **Ladybug SDK** (C++).
- Used for detailed visualization and scene context.

---

## ⚙️ Architecture & Workflow

1. **Backend**: 
   - Developed in **Python** using **Flask**.
   - Handles communication between devices and the user interface.

2. **Frontend**: 
   - Developed with **React**.
   - User interface to control the devices and display data.

3. **Device Synchronization**: 
   - The LiDAR, GPS, and Camera are synchronized to collect data simultaneously.
   - Data is processed and stored locally for further analysis.

4. **Data Storage**:
   - LiDAR data is stored in `.zfs` format.
   - GPS data in `.gps` format.
   - All data is managed and accessed through FTP.

---
### 🎥 Demo Video

Click [here](demo/demo-video.mp4) to watch the demo video.


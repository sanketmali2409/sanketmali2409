<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Sanket%20Mali&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Embedded%20Systems%20%C2%B7%20Robotics%20%C2%B7%20Autonomous%20Navigation&descAlignY=55&descSize=17" width="100%" />

<a href="https://github.com/sanketmali2409">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=21&pause=1200&color=36BCF7&center=true&vCenter=true&width=620&lines=Firmware+that+ships+on+real+hardware;ROS+2+robots+that+navigate+without+a+human;Sensors%2C+timing%2C+and+the+bugs+in+between" alt="Typing SVG" />
</a>

<br/>

<a href="https://www.linkedin.com/in/sanket-mali-310469250"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://sanketmali2409.onrender.com/"><img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
<a href="mailto:raushan@xprobotics.ai"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>

</div>

---

## 👋 About

I build the layer where **software meets moving hardware** — firmware on microcontrollers, Linux on SBCs, and ROS 2 stacks that turn sensor noise into navigation.

- 🤖 Autonomous mobile robots: **SLAM, Nav2, sensor fusion, mecanum & differential drive**
- ⚙️ Bare-metal and RTOS firmware on **ESP32, STM32, ARM Cortex-M**
- 🐧 Embedded Linux on **Raspberry Pi 4/5, Jetson Nano, RK3588** — drivers, V4L2, Yocto images
- 📷 Perception plumbing: **multi-camera capture, stereo depth, LiDAR, IMU, encoders**
- 🕰️ The part nobody puts on a badge: **timestamp alignment, USB bandwidth budgets, and why the camera returns EBUSY**

**Currently:** building production-grade autonomous cleaning robots and multi-sensor logging pipelines.

---

## 🛠️ What I Work With

| Domain | Tools & Technologies |
|---|---|
| **Languages** | C · C++ (11/17) · Python · Bash |
| **MCUs** | ESP32 · ESP8266 · STM32 · ARM Cortex-M · LPC2148 · PIC · 8051 |
| **SBC / Linux** | Raspberry Pi 4 & 5 · Jetson Nano · RK3588 · Embedded Linux · Yocto / BitBake · U-Boot |
| **Robotics** | ROS 2 (Humble, Jazzy) · Nav2 · SLAM Toolbox · TF2 · robot_localization · Gazebo · RViz |
| **Perception** | OpenCV · YOLO · stereo depth · camera calibration · RPLiDAR A1M8 · YDLiDAR X2 · MPU6050 |
| **Interfaces** | UART · I²C · SPI · CAN · USB 2.0 · BLE · Wi-Fi · ESP-NOW · LoRa · GSM · GPS |
| **Data & Tooling** | MCAP · rosbag2 · Foxglove · Docker · Git · PlatformIO · KiCad · Keil · MPLAB |

<div align="center">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" height="38" alt="C" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" height="38" alt="C++" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="38" alt="Python" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="38" alt="Linux" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/raspberrypi/raspberrypi-original.svg" height="38" alt="Raspberry Pi" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/opencv/opencv-original.svg" height="38" alt="OpenCV" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" height="38" alt="Docker" />&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" height="38" alt="Git" />
</div>

---

## 🚀 Featured Work

### 🧹 Autonomous Floor & Stair Cleaning Robot
> Omnidirectional cleaning robot that maps an unknown floor and covers it without a driver.

**Stack:** Raspberry Pi 5 + ESP32 · ROS 2 · Nav2 · SLAM Toolbox · RPLiDAR · MPU6050 · wheel encoders · mecanum drive

- Split the system: **ESP32 owns real-time motor control and encoder ticks**, the Pi owns mapping and planning — so a busy planner can never stall a motor loop.
- Fused wheel odometry with IMU through `robot_localization` to stop the heading drift that kept breaking loop closure.
- Tuned Nav2 costmaps and controllers for **holonomic motion**, where the usual differential-drive defaults simply don't apply.

### 📡 Distributed Sensor Synchronization
> Many ESP32 nodes, one coherent timeline.

**Stack:** ESP-NOW · UART/USB bridge · Python · MCAP · Foxglove

- Built a **timestamp synchronization scheme over ESP-NOW** so samples from independent nodes land on a shared clock instead of arrival order.
- Streams into **MCAP** for replay and inspection in Foxglove — logs you can actually debug after the run, not just during it.
- Designed for continuous real-time logging without dropping frames under load.

### 👁️ Multi-Camera Robotic Perception
> Stereo + wrist cameras on a single USB 2.0 tree, running together.

**Stack:** stereo camera · wrist cameras · USB 2.0 hub · MJPEG · OpenCV

- Worked inside the **USB 2.0 bandwidth ceiling** using MJPEG and per-camera resolution budgeting so all streams stay alive at once.
- Calibrated and synchronized cameras for **depth and spatial perception** across viewpoints.
- Solved the real-world failure modes: enumeration order, device busy conflicts, and per-frame timestamping.

---

## 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats-fast.vercel.app/api?username=sanketmali2409&show_icons=true&include_all_commits=true&count_private=true&theme=tokyonight&hide_border=true" height="160" alt="GitHub Stats" />
<img src="https://github-readme-stats-fast.vercel.app/api/top-langs?username=sanketmali2409&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&card_width=330" height="160" alt="Top Languages" />

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=sanketmali2409&theme=tokyo-night&hide_border=true&area=true" alt="Contribution Graph" width="98%" />

</div>

---

## 🌱 Currently Exploring

`Sensor fusion beyond EKF` · `Visual-inertial odometry` · `Real-time scheduling on embedded Linux` · `Yocto image hardening for field robots`

---

<div align="center">

**Open to collaborating on robotics, embedded systems, and anything that has to work when nobody is watching it.**

<a href="mailto:raushan@xprobotics.ai"><img src="https://img.shields.io/badge/Let's%20build%20something-36BCF7?style=for-the-badge&logoColor=white" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=110&section=footer" width="100%" />

</div>

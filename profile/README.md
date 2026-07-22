<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg" />
    <img src="assets/banner-dark.svg" alt="ChiefTechLabs — Full-stack Robotics R&D" width="100%" />
  </picture>
</div>

<br />

<div align="center">
  <strong>Full-stack robotics R&amp;D — from bare-metal drivers to autonomous systems.</strong><br />
  <sub>机器人全栈研发 —— 从底层硬件接口到上层自主系统。</sub>
</div>

<br />

---

## Tech Stack / 技术栈

<sub>Extracted from production code across our repositories. 以下技术栈提取自各仓库的实际生产代码。</sub>

| Domain | Technologies |
| --- | --- |
| **Languages** | ![C++23](https://img.shields.io/badge/C%2B%2B_23-16222e?style=flat-square&logo=cplusplus&logoColor=22d3ee) ![C](https://img.shields.io/badge/C-16222e?style=flat-square&logo=c&logoColor=22d3ee) ![Python](https://img.shields.io/badge/Python_3.10%2B-16222e?style=flat-square&logo=python&logoColor=22d3ee) ![TypeScript](https://img.shields.io/badge/TypeScript-16222e?style=flat-square&logo=typescript&logoColor=22d3ee) ![Shell](https://img.shields.io/badge/Shell-16222e?style=flat-square&logo=gnubash&logoColor=22d3ee) |
| **Robot Middleware** | ![ROS 2 Humble](https://img.shields.io/badge/ROS_2_Humble-16222e?style=flat-square&logo=ros&logoColor=22d3ee) ![ros2_control](https://img.shields.io/badge/ros2__control-16222e?style=flat-square) ![MoveIt 2](https://img.shields.io/badge/MoveIt_2-16222e?style=flat-square) ![Nav2](https://img.shields.io/badge/Nav2-16222e?style=flat-square) ![Gazebo](https://img.shields.io/badge/Gazebo-16222e?style=flat-square) |
| **Perception & Navigation** | ![OpenCV](https://img.shields.io/badge/OpenCV-16222e?style=flat-square&logo=opencv&logoColor=22d3ee) ![Intel RealSense](https://img.shields.io/badge/Intel_RealSense-16222e?style=flat-square) ![LiDAR SLAM](https://img.shields.io/badge/LiDAR_SLAM-16222e?style=flat-square) ![LIO · ESKF](https://img.shields.io/badge/LIO_%C2%B7_ESKF-16222e?style=flat-square) |
| **Embedded & Hardware** | ![ESP32-C3](https://img.shields.io/badge/ESP32--C3-16222e?style=flat-square&logo=espressif&logoColor=22d3ee) ![STM32](https://img.shields.io/badge/STM32-16222e?style=flat-square&logo=stmicroelectronics&logoColor=22d3ee) ![CAN bus](https://img.shields.io/badge/CAN_bus-16222e?style=flat-square) ![Modbus RTU](https://img.shields.io/badge/Modbus_RTU-16222e?style=flat-square) |
| **Backend & AI** | ![FastAPI](https://img.shields.io/badge/FastAPI-16222e?style=flat-square&logo=fastapi&logoColor=22d3ee) ![SQLAlchemy 2.0](https://img.shields.io/badge/SQLAlchemy_2.0-16222e?style=flat-square) ![LangChain](https://img.shields.io/badge/LangChain-16222e?style=flat-square&logo=langchain&logoColor=22d3ee) ![LangGraph](https://img.shields.io/badge/LangGraph-16222e?style=flat-square&logo=langgraph&logoColor=22d3ee) ![Playwright](https://img.shields.io/badge/Playwright-16222e?style=flat-square) |
| **Frontend** | ![React 19](https://img.shields.io/badge/React_19-16222e?style=flat-square&logo=react&logoColor=22d3ee) ![Vite](https://img.shields.io/badge/Vite-16222e?style=flat-square&logo=vite&logoColor=22d3ee) ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-16222e?style=flat-square&logo=tailwindcss&logoColor=22d3ee) ![shadcn/ui](https://img.shields.io/badge/shadcn--ui-16222e?style=flat-square&logo=shadcnui&logoColor=22d3ee) ![Radix UI](https://img.shields.io/badge/Radix_UI-16222e?style=flat-square&logo=radixui&logoColor=22d3ee) |
| **Engineering & DevOps** | ![Docker](https://img.shields.io/badge/Docker-16222e?style=flat-square&logo=docker&logoColor=22d3ee) ![CMake](https://img.shields.io/badge/CMake-16222e?style=flat-square&logo=cmake&logoColor=22d3ee) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-16222e?style=flat-square&logo=githubactions&logoColor=22d3ee) ![Dev Containers](https://img.shields.io/badge/Dev_Containers-16222e?style=flat-square) ![Clang Toolchain](https://img.shields.io/badge/Clang_Toolchain-16222e?style=flat-square&logo=llvm&logoColor=22d3ee) ![Ruff · Black](https://img.shields.io/badge/Ruff_%C2%B7_Black-16222e?style=flat-square) |

<br />

---

## Projects / 项目

### Robotics Core · 机器人核心

<sub>Hardware-near software: drivers, firmware, and the ROS 2 workspace that ties them together. 贴近硬件的一层：驱动、固件，以及把它们组织起来的 ROS 2 工作空间。</sub>

| Repository | Description |
| --- | --- |
| [`omrobot`](https://github.com/ChiefTechLabs/omrobot) | ROS 2 Humble workspace for OMRobot — mobile platform with robotic arm, omnidirectional chassis, and LiDAR SLAM navigation |
| [`dais_motor`](https://github.com/ChiefTechLabs/dais_motor) | Pure C++ Modbus RTU driver for the D-AIS48025A-R servo drive — zero ROS dependency |
| [`realman_arm`](https://github.com/ChiefTechLabs/realman_arm) | Pure C++ wrapper for the RealMan RM_API2 SDK — arm motion, gripper, and state monitoring |
| [`m65_chassis`](https://github.com/ChiefTechLabs/m65_chassis) | Pure C++ serial driver for the M65 omnidirectional chassis — zero ROS dependency |
| [`photogate`](https://github.com/ChiefTechLabs/photogate) | ESP32-C3 photogate sensor — firmware, C++ driver, and ros2_control plugin for OMRobot |

### AI & Automation · AI 与自动化

<sub>GenAI-powered pipelines that plan, generate, and ship content autonomously. 由 GenAI 驱动的自动化流水线。</sub>

| Repository | Description |
| --- | --- |
| [`geo`](https://github.com/ChiefTechLabs/geo) | GEO automation platform — GenAI-powered content pipeline for generative engine optimization: plan, generate, optimize, review, publish |

### Developer Tools · 开发工具

<sub>Agent skills and CLI tooling that make our daily workflow faster. 提升日常研发效率的 Agent 技能与命令行工具。</sub>

| Repository | Description |
| --- | --- |
| [`lark-skills`](https://github.com/ChiefTechLabs/lark-skills) | AI agent skills for lark-cli — natural-language control of Lark/Feishu: IM, docs, sheets, calendar, wiki, approval, and more |
| [`weekly-report`](https://github.com/ChiefTechLabs/weekly-report) | OpenCode skill — auto-generate structured weekly reports from OpenCode session history across projects |
| [`printer`](https://github.com/ChiefTechLabs/printer) | OpenCode skill — print documents, photos, and web pages via CUPS/IPP with automatic printer discovery |

<br />

---

## Join Us / 加入我们

<div align="center">
  <p>
    We hire engineers who are fluent at every layer — from registers to route planning.<br />
    <sub>我们在寻找打通每一层的工程师 —— 既读得懂寄存器，也调得好路径规划。</sub>
  </p>
  <a href="mailto:lorenzo@ugenrobot.com">
    <img src="https://img.shields.io/badge/We_are_hiring-lorenzo%40ugenrobot.com-0e7490?style=flat-square" alt="We are hiring — lorenzo@ugenrobot.com" />
  </a>
</div>

<br />

---

<div align="center">
  <sub><strong>ChiefTechLabs</strong> · Full-stack robotics R&amp;D · <a href="https://github.com/ChiefTechLabs">github.com/ChiefTechLabs</a></sub>
</div>

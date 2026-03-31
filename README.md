# Enterprise-Camera-System-Monitor
A full-stack web application that simulates and monitors an enterprise-scale IP camera system across multiple airport locations. This project was built to demonstrate real-world infrastructure monitoring, troubleshooting workflows, and system design concepts used in large environments like airports.

Live Demo
https://enterprise-camera-system-monitor.vercel.app/

Project Purpose
This project was designed to replicate real-world scenarios I encounter within IT Field Support working in an airport environment.
It focuses on:
• Monitoring IP-based camera systems
• Identifying common network and device issues
• Visualizing system health across multiple locations
• Simulating real-world failures for troubleshooting practice

System Overview
The application simulates 300+ IP cameras across multiple sites:
• Terminal 4 (T4) → VLAN 100 → 10.51.100.x
• Terminal 5 (T5) → VLAN 200 → 10.51.200.x
• TBIT → VLAN 300 → 10.51.300.x

Each camera includes:
• Status (Online / Offline)
• IP Address
• VLAN assignment
• Firmware version
• Location / Site

Key Features
- Real-Time Simulation
• System updates every 10 seconds
• Cameras randomly change state to simulate real issues:
• Offline devices
• DHCP failures (APIPA 169.254.x.x)
• Incorrect VLAN assignments
• Outdated firmware

API-Driven Backend
• REST API endpoints
/api/cameras
• Returns live camera data in JSON format
• Built with Node.js and Express

Interactive Frontend
• Displays all cameras in a clean dashboard
• Highlights problematic devices for quick identification
• Built using React + Tailwind CSS

<img width="658" height="494" alt="image" src="https://github.com/user-attachments/assets/a05ba2f8-8860-459a-b9ef-8c3241c2b635" />




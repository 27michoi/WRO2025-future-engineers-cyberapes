# WRO 2025 Future Engineers – Self-Driving Car Project  
Team Name: Cyberapes  
Category: Future Engineers — Self-Driving Cars  
Competition Year: 2025  


## 1. Summary
This repository contains the full documentation of our engineering process, source code, 3D models, and testing results for our entry in the World Robot Olympiad (WRO) Future Engineers category.  

Our goal was to design, build, and program a fully autonomous four-wheeled vehicle capable of completing both the **Open Challenge** and the **Obstacle Challenge** within the WRO rules, while documenting our full engineering journey to inspire and guide future teams.

Over the course of development, we designed **three chassis versions:
1. Prototype 1 — our quick first build to validate steering and driving concepts.
2. Prototype 2 — a refined and more stable platform with better sensor mounting.
3. Final Model — our competition-ready chassis, optimized for weight, stability, and serviceability.



## 2. Team
| Stefano | Team Leader, Mechanical Engineer | Systems integration, project coordination, chassis design |
| Aadidef | Software Engineer | Computer vision, control algorithms |
| Minjun | Mechanical Engineer, Documenter | Chassis design, fabrication, Documentation |



## 3. Development Timeline & Key Commits
WRO rules require at least 3 commits spaced over time, each reflecting substantial progress.  
- Commit 1 (≥2 months before competition): Initial chassis frame, steering assembly, and 20% of final control code.  
- Commit 2 (≥1 month before competition): Integration of camera + LiDAR, improved steering linkage, sensor fusion.  
- Commit 3 (≥2 weeks before competition): Final optimizations, parking routine implementation, wiring cleanup.  




## 4. Chassis Iterations

# 4.1 Prototype 1 — The Learning Platform  
Date: [Insert Date]  
Goal: Quickly test our basic steering and drive system.  
Features: 
- Aluminium frame, 4-wheel configuration, rear-wheel drive with front-wheel steering.  
- Simple sensor mounts for rapid testing.  

Challenges:
- Steering linkage had excessive play, reducing accuracy.  
- Motor torque was too high for smooth starts.  
- Limited surface area for secure sensor placement.  



# 4.2 Prototype 2 — The Stability Upgrade  
Date: [Insert Date]  
Goal: Improve steering precision, sensor layout, and vibration control.  
Features: 
- Custom 3D-printed steering assembly for tighter tolerances.  
- Extended chassis plate for better weight distribution.  
- Vibration damping to improve camera performance.  

Challenges: 
- Added weight brought us close to the 1.5 kg limit.  
- Cable routing interfered with steering during tight turns.  
- Overheating in motor drivers after prolonged runs.  


# 4.3 Final Model — Competition-Ready  
Date: [Insert Date]  
Goal: Deliver a stable, rule-compliant, and easily serviceable chassis.  
Features:  
- Lightweight carbon-fiber-reinforced base




## 5. Mobility, Power & Sensor Systems

Mobility Management
- Drive: Rear-wheel drive powered by DC motors with gearbox.
- Steering: Front-wheel servo-based rack-and-pinion system.
- Materials: Combination of aluminium, carbon fiber, and 3D-printed PLA+.

Power & Sense Management
- Power: [Battery Type] [Voltage/Capacity]
- Sensors: HD camera for vision, ultrasonic sensors for obstacle detection, IMU for orientation.

Obstacle Management
- Uses color detection (OpenCV) to identify green/red pillars.
- Dynamic path planning to adjust steering and speed in real time.


## 6. Assembly Instructions
1. Chassis Frame — Attach steering system to front axle and secure drive motors at the rear.
2. Electronics Mounting — Fix SBC/microcontroller, motor driver, and sensor boards using vibration-isolated mounts.
3. Wiring — Follow the wiring diagram in `/docs/wiring_diagram.png`.
4. Power System — Mount the battery securely in the center for balanced weight distribution.
5. Sensor Alignment — Calibrate camera and ultrasonic sensors using provided calibration scripts.


## 7. Code Instructions

add stuff here bro








pip install -r requirements.txt
python run_simulation.py
scp -r code/ pi@raspberrypi.local:/home/pi/robot
ssh pi@raspberrypi.local 'cd robot && ./start.sh'



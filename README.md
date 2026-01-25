





## Task 2: API

For this task, I built a small web app that shows real-time weather for any city using the OpenWeather API. I made it so I can type a city name and click a button to see the temperature, weather conditions, humidity, and wind speed. I also added a feature to refresh the data automatically every five minutes so it stays updated. While working on this, I got hands-on experience with fetching data from an API using JavaScript and displaying it on a webpage. It was interesting to see how quickly I could make the app respond to user input and show live information.  

![Screenshot_24-1-2026_125020_](https://github.com/user-attachments/assets/28a5bd4c-5bd1-462b-b52f-19bdcb0e2682)

 Here's the link [GitHub repository](https://github.com/vaishnavi070306-commits/wesatherapp)

### Task 3: Working with GitHub

In this task, I identified and fixed a small bug in an existing GitHub repository. The issue was present in the `add()` function, where an extra operation caused incorrect output, and I corrected it to ensure the function worked as expected. Through this task, I learned how GitHub workflows operate, including forking a repository, making changes on a separate branch, and creating a pull request to propose updates to the main repository. I also gained hands-on experience with repository management, code review processes, and collaboration using GitHub. 

![Screenshot_25-1-2026_122538_github com](https://github.com/user-attachments/assets/155a6b74-cf5e-4c5c-b1a0-75f1513f302f)

**[GitHub](https://github.com/vaishnavi070306-commits/git-task)**.

# Task 7: Create a Portfolio Webpage

For this task, I have created a **portfolio webpage** using **HTML**. The purpose of the webpage is to showcase my profile, interests, projects, and social media profiles in a clean and professional manner. 

<img width="1889" height="909" alt="portfoliophoto pngfile" src="https://github.com/user-attachments/assets/2bf1b6ac-5c68-4f29-9b08-d11f3a78ccdc" />

# Task 9: Tinkercad

In this task, a Tinkercad account was used to explore the simulation environment and example circuits. A circuit with an ultrasonic sensor was simulated to measure the distance between the sensor and an object, and the results were displayed on the serial monitor. The ultrasonic sensor works by sending sound waves and calculating the time taken for the echo to return. A basic radar system was also implemented by attaching a servo motor to the sensor, allowing it to rotate and detect objects over a wider area. This experiment helped in understanding distance measurement, servo control, and how these can be combined for object detection. 


![Screenshot_24-1-2026_20252_www tinkercad com](https://github.com/user-attachments/assets/ee988e03-9436-457f-bcb6-eee59867ea0c)


[tinkercad](https://www.tinkercad.com/things/49RVmJZ56W4/editel).

# Task 10: Speed control of DC motor

A 5V DC motor was controlled using an Arduino UNO and an L298N motor driver to explore basic techniques of motor speed and direction control. The motor speed was varied using PWM signals, and the direction was adjusted through the H-Bridge connections. This experiment provided practical experience in connecting the hardware, configuring the motor driver, and using Arduino programming to control motor behavior effectively. The process helped in understanding the application of PWM and H-Bridge circuits in real-world motor control systems.
![WhatsApp Image 2026-01-24 at 12 48 50 PM](https://github.com/user-attachments/assets/4b69214b-91f5-4746-856c-899ac45919bf)

The results showed that the motor responded smoothly to changes in PWM signals, allowing precise control over its speed. Forward and reverse motion was achieved reliably by switching the H-Bridge input pins, and the motor maintained stable operation across different speed settings. Recording the experiment confirmed that the setup worked as intended and demonstrated the practical effectiveness of using Arduino and L298N driver for DC motor control.

https://github.com/user-attachments/assets/6ee82cbf-0ec9-4ff7-8195-8dd657b52d8b



## Task 12: Soldering Prerequisites

I studied the soldering equipment available in the laboratory, including the soldering iron, solder wire, flux, and soldering wick, and learned their functions.  
I practiced basic soldering techniques on a perf board by assembling a simple LED setup under the supervision of a coordinator.  
This experiment helped me understand proper handling and usage of soldering tools.



<img src="https://github.com/user-attachments/assets/36945e5e-560f-41c9-8e9b-52f7aedc1443" width="400"/>

<img src="https://github.com/user-attachments/assets/b8202e0d-2ead-4660-8f66-fdaab8603fbd" width="400"/>

## Task 14: Karnaugh Maps and Deriving The Logic Gate

In this task, I designed a simple burglar alarm using two inputs: **Door (D)** and **Key (K)**. The alarm turns ON only when the door is open and the key is not pressed. I created a **truth table** for all four cases, then used a **Karnaugh Map (K-Map)** to simplify the logic. The resulting Boolean expression is **A = D · K̅**, which I implemented using a **NOT gate** for the key input and an **AND gate** to drive the buzzer or LED. This exercise helped me understand how K-Maps simplify logic for practical circuits.

# Task 16:Data sheet report writing

## Introduction

The **L293D** is a dual H-bridge motor driver IC commonly used to control **the direction and speed of DC motors**. It allows a microcontroller or logic circuit to drive motors that require higher current than the controller can supply. The IC contains **two full H-bridge circuits**, enabling **independent bidirectional control of two DC motors**.

## IC Configuration

![WhatsApp Image 2026-01-17 at 7 00 02 PM](https://github.com/user-attachments/assets/99f52530-2052-4e44-b53a-e1e59bf16c9e)


- **Package:** 16-pin Dual In-Line Package (DIP)  
- **Logic Supply (VSS):** 5 V, powers the internal control circuitry  
- **Motor Supply (VS):** 4.5–36 V, powers the motors directly  
- **Ground Pins:** 4, all connected to a common ground  
- **Control Pins:**  
  - **IN1 & IN2:** Set the direction of Motor A  
  - **IN3 & IN4:** Set the direction of Motor B  
  - **EN1 & EN2:** Enable Motor A and allow PWM speed control  
  - **EN3 & EN4:** Enable Motor B and allow PWM speed control  
- **Output Pins:**  
  - **OUT1 & OUT2:** Motor A terminals  
  - **OUT3 & OUT4:** Motor B terminals  

### Pin Logic

| Inputs | Enable | Motor Operation |
|--------|--------|----------------|
| 0,0    | 1      | Motor stopped  |
| 0,1    | 1      | Motor rotates clockwise |
| 1,0    | 1      | Motor rotates counter-clockwise |
| 1,1    | 1      | Motor stopped  |
| X,X    | 0      | Motor disabled |

> **Note:** `X` can be either 0 or 1. Speed control is done by applying a **PWM signal** to the Enable pins.

## Internal IC Components

- The L293D uses **Darlington transistor pairs** to amplify current, enabling it to drive motors requiring high current.  
- Each motor channel has a **complete H-bridge**, allowing current to flow in either direction through the motor.  
- **Clamp diodes** are included internally to protect the IC from **back EMF** generated by inductive loads like motors.  
- Two H-bridges allow **independent control of two motors** simultaneously.


## H-Bridge Functionality

![WhatsApp Image 2026-01-17 at 7 02 57 PM](https://github.com/user-attachments/assets/b7f9cd53-8d5d-46d2-8d97-a15ee49315a0)


An H-bridge is a circuit that allows a motor to be driven **forward or backward**. In the L293D:

- Input pins control the direction of current through the motor.  
- Enable pins turn the H-bridge on or off, and PWM signals applied to these pins allow **speed control**.  
- The internal Darlington pairs increase the current capability of the IC, enabling it to safely drive motors up to **600 mA continuously** and up to **1.2 A peak** per channel.


## PWM Speed Control

- **Pulse Width Modulation (PWM)** is applied to the Enable pins.  
- By changing the duty cycle of the PWM signal, the **average voltage applied to the motor changes**, which controls the speed.  
- This method allows smooth motor speed regulation **without adjusting the motor supply voltage (VS)**.

## Applications

- Robotics and automation projects  
- Embedded systems requiring bidirectional motor control  
- Educational experiments for motor interfacing  
- Small electric vehicles or conveyor systems

# TASK 17:Introduction to VR

## What is Virtual Reality?

Virtual Reality (VR) is a technology that creates a **simulated environment**, allowing users to feel as though they are present in a completely different place or world. VR places the user inside a **computer-generated environment** that feels real and immersive.

This is achieved using special equipment such as a **VR headset**, which covers the eyes and sometimes the ears. The headset blocks out the physical world and replaces it with a **believable, interactive 3D environment** that users can explore and interact with, creating a strong sense of presence.

## How Virtual Reality Works

Virtual Reality works by using a **head-mounted display (HMD)** combined with **input tracking systems**.

- The display is split between the two eyes, creating a **stereoscopic 3D effect**
- Stereo sound enhances realism and depth
- Images are fed at **slightly different angles** to each eye, creating the illusion of depth and solidity
- LCD or OLED panels, combined with lenses, fill the entire field of vision
- Sensors track head movement and user input to update the virtual world in real time

Together, these technologies create an **immersive and believable digital world** generated entirely by a computer.

## Evolution of Virtual Reality

Although VR feels like a modern invention, it has existed in various forms for **decades**. Early examples include **360° panoramic paintings**, which surprised audiences by creating a sense of immersion long before digital VR existed.

![WhatsApp Image 2026-01-18 at 11 47 45 AM](https://github.com/user-attachments/assets/4f13c1ca-36ee-47a0-98e1-753987f0adad)

Virtual Reality can be considered the **“wise mind” of the digital world**—it creates an environment that functions independently of the user while still allowing interaction. It offers first-hand experiences of events and scenarios, including their psychological after-effects.

This makes VR a powerful tool for understanding **human perception, cognition, and behavior**.

## Difference Between Virtual Reality (VR) and Augmented Reality (AR)

![WhatsApp Image 2026-01-18 at 11 54 25 AM](https://github.com/user-attachments/assets/cbe751db-f4ef-47e9-909d-bdaa2d8b58c6)

| Feature | Virtual Reality (VR) | Augmented Reality (AR) |
|------|---------------------|------------------------|
| Definition | Creates a fully immersive digital environment | Overlays digital elements onto the real world |
| User Experience | Completely replaces the real world | Enhances the real world with digital content |
| Hardware Requirement | Requires VR headsets or similar devices | Works on smartphones, tablets, or AR glasses |
| Awareness of Reality | User is isolated from the real world | User remains aware of the real environment |
| Technology Complexity | Requires powerful hardware and software | Requires relatively simpler technology |
| Examples | PlayStation VR, Samsung Gear VR, HTC Vive | Pokémon GO, Google Maps AR, IKEA AR App |


## Emerging Trends in Virtual Reality and Space Technology
### 1. Mixed Reality Integration
Devices like **Apple Vision Pro+** and **HTC Vive XR Elite 2** blend virtual objects with the physical world. This mixed reality approach is transforming design, training, and collaboration.
### 2. Wireless, All-in-One Devices
Standalone VR headsets no longer require external PCs or consoles. Devices like **Meta Quest 4** offer high-resolution graphics, longer battery life, and complete freedom of movement.
### 3. Eye-Tracking and Hand-Gesture Controls
Advanced sensors track eye movement and hand gestures, enabling intuitive navigation, realistic avatars, and optimized rendering for smoother performance.
### 4. VR in Education and Healthcare
- Schools use VR for immersive lessons in science, history, and engineering  
- Hospitals apply VR for pain management, surgical training, and therapy  
### 5. Virtual Workspaces
Remote teams collaborate in **3D virtual offices**, conducting meetings, presentations, and co-editing 3D models beyond traditional video calls.
### 6. Teleoperation of Spacecraft and Rovers
VR enables precise teleoperation of spacecraft and robotic rovers, bridging the gap between Earth and space missions.
### 7. Designing and Testing Space Equipment
Engineers use VR to design, test, and validate spacecraft components in simulated environments before physical production.
### 8. Mission Training and Simulation
Astronauts and engineers train in **risk-free virtual simulations**, preparing for critical space mission operations.

## Top Virtual Reality Companies in India
### 1. Absentia VR:Specializes in VR content creation tools and immersive experiences for entertainment and education.
### 2. SmartVizX:Provides VR solutions for architecture, engineering, and construction with immersive virtual walkthroughs.
### 3. SimulanisDevelops immersive training platforms for industries such as manufacturing and pharmaceuticals.
### 4. ImagineFocuses on AR and VR collaboration platforms, with its flagship product **NuSpace** enabling virtual meetings and teamwork.
### 5. VeativeOffers immersive learning solutions with one of the world’s largest **curriculum-aligned VR libraries for STEM education**.





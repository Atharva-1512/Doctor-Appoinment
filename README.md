🏥 Doctor Appointment System

Client-Server Based Healthcare Scheduling System using Socket Programming

📌 Overview

This project is a Doctor Appointment Scheduling System built using Python socket programming. It simulates real-world communication between patients, doctors, and a health center server using both TCP and UDP protocols.
The system allows patients to:
Authenticate
View available doctor slots
Book appointments
Receive estimated consultation costs
The architecture follows a multi-phase client-server model, making it a strong demonstration of networking concepts.

🚀 Key Features
✅ Client-Server Architecture
Central Health Center Server
Multiple Patients & Doctors as clients
✅ Hybrid Communication
TCP → Authentication & scheduling
UDP → Cost estimation (real-time doctor-patient interaction)
✅ Appointment Scheduling
Dynamic slot availability
Prevents double booking
Real-time updates for multiple users\
✅ Database Integration
Uses SQLite database (Vidhi.db)
Stores doctor & patient information
✅ Multi-User Simulation
Supports multiple doctors and patients running simultaneously

🛠️ Tech Stack
Language: Python

Concepts Used:
Socket Programming (TCP & UDP)
Client-Server Architecture
Networking Protocols
Database: SQLite
Environment: CLI-based execution


📂 Project Structure

Doctor-Appoinment/
│── healthcenterserver.py   # Main server
│── doctor1.py              # Doctor client 1
│── doctor2.py              # Doctor client 2
│── patient1.py             # Patient client 1
│── patient2.py             # Patient client 2
│── Vidhi.db                # SQLite database
│── 2-Create-Table.py       # DB table creation
│── insert scripts          # Data insertion scripts
│── read scripts            # Data retrieval scripts
│── README.md


⚙️ How It Works

The system operates in 3 phases:

🔐 Phase 1: Authentication

Patient connects to server via TCP

Server verifies patient credentials

📅 Phase 2: Appointment Scheduling

Server sends available doctor slots

Patient selects a preferred time slot

Slot gets reserved and removed from availability

💰 Phase 3: Cost Estimation

Patient connects to doctor via UDP

Doctor calculates and sends consultation cost based on insurance

👉 This hybrid approach demonstrates real-world protocol usage where reliability (TCP) and speed (UDP) are both needed.

▶️ Execution Steps

Run files in the following order:

python healthcenterserver.py
python doctor1.py
python doctor2.py
python patient1.py
python patient2.py

📊 Sample Workflow
Start server → displays doctors & patients data
Start doctors → wait for patient connections
Patient logs in → selects available slot
Slot gets booked → removed for other patients
Patient receives cost from doctor via UDP

🔥 Key Learning Outcomes
Practical implementation of TCP vs UDP
Understanding multi-client communication
Real-world simulation of distributed systems
Database integration with networking
Handling concurrency & synchronization

🚧 Future Improvements
Add GUI (Tkinter / Web UI)
Convert to full-stack web app (React + Node.js)
Implement authentication system (JWT)
Add real-time notifications
Deploy as cloud-based service

💡 Use Cases
Hospital appointment systems
Networking academic projects
Distributed system simulations
Backend system design practice

👨‍💻 Author
Atharva Gade
BE IT (SPPU)
AI/ML Enthusiast
Interested in Backend Systems & Distributed Computing

🏥 Doctor Appointment System
Client-Server Based Healthcare Scheduling System








📌 Overview

The Doctor Appointment System is a client-server based healthcare scheduling application developed using Python socket programming.

It simulates real-world communication between patients, doctors, and a centralized health center server using both TCP and UDP protocols.

The system enables patients to authenticate, view available slots, book appointments, and receive consultation cost estimates—demonstrating core concepts of networking and distributed systems.

🚀 Key Features
✅ Client-Server Architecture
Centralized health center server
Multiple doctor and patient clients
Supports concurrent multi-user interactions
✅ Hybrid Communication Model
TCP Protocol → Secure and reliable communication for authentication & scheduling
UDP Protocol → Fast, real-time communication for consultation cost estimation
✅ Appointment Scheduling System
Dynamic doctor slot availability
Prevention of double booking
Real-time updates across multiple clients
✅ Database Integration
SQLite database (Vidhi.db)
Stores patient and doctor data
Supports persistent data management
✅ Multi-User Simulation
Simulates multiple doctors and patients running simultaneously
Demonstrates concurrency and synchronization handling
🛠️ Tech Stack
Category	Technology
Language	Python
Networking	Socket Programming (TCP & UDP)
Architecture	Client-Server Model
Database	SQLite
Environment	CLI-Based Execution
📂 Project Structure
Doctor-Appointment/
│
├── healthcenterserver.py    # Central server
├── doctor1.py               # Doctor client 1
├── doctor2.py               # Doctor client 2
├── patient1.py              # Patient client 1
├── patient2.py              # Patient client 2
├── Vidhi.db                 # SQLite database
├── 2-Create-Table.py        # Database setup script
├── insert_scripts/          # Data insertion scripts
├── read_scripts/            # Data retrieval scripts
└── README.md
⚙️ System Workflow

The application operates in three distinct phases:

🔐 Phase 1: Authentication
Patient connects to the server using TCP
Server validates user credentials
📅 Phase 2: Appointment Scheduling
Server provides available doctor time slots
Patient selects a preferred slot
Slot is reserved and removed from availability
💰 Phase 3: Cost Estimation
Patient communicates with doctor using UDP
Doctor calculates consultation cost based on insurance details
Cost is sent back in real time

This hybrid model effectively demonstrates the use of reliable (TCP) and low-latency (UDP) communication in real-world systems.

▶️ Execution Steps

Run the components in the following order:

python healthcenterserver.py
python doctor1.py
python doctor2.py
python patient1.py
python patient2.py
📊 Sample Workflow
Start server → initializes doctor and patient data
Launch doctor clients → ready to accept requests
Patient logs in → retrieves available slots
Appointment is booked → updated across system
Patient receives consultation cost via UDP
🔥 Key Learning Outcomes
Practical implementation of TCP vs UDP protocols
Understanding multi-client communication systems
Hands-on experience with distributed system concepts
Integration of database with network applications
Handling concurrency and synchronization
🚧 Future Enhancements
🖥️ Graphical User Interface (Tkinter / Web UI)
🌐 Full-stack migration (React + Node.js)
🔐 Secure authentication (JWT-based)
🔔 Real-time notifications
☁️ Cloud deployment and scalability
💡 Use Cases
Hospital appointment management systems
Academic networking and distributed system projects
Backend system design practice
Simulation of real-world service architectures
👨‍💻 Author

Atharva Gade
🎓 BE IT (SPPU)
🤖 AI/ML Enthusiast
⚙️ Interested in Backend Systems & Distributed Computing


🏆 Recruiter Note

This project demonstrates:

Strong understanding of network protocols and socket programming
Ability to design scalable client-server architectures
Practical implementation of distributed systems concepts
Backend-focused problem solving with real-world relevance

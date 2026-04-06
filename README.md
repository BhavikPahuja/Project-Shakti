# Project-ShaktiProject Shakti: Ecosystem Overview
Project Shakti transforms school safety from a passive compliance task into an active, intelligent, and highly responsive system. By combining high-speed real-time networks with predictive AI, it ensures schools in Punjab are continuously prepared for, and capable of responding to, any emergency scenario.

1. Frontend Architecture (The Client Layer)
The user-facing interfaces are split into role-specific platforms to ensure everyone has exactly what they need during a crisis or training session.

Admin Command Dashboard (React & Vite): * A high-performance web interface designed for school principals and safety officers.

Displays macro-level analytics, school-wide "Readiness Scores," and live maps of the campus during emergencies.

Allows admins to trigger campus-wide alerts instantly.

Teacher & Staff Tactical App (Flutter / React Native):

A cross-platform mobile application built for fast, on-the-go access.

During an emergency, teachers use this to mark their assigned students as "Safe," "Injured," or "Missing," which feeds directly into the central Admin Dashboard.

Includes a one-tap SOS feature for localized threats (e.g., medical emergencies in a classroom).

Student Learning Portal (Web/Mobile):

An accessible portal focused on education and engagement.

Hosts the gamified safety modules, quizzes, and digital rewards, ensuring students know their evacuation routes and basic first aid.

2. Backend Infrastructure (The Core Engine)
The backend is designed for extreme reliability and low latency, ensuring that critical data is never bottlenecked during an actual disaster.

API & Logic (Node.js & Express.js): Acts as the central nervous system, handling authentication, data routing, and the logic for the gamification engine.

Real-Time Communications (WebSockets): Bypasses standard HTTP delays to provide instant, bi-directional communication. This ensures that the moment an Admin hits "Evacuate," every Teacher's phone rings instantly, and every "Safe" status update appears on the Admin's screen in milliseconds.

Database (MongoDB): A flexible NoSQL structure perfect for handling diverse datasets—from standard user profiles and login credentials to highly unstructured data like live chat logs during an emergency and dynamic school blueprints.

3. AI & Machine Learning Implementations (Python & TensorFlow)
This is where Project Shakti shifts from a reactive tool to an intelligent, proactive safety advisor. These microservices run in Python and communicate with the Node.js backend.

AI Mock Drills (Adaptive Drill Advisor): * Instead of doing a fire drill once a year on a fixed date, the AI analyzes weather patterns, school capacity, and time elapsed since the last drill (calculating a "skill decay" curve).

It dynamically triggers recommendations for specific mock drills exactly when the school's readiness dips below a safe threshold.

Student Performance-Based Resource Recommendation: * The model analyzes how students perform in their gamified learning modules.

If the data shows that 8th graders are consistently failing the "Earthquake Protocol" quizzes, the AI automatically recommends that administrators allocate more training resources to that specific grade or schedule a targeted, micro-drill for that wing of the school.

Computer Vision (YOLOv8) Hazard Detection: Integrates with CCTV to map crowd density during evacuations and spot physical hazards (like blocked fire exits) before they cause harm.

NLP Distress Triaging: Analyzes text inputs from teachers during an event, identifying keywords to prioritize rescue efforts (e.g., flagging a message that says "trapped" higher than one that says "waiting for instructions").

4. Core Platform Features
Bringing the tech stack together, these are the primary operational features of the platform:

Gamified Education Engine: Replaces boring safety manuals with interactive modules that reward students for learning life-saving protocols.

Real-Time "Safe/Missing" Roster: A live-updating digital headcount system that eliminates the chaos of paper clipboards during an evacuation.

Predictive Resource Logistics: Digitally maps all safety infrastructure (fire extinguishers, medical kits) and uses predictive logic to warn administrators before items expire or require maintenance.

Multi-Tiered Alert Network: Capable of sending silent alerts (for localized threats like an intruder) or blaring, campus-wide push notifications that override phone silent modes for immediate evacuations.
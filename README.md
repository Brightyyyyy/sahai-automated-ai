# 🏥 SAHAY: Intelligent Conversational AI for Automated Appointment Scheduling

An AI-powered conversational system that automates hospital appointment booking, rescheduling, and cancellation through natural language — accessible via both chat and voice, built on a serverless, LLM-driven architecture.

---

## 📌 Overview

In many hospitals, appointment booking is still handled manually at the reception desk — patients must call or visit in person to book, reschedule, or cancel appointments, leading to long wait times, heavy staff workload, and inefficiency during peak hours. These issues are especially critical for elderly patients and people from rural areas with limited access.

SAHAY solves this with an AI-powered conversational agent that lets patients interact naturally — by chat or voice — to manage appointments end-to-end. The system understands patient intent (booking, rescheduling, cancelling), checks doctor availability by specialty, displays open time slots, collects patient details, and confirms the appointment automatically — functioning as a 24/7 virtual receptionist that reduces manual workload without replacing hospital staff.

---

## 🧠 System Architecture

SAHAY is built on a **five-layer architecture**:

1. **User Interaction Layer** — web-based chat interface and voice input via telephony
2. **AI Processing Layer** — a large language model (Google Gemini) interprets user intent and drives responses
3. **Serverless Logic Layer** — Netlify Functions handle scalable, event-driven backend processing with no server management overhead
4. **Data Management Layer** — Supabase PostgreSQL securely stores and manages patient and appointment data with ACID compliance
5. **Dashboard & Analytics Layer** — real-time monitoring and reporting for hospital administrators

**Data flow:** A user sends a message or speaks through a phone call → speech is converted to text if needed → the LLM identifies intent → it triggers the relevant microservice (e.g. `bookAppointment`) → the microservice interacts with the database → a confirmation is sent back → the admin dashboard updates automatically.

---

## 🧩 Module Breakdown

| Module | Responsibility |
|---|---|
| **Conversational UI** | Chat interface with speech input/output support, accessible design |
| **AI Engine** | Intent detection and structured tool invocation for semantic accuracy |
| **Appointment Manager** | Booking, rescheduling, cancellation, and conflict validation |
| **Database Security** | Encrypted communication and strict API-based access control |
| **Admin Dashboard** | Real-time analytics, appointment logs, and doctor availability overview |

---

## 🛠️ Tech Stack

- **Frontend:** React, HTML, CSS, JavaScript
- **Backend:** Node.js, Netlify Functions (serverless)
- **AI:** Google Gemini (LLM) for intent detection and natural language understanding
- **Telephony:** Exotel API for voice-based interaction
- **Database:** Supabase PostgreSQL (ACID-compliant)

---

## 🎯 Key Objectives

- Understand natural language to assist users in appointment scheduling
- Support both text and voice interaction for booking, rescheduling, and cancellation
- Automate healthcare workflows through serverless microservices
- Maintain secure, consistent data handling with ACID-compliant architecture
- Provide a real-time administrative dashboard for hospital staff
- Reduce dependency on manual reception work and eliminate human error
- Ensure the system remains scalable, modular, and cost-effective

---

## 📊 Data Handled

- **User information** — contact and identity details
- **Appointment logs** — bookings, reschedules, cancellations, and status
- **Doctor profiles** — specialty and availability schedules
- **Department listings** — medical specialties for filtering and analytics

---

## 🚀 Future Enhancements

- Real-time WebSocket messaging for instant updates and notifications
- Multi-language voice support for broader accessibility
- A revamped React dashboard with richer visual analytics
- Integration with Electronic Health Records (EHR) systems
- ML-based appointment prediction to optimize scheduling and reduce wait times
- Automated reminders and follow-ups to reduce no-shows

---

## 🎓 Project Context

Developed as a major project for the Bachelor of Technology degree in Computer Science & Engineering (Data Science), involving requirement analysis, system design, AI integration, database setup, telephony integration, implementation, testing, and deployment as part of the full project lifecycle.

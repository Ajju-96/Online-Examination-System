# 🎓 Online Examination System (OES)

> A robust, web-based platform designed to automate assessment workflows, transitioning examination processes from manual paperwork to a secure, paperless digital environment.

---

## 📖 Table of Contents
- [Overview](#-overview)
- [Key Features](#-key-features)
- [System Architecture](#-system-architecture)
- [Tech Stack](#-tech-stack)
- [Workflow](#-workflow)

---

## 📝 Overview

The **Online Examination System** is a web application engineered to conduct "paperless examinations," significantly reducing human workload through automated processing. The system acts as a unified "two-way road," handling interactions between the examiner and the candidates seamlessly.

It is designed to be versatile, capable of conducting examinations over the **Internet** globally or within a specific geographical region using **LAN/Intranet** for organizations.

---

## 🌟 Key Features

### Examination Modes
The system supports dual assessment methods to cater to different academic needs:
* **Objective Type:** Fully automated checking process carried out directly by the system for instant grading.
* **Subjective Type:** Supports descriptive answers where candidate responses are securely sent to an examiner for manual review and mark assignment.
* **Graphical Support:** Unlike legacy systems restricted to simple text, this platform integrates CMS tools to present **graphical and image-based questions**.

### Security & Integrity
To ensure a fair testing environment, the system implements rigorous security protocols:
* **Candidate Isolation:** Keeps each candidate "invisible" to others to prevent collusion.
* **Randomized Question Sets:** Provides different questions to different systems simultaneously.
* **Browser Locking:** Configures browser settings to disable minimization and restrict the use of other devices.
* **Session Control:** Automatically disables answer options once the time limit is reached.

### Time Management
* **Dual Timer Mechanism:** The system features two distinct timers—one for individual questions and another for different exam sections.
* **Auto-Transition:** Upon reaching the specified time limit, questions automatically change, and servlets forward the user to the next module upon completion.

---

## 🏗 System Architecture

### Problem Statement (Existing System)
The legacy systems previously in use suffered from significant technical drawbacks:
* **Data Redundancy:** Entering the same data into different tables was not possible without consistency errors.
* **Database Inefficiency:** Updates required additional workload, increasing strain on the database.
* **Lack of Relationships:** One-to-one and one-to-many relationships were not implemented effectively.

### Our Solution (Proposed System)
The new **Online Examination System** addresses these issues through:
* **CMS Integration:** Full integration of Content Management System (CMS) concepts and graphical tools.
* **Role-Based Examiners:** The system distinguishes between two examiner types—one for checking objective questions and another for descriptive questions.

---

## 💻 Tech Stack

* **Backend:** Java (Servlets) for module forwarding and logic processing.
* **Frontend:** HTML, CSS, JavaScript (Graphical tools integration).
* **Database:** SQL (Resolved data redundancy and relationship mapping).
* **Deployment:** Supports LAN, Intranet, and Internet-based hosting.

---

## 🔄 Workflow

1.  **Candidate Application:** Candidates apply for the exam and receive login credentials.
2.  **Exam Execution:**
    * The browser is locked down to prevent minimization.
    * Questions (Text or Graphical) are presented with a strict timer.
3.  **Submission:**
    * **Objective:** Auto-graded by the system immediately.
    * **Subjective:** Answers are routed to the specific examiner panel for review.
4.  **Results:**
    * Admins configure the results display section as per requirements.
    * Candidates receive results either immediately after completion or via email.

---

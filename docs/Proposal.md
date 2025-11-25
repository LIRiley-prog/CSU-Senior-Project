Meccanoid AI Robot
===================================================
**Student Name(s)**: Logan Riley  
**Degree and Major**: B.S. in Applied Computing with Business Concenttion  
**Project Advisor Name**: Dr. Hayes  
**Expected Graduation Date**: May 2026  

**GitHub Repository Link**
https://github.com/LIRiley-prog/CSU-Senior-Project 

Problem Statement
-----------------
The majority of consumer robots are toys with limited interactivity, often relying on preprogrammed movement and basic voice commands. These qualities render them unsuitable as functional assistants, learning aids, or adaptable devices for real world application. My project solves the problem of changing an available robot (the Meccanoid G15) into an intelligent system with natural language understanding, dynamic interactivity, and independent decision making by integrating artificial intelligence and modern computing features.

Project Description
-------------------
The task involves re-programming a Meccanoid G15 robot with advanced AI features. The central objective is to replace the toy-like, command-based interface with an adaptive and conversational one. The robot will be connected to a local server that serves a lightweight large language model for speech-to-text, intent recognition, and response generation.

The system will allow the robot to:
- Respond verbally in real-time.
- Learn from human interaction to improve future output.
- Make motorized actions (walking, waving, pointing, dancing) to accompany conversation prompts.
- Demonstrate possible uses for customer support, education, or companionship.
- This project combines hardware programming, AI integration, and robotics control to demonstrate an everyday application of machine learning to physical systems.

Proposed Implementation Language(s)
-----------------------------------
C++  
Python  

Libraries, Packages, Development Kits, etc., to be used in the proposed implementation language(s)
--------------------------------------------------------------------------------------------------
Speech Recognition: Vosk, Whisper, or SpeechRecognition  
LLM Integration: local LLM (via Ollama)  

Additional Software/Equipment Needed
------------------------------------
Hardware: Meccanoid G15 robot, USB/Bluetooth interface, local server.  
Software: Visual Studio Code (IDE), Python and C++ compilers, GitHub for version control.  
Testing/Deployment: Local test bench with microphone and speaker setup.  

Alternative Solutions and Rationale #
--------------------------------------
> **Purpose**: Describe at least two alternative solutions or approaches to your project. Compare these with your chosen solution based on relevant criteria (e.g., feasibility, scalability, cost, performance, usability). Explain why you selected your final approach.

### Alternative 1
- **Description**:  
  _Use a cloud-based AI API (like OpenAI API or Google Dialogflow) to handle robot responses._
- **Pros**:  
  - _Fast setup with powerful AI models_  
  - _No need for heavy local computation_
- **Cons**:  
  - _Requires constant internet connection_  
  - _Potential privacy/security concerns with cloud data_  
  - _Higher costs due to API usage_

### Alternative 2
- **Description**:  
  _Keep the Meccanoid’s default programming and only add basic speech recognition modules for command expansion._
- **Pros**:  
  - _Simpler to implement_  
  - _Less resource-intensive_
- **Cons**:  
  - _Limited interactivity and no real intelligence_  
  - _Fails to demonstrate innovation or AI application_

### Chosen Solution and Rationale
- **Chosen Solution**:  
  _Reprogram the Meccanoid with a local AI model running on Python, integrated with C++ for motor control._
- **Rationale**:  
  _This balances viability, cost, and creativity. It avoids cloud reliance, maintains user privacy, and showcases technical expertise in AI and robotics. It is more complex but provides a stronger demonstration of real-world AI integration._

Personal Motivation
-------------------
I grew up taking apart electronics and learning how machines work, and I have always been fascinated by the idea of robots that could think and interact with people. This project lets me combine my interests in AI, computing, and hands-on robotics. It will also prepare me for a career in IT or AI systems analysis by giving me practical experience in integrating software with hardware.

Outline of Future Research Efforts
----------------------------------

### **1. Learn the Meccanoid G15’s SDK or Reverse-Engineer Motor Control**
**Goal:** Understand how to send movement commands (walk, wave, turn, nod).  
**First Steps:**  
- Study the Meccanoid protocol documentation from PenguinTutor:  
  https://www.penguintutor.com/news/linux/meccanoid  
- Watch YouTube tutorial: “Reverse Engineering Meccanoid Protocol.”  
- Use a USB/Bluetooth serial adapter to manually send Meccanoid servo commands.  
- Write a small C++ test program to trigger a known action (“wave”).  
**Outcome:** A functioning C++ motor control module.

### **2. Research and Test Lightweight LLMs for Local Deployment**
**Goal:** Choose a model small enough to run locally with low latency.  
**First Steps:**  
- Install Ollama on a laptop/server.  
- Test these models: Phi-3 Mini, Gemma 2B, Mistral 7B (quantized).  
- Follow Ollama’s tutorial “Using Ollama with Python.”  
- Create a Python timing script to benchmark response speed.  
**Outcome:** A chart comparing speed, accuracy, and resource usage.

### **3. Explore Speech Recognition Libraries and Optimize for Real-Time Interaction**
**Goal:** Achieve accurate voice recognition with <1 second delay.  
**First Steps:**  
- Test Vosk with Python using the “Offline Speech Recognition with Vosk” tutorial.  
- Install and test Whisper.cpp using its GitHub quick-start guide.  
- Measure real-time accuracy at different mic distances.  
- Add wake-word detection (“Hey Mecca”) using Porcupine demo models.  
**Outcome:** Working speech-to-text pipeline for the robot.

### **4. Develop Integration Between AI Responses and Robotic Gestures**
**Goal:** Make conversations feel natural with synced speech + movement.  
**First Steps:**  
- Create a mapping table that links AI intents to gestures.  
- Write a Python function that detects keywords from the LLM output.  
- Follow the tutorial “Sending Servo Commands via Python Serial.”  
- Build a timing system so movements trigger after the robot speaks.  
**Outcome:** Gesture enhanced dialogue sequences.

### **5. Test User Scenarios (Greeting, Q&A, Movement Commands)**
**Goal:** Validate whether robot behavior matches expected human interaction.  
**First Steps:**  
- Script 10 basic interaction tests (hello, walk, wave, questions).  
- Write Python unit tests for each scenario.  
- Log accuracy, delay, and gesture success rate.  
- Record short testing videos for evaluation.  
**Outcome:** A performance report with improvements based on observed results.

Schedule #
-----------
*Fall 2025 - CSCI 497*  
- August 15 - Research ideas for senior project  
- September 7 - Bring idea to advisor  
- October 6 - Dft proposal  
- November 25 - Completed Proposal / Requirements Document  
- December 1 - Deeper research for project  

*Spring 2026 - CSCI 498*  
- December 10 - Implement test plan  
- December 14 - Evaluate test results  
- December 20 - Apply updates and bug fixes based on the results  
- December 27 - Progress presentation / advisor feedback  
- January 4 - Finish Design Documentation  

*Spring 2026 - CSCI 499*  
- January 15 - Begin structured user intection testing  
- January 20 - Apply bug fixes, optimize robot features  
- February 14 - Final round of user testing / create performance data  
- Apr 25 - Final project documentation  
- May 1 - Final defense / project presentation  

References #
-------------
[(https://www.meccano.com/product/meccanoid-g15-personal-robot-model-1/)]  
[https://www.penguintutor.com/news/linux/meccanoid]  

Phase 5: Project Demonstration & Documentation 
Title: AI-Powered Supply Chain Management 
1. Objective 
The objective of Phase 5 is to comprehensively evaluate the performance of 
the AI-Powered Supply Chain Management Assistant system built in earlier 
phases and optimize its components. This involves analyzing the system’s 
accuracy, speed, scalability, and user interaction quality under real-world
like conditions. 
 
2. Evaluation Metrics and Tools 
Each component of the system was tested using quantitative metrics and 
standard industry tools: 
Component Key Metrics Tools Used 
Forecasting 
Model 
RMSE, MAE, R², prediction 
latency 
Python (scikit-learn, 
pandas) 
Chatbot Interface Average response time, intent 
recognition rate 
Manual tests, spaCy, 
Google Translate API 
IoT Data 
Integration 
Data refresh rate, fault 
tolerance 
Simulated JSON sensor 
feeds 
Blockchain 
Simulation 
Transaction finality, block 
generation time 
Python + manual hash 
tampering checks 
Security 
Framework 
AES decryption accuracy, 
access control success 
Simulated attack logs, RBAC 
simulator 
 
3. Experimental Design 
• Test Users: 10 internal testers (team members and classmates). 
• Simulated Products: 10 SKU samples with diverse sales behavior. 
Page | 4 
 
• Forecast Horizon: 7-day and 30-day ahead predictions. 
• IoT Simulation: CSV feeds generated every 5 seconds mimicking stock 
levels and transit info. 
• Security Testing: Attempted unauthorized access, role mismatches, key 
revocation, and encryption/decryption validation. 
 
4. Optimization Strategies 
The system was optimized based on Phase 4 testing results: 
• AI Model: Hyperparameter tuning increased R² score from 0.67 to 0.84. 
• Chatbot: NLP model reduced average response time from 2.3s to 1.1s. 
• IoT Data Handling: Added buffering to minimize missed sensor readings. 
• Blockchain Ledger: Switched to simulated batch processing to reduce 
block confirmation time. 
• Security: Introduced simulated AES-256 rotating keys for session 
encryption. 
 
5. System Architecture Summary 
A high-level architecture of the Phase 5 prototype is summarized below: 
• Frontend: Chatbot interface (text-based) integrated into the SCM 
dashboard. 
• Backend: Python services for ML inference, IoT feed parsing, and 
blockchain simulation. 
• Data Layer: CSV and JSON files simulating databases and sensor feeds. 
• Security: AES encryption, role-based access simulation, session 
validation. 
• Integration Layer: Interfaces between chatbot, forecast engine, and data 
feeds. 
 
Page | 5 
 
6. Extended Testing Results 
Test Scenario Result 
Forecast for fast-moving 
product Predicted demand: 132 units (actual: 128) 
Chatbot Hindi interaction 96% accuracy in interpretation and response 
IoT feed simulation (12 hrs) 98.7% of feeds received and processed 
correctly 
Unauthorized role access 
attempt Blocked and logged successfully 
Smart contract simulation test Payment auto-confirmed for valid shipment 
data 
 
7. User Feedback Summary 
Criteria Rating (1–5) Comment 
Forecast Accuracy 4.5 “Impressive precision; would trust it.” 
Chatbot Usability 4.7 “Smooth and multilingual responses.” 
Dashboard Simplicity 4.2 “Could improve filter options.” 
Security Confidence 4.6 “System felt secure and well monitored.” 
Overall Satisfaction 4.6 “Robust system with practical features.” 
 
8. Outcome and Recommendations 
The optimized system demonstrates: 
• High forecasting accuracy for diverse products. 
• Resilience in handling real-time IoT data. 
• Robust security and role-based access. 
• An intuitive multilingual chatbot aiding supply chain workers. 
Page | 6 
 
Recommended Enhancements: 
• Transition from CSV/JSON to real-time cloud databases (Firebase, 
MongoDB). 
• Integrate real APIs for IoT sensors and shipment tracking. 
• UI/UX improvements to the dashboard (charts, filters, notifications). 
• Expand blockchain features with proof-of-delivery and multi-party 
contracts. 
 
9. Future Work & Handover Guidelines 
Future Enhancements: 
• Support for more languages (e.g., Tamil, Bengali). 
• Real-time cloud deployment on AWS or Azure. 
• Mobile app version of the assistant. 
• AI explainability module for forecast justifications. 
Handover Artifacts: 
• Final codebase (Python scripts + config files). 
• Sample data files (products.csv, orders.csv, iot_feed.json). 
• Admin manual with setup and testing instructions. 
• Performance logs and feedback summary. 

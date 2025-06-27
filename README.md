📘 Project Overview: Digital eGramPanchayat 
🔰 Objective:
Digital eGramPanchayat is a web-based platform aimed at digitizing the functioning of local self-governance bodies (Gram Panchayats). 
It provides a centralized portal where Officers, Staff, and Citizens (Applicants) can interact securely and transparently, helping to improve public service delivery, reduce manual workloads,
and promote digital governance in villages and small towns.

🧩 Stakeholders & Roles:

👨‍💼 Officer (Admin):
The Panchayat Officer oversees and manages all services, applications, and staff actions.
Features:

Secure Firebase-based login. Create, update, and delete government services. View and monitor all citizen applications in real-time.
Approve/reject applications and change status. Manage staff assignments for services. 
Assign approval authority using Officer ID and location filters. 
Real-time updates and monitoring via Firestore onSnapshot.

👨‍🔧 Staff Member (Clerk/Operator):
Assists in processing citizen applications and supports the Officer.
Features:

Secure login using Firebase Authentication. 
Access only to assigned services. 
Can view, mark, or recommend applications for review.
Submit remarks or request additional documents. 
Can update status to “Under Review” or forward to Officer. 
Access is role-based and controlled via Firestore rules.

👨‍🌾 User/Applicant (Citizen):
The resident who applies for a Panchayat service. 
Features:

Register and login using Firebase Auth (email/phone).
View available Panchayat services.
Submit application forms with personal and required service details.
Track application status (Pending / Approved / Rejected). 
Receive auto-updates when application status is changed. 
Upload required documents and Aadhaar. 
View history of previously applied services.

⚙️ Functional Modules: 
Module Description Login Module :
Firebase Authentication for Officer, Staff, and User roles
Service Management :
Officer can create/update/delete services 
Application Submission :
Users can apply for services 
Status Management :
Officer/Staff can update application status 
Role-Based Access :
Officers have full access, staff have limited rights
Notification System :
Auto-alerts on status changes using Firestore triggers

🛠️ Technology Stack: Tech Role HTML/CSS : Front-end UI JavaScript : Client-side logic Firebase Authentication : Login & Role Handling Firebase Firestore : Real-time NoSQL database Firebase Hosting : Website deployment Firebase Cloud Functions : Background operations GitHub Actions : CI/CD for auto-deploy VS Code / GitHub : Development & version control

🔒 Security & Access Control: Officer can access all services and applications. Staff can only access assigned service types (controlled via Firestore roles). Users can only view and track their own applications. Firestore Security Rules ensure data separation and access protection.

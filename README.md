Student Project and Supervisor Allocation System

Course: Software Engineering (CT-365), NED University of Engineering and Technology Group: 05 Repository: SE_CCP_Group05_StudentProjectSupervisorAllocationSystem

Team Member	Roll Number
Bhoomi	TCT-24005
Heer	TCT-24026
Habiba	TCT-24029
About the Project

A web-based application that manages student project proposals, supervisor allocation, proposal reviews, and project progress monitoring. It replaces manual coordination with a single system where students, supervisors, and administrators work with the same data.

User Roles and Features
Role	Main Features
Student	Log in, manage profile, submit a project proposal, view proposal status, view assigned supervisor, submit project progress, view feedback and notifications
Supervisor	Log in, view assigned projects, review proposals, accept or reject proposals, provide feedback, monitor progress, view notifications
Administrator	Log in, manage student and supervisor profiles, set supervisor capacity, allocate supervisors, view allocation records, generate reports

Key rules enforced by the system: role-based access, a supervisor's maximum capacity is checked before every allocation, a project can have only one active supervisor allocation, and notifications are sent when proposals are reviewed and supervisors are allocated.

Technology Stack
Backend: Python, Django
Database: PostgreSQL
Frontend: HTML, CSS, Bootstrap, JavaScript
Architecture: Three-tier (Presentation, Application, Database)
Version control: Git / GitHub
Repository Structure
SE_CCP_Group05_StudentProjectSupervisorAllocationSystem/
├── README.md
├── Proposal/            Project proposal
├── SRS/                 Software Requirements Specification
├── Design/              System Analysis and Design (UML, ERD, architecture, wireframes)
├── SourceCode/          Application source code
├── Tests/               Test cases and test scripts
├── TestReports/         Test execution reports
├── FinalReport/         Final project report
├── Presentation/        Final presentation
└── InputData/           Sample / seed data
Setup and Installation

Adjust the paths and file names below to match the final contents of SourceCode/.

Prerequisites: Python 3.10+, PostgreSQL 14+, Git

bash
# 1. Clone the repository
git clone https://github.com/<username>/<repository-name>.git
cd <repository-name>/SourceCode

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Create the PostgreSQL database and set the credentials
#    (database name, user, password and host in the Django settings file)

# 5. Apply migrations and create an administrator account
python manage.py migrate
python manage.py createsuperuser

# 6. (Optional) Load sample data from ../InputData/

# 7. Run the development server
python manage.py runserver

Open http://127.0.0.1:8000/ in a browser and log in with an Administrator, Supervisor, or Student account.

Running the Tests
bash
python manage.py test

Test cases are in Tests/ and the execution results are in TestReports/.

Documentation

All documentation is submitted in PDF format and kept in the folders above.

Document	Location
Cover Page	Design/ or repository root, as required by the instructor
Proposal	Proposal/
Software Requirements Specification	SRS/
System Analysis and Design	Design/
Test Reports	TestReports/
Final Report	FinalReport/
Final Presentation	Presentation/
File Naming Convention

Team

Developed by Bhoomi, Heer, and Habiba for the Software Engineering (CT-365) course at NED University of Engineering and Technology.# Software-Engineering-Project-NED-UNIVERSITY

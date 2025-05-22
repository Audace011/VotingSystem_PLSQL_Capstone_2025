# VotingSystem_PLSQL_Capstone_2025

# 🗳️ Digital Voting and Election Management System

## 📌 Problem Statement

In many traditional voting systems, the process of managing voter eligibility, preventing multiple votes, tracking real-time results, and auditing user activity is manual and error-prone. These weaknesses can lead to:
- Voting fraud (e.g., multiple voting)
- Ineligible voter participation
- Difficulties in result tracking and auditing
- Poor transparency and scalability

This project proposes a **Digital Voting and Election Management System** developed using **PL/SQL** and Oracle technologies to address these issues through:
- Automated vote recording
- Eligibility verification
- Real-time result tracking
- Secure audit logging and rule enforcement



## ⚙️ Methodology

The system was developed across **seven structured phases**, each contributing to the overall functionality and robustness:

1. **Phase I**: Project Topic Selection – Voting system
2. **Phase II**: Business Process Modeling (BPMN)
3. **Phase III**: Logical Data Modeling (ER Diagram)
4. **Phase IV**: PDB Setup and User Creation
5. **Phase V**: Physical Table Implementation and Sample Data Insertion
6. **Phase VI**: PL/SQL Procedures, Functions, and Sequences
7. **Phase VII**: Triggers and Auditing for Business Rule Enforcement

Technologies used:
- Oracle SQL Developer
- Oracle PDB (Pluggable Database)
- PL/SQL (Procedures, Functions, Triggers)
- GitHub for code management



## 🔷 UML/BPMN Diagrams
 🔷 BPMN Diagram

![Voting BPMN](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20II/BPMN.PNG?raw=true)
  
> 📝 *This diagram models the business process flow: voter registration, candidate setup, voting action, and result tracking. Swimlanes include voters, system, and admin roles.*



## 🔷 Entity Relationship Diagram (ERD)

> ![Voting System ERD](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20III/ERD.PNG?raw=true)  
> 📝 *This ER diagram shows the core relationships between voters, elections, candidates, votes, and results. It enforces data integrity via foreign keys and constraints.*



## 🧪 Screenshots and Explanations

> 📎 **Insert screenshots here showing:**
> - Table creation
> - Sample data
> - Procedure execution (e.g., `cast_vote`)
> - Triggers in action (e.g., duplicate voting error)
> - Vote audit logs

### 📌 Explanations:
- **Table Creation**: The system defines normalized tables for `Voters`, `Elections`, `Candidates`, `Votes`, and `Results`.
- ![Voters Table](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20V/VOTERS.PNG?raw=true)
![Candidates Table](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20V/candidates.PNG?raw=true)
![Elections Table](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20V/elections.PNG?raw=true)
![Candidates Insert Script](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20V/candidates%20ins.PNG?raw=true)
- **Procedure Execution**: `cast_vote` ensures that voters are eligible and haven't already voted before inserting a record.
🔧 Procedure: `cast_vote` Creation

 ![Procedure Creation](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20VI/cast%20vote%20creation.PNG?raw=true)
 ▶️ Procedure: `cast_vote` Execution

![Procedure Execution](https://github.com/Audace011/VotingSystem_PLSQL_Capstone_2025/blob/main/PHASE%20VI/prcedure%20calling.PNG?raw=true)

- **Triggers**: Prevent voting after deadlines and duplicate voting.
- **Audit Logging**: A separate `Vote_Audit` table captures voter actions, improving transparency and traceability.



## ✅ Project Outcomes

- Prevented double voting using both procedures and triggers
- Validated voting eligibility before recording a vote
- Logged each voting action for auditing
- Enforced time-based voting restrictions
- Provided a clear and testable PL/SQL implementation



## 🙌 Author

- **Name**: Karenzi Audace  
- **University**: Adventist University of Central Africa  
- **Project Phase**: PL/SQL Capstone  
- **GitHub Repo**: [your-repo-link-here]




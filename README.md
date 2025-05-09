# Software-modelling-

Great — let’s solve this step by step for your Library Management System (LMS) practical exam. Your paper includes:

Prepare SRS document for LMS

Compute Functional Point, Schedule the project time, and estimate effort

Discuss Component Level Design in detail with diagram

✅ 1. SRS Document for LMS (6 marks)
Software Requirement Specification (SRS) for Library Management System

1. Introduction
Purpose: The LMS automates the operations of a library like managing books, issuing/returning books, tracking members, and handling fines.

Scope: Includes modules for students, librarians, book database, issuing & returning system, report generation, etc.

Users: Admin (Librarian), Students (Users)

2. Functional Requirements
Login/Signup for users and librarian

Search books by title, author, or category

Borrow and return books

Maintain member records

Fine calculation

Book inventory management (add/delete/update books)

Generate reports (daily/weekly/monthly)

3. Non-functional Requirements
System should be secure (user authentication).

High availability and easy to use (UI/UX).

Should support up to 1000 concurrent users.

Daily automatic backup.

4. External Interface Requirements
UI: Web-based interface

Hardware: Minimum 4 GB RAM, Web Server

Software: MySQL, Node.js/Angular (or Java/PHP)

✅ 2. Function Point Calculation, Time, and Effort Estimation (6 marks)
🧮 Step 1: Count Functional Components
Function Type	Count	Complexity	FP Value
External Inputs (EI)	5	Avg	5×4 = 20
External Outputs (EO)	4	Avg	4×5 = 20
External Inquiries (EQ)	3	Avg	3×4 = 12
Internal Logical Files (ILF)	4	Avg	4×7 = 28
External Interface Files (EIF)	2	Avg	2×5 = 10
Total			90

🛠️ Step 2: Adjustment Factor (14 Questions)
Assume ratings are mostly average (rating 3 out of 5), so:

Total rating sum = 14 × 3 = 42

Adjustment Factor = 0.65 + (0.01 × 42) = 0.65 + 0.42 = 1.07

✅ Step 3: Final FP Value
𝐹
𝑃
=
𝑈
𝑛
𝑎
𝑑
𝑗
𝑢
𝑠
𝑡
𝑒
𝑑
𝐹
𝑃
×
𝐴
𝑑
𝑗
𝑢
𝑠
𝑡
𝑚
𝑒
𝑛
𝑡
𝐹
𝑎
𝑐
𝑡
𝑜
𝑟
=
90
×
1.07
=
96.3
 
(round
 
to
 
96)
FP=UnadjustedFP×AdjustmentFactor=90×1.07=96.3 (round to 96)
🕒 Time & Effort Estimation
Assume Productivity Rate = 5 FP/day

So, Time = 96 ÷ 5 = ~19.2 days

Assume Effort Rate = 1 person × 8 hours/day

Effort = 19.2 × 8 = 153.6 hours

✅ 3. Component Level Design with Diagram (6 marks)
📦 Components of LMS
User Interface

Login/Register

Search Books

View Issued Books

Admin Panel (Librarian)

Add/Update/Delete Books

Manage Users

Generate Reports

Book Management Module

Book Inventory

Book Details

Book Categories

Transaction Module

Book Issue/Return

Fine Calculation

Database Layer

Book Table

User Table

Transactions Table

🧩 Component Design Diagram (Textual)
less
Copy code
[UI Layer]
   |
   V
[User Module]      [Admin Module]
     |                  |
     --------------------
             |
    [Book Management Module]
             |
    [Transaction Module]
             |
       [Database Layer]
Yeh pura solution hai aapke practical ke liye. Agar tu chahe toh main is design ka ek figma-type UI diagram bhi bana sakta hoon. Chahiye kya?






You said:
Ei eo eq ilf eif inme kya kya aayega likh do


ChatGPT said:
Bilkul bhai, chalo Library Management System (LMS) ke liye clearly likh dete hain ki:

✅ Function Point Categories with Examples
1. EI – External Inputs (User se data system mai aata hai)
Input Function	Description
User Login / Signup	Student & Librarian login/registration
Add New Book	Librarian adds new book to system
Issue Book	Student/librarian issues book
Return Book	Book return process
Add New Member	Add student/member to system

➡ Total EI = 5

2. EO – External Outputs (System se data bahar jata hai)
Output Function	Description
View Book List	Display all available books
Generate Fine Report	Shows fine report to user/librarian
Generate Book Issue Report	Report of issued books
Member Activity Report	Show each member’s transactions

➡ Total EO = 4

3. EQ – External Inquiries (Data fetch ho raha hai, bina major update ke)
Inquiry Function	Description
Search Book by Title/Author	Simple query search
View Member Profile	Fetch profile without editing
View Issued Books History	Student checks past issued books

➡ Total EQ = 3

4. ILF – Internal Logical Files (System ke andar ke data groups)
Logical File	Description
Book Database	Stores all book details
User Database	Student and librarian login data
Issue/Return Transactions	Record of book issues and returns
Fine Management File	Track fines for overdue books

➡ Total ILF = 4

5. EIF – External Interface Files (Bahar ke system se data use karna)
External File	Description
External Library Catalog API	If it syncs with another library DB
University Student Database	Preloaded student info from college system

➡ Total EIF = 2

Agar tu chaahe toh main inko ek table format mai proper printout-ready bhi bana ke de sakta hoon. Bataa de?

# Student Attendance Support System (SASS)

## 1. Project Overview

The Student Attendance Support System (SASS) is a simple program developed to help teachers and school administrators monitor students' monthly attendance.

The system allows a user to enter a student's name and monthly attendance percentage. It then checks whether the attendance meets the selected minimum attendance threshold of 80%.

Students with attendance below 80% are identified as needing attendance support, while students with attendance of 80% or above are considered to have good attendance.

The program was developed using Flowgorithm as part of the PROG101 Programming Logic assignment.

## 2. Author

- **Name:** Ansu Tucker
- **Student ID:** 905006550
- **Course:** PROG101
- **Institution:** Limkokwing University of Creative Technology, Sierra Leone

## 3. Problem Statement

Student absenteeism can negatively affect academic performance and learning progress. When schools do not monitor attendance regularly, students who frequently miss classes may not receive the support they need.

The Student Attendance Support System provides a simple way to check monthly attendance and identify students whose attendance falls below a selected minimum threshold. This can help teachers recognise possible attendance concerns and take appropriate action.

## 4. Project Objectives

The main objectives of the Student Attendance Support System are to:

- Check students' monthly attendance percentages.
- Identify students whose attendance is below the 80% threshold.
- Validate attendance entries to prevent invalid percentages.
- Display clear attendance results.
- Allow users to check multiple students during one program session.
- Demonstrate the use of functions, modular programming, decisions, loops, and input validation.

## 5. Scope of the Project

The system focuses on checking one student's attendance at a time. The user enters the student's name and monthly attendance percentage. The program validates the percentage, compares it with the selected 80% threshold, and displays the student's attendance status.

The program also allows the user to repeat the process to check another student without restarting the application.

The system is designed as a basic attendance-checking program and does not replace a school's complete attendance management system.

## 6. System Requirements

The following are required to use the program:

- A computer.
- Flowgorithm installed on the computer.
- The SASS Flowgorithm project file (`.fprg`).

## 7. Variables and Constants

The program uses the following variables and constant:

| Variable/Constant | Data Type | Purpose |
|---|---|---|
| `name` | String | Stores the student's name. |
| `attendance` | Integer | Stores the student's attendance percentage. |
| `MinAttendance` | Integer | Stores the minimum attendance threshold of 80. |
| `status` | String | Stores the student's attendance status. |
| `continueChecking` | String | Stores the user's response about checking another student. |

**Constant value:**

`MinAttendance = 80`

The 80% threshold is a design choice for this academic project.

## 8. Functional Modules

The program is divided into three functions to make the solution modular and easier to understand.

### 8.1 Main Function

The `Main` function controls the overall execution of the program. It:

- Requests the student's name.
- Calls `GetValidAttendance()` to obtain a valid attendance percentage.
- Calls `GetAttendanceStatus()` to determine the student's attendance status.
- Displays the student's name, attendance percentage, and status.
- Asks the user whether they want to check another student.
- Repeats the process when the user enters YES and ends when the user enters NO.

### 8.2 GetValidAttendance Function

The `GetValidAttendance()` function is responsible for collecting and validating the attendance percentage.

It checks that the entered attendance is between 0 and 100. If the user enters a value below 0 or above 100, the program displays an invalid-entry message and requests another value.

Once a valid percentage is entered, the function returns the attendance value to the `Main` function.

**Return type:** Integer

### 8.3 GetAttendanceStatus Function

The `GetAttendanceStatus()` function compares the student's attendance percentage with the minimum attendance threshold.

- If attendance is below 80%, it returns **"Needs attendance support"**.
- If attendance is 80% or above, it returns **"Attendance is good"**.

**Return type:** String

**Parameters:**
- `attendance` – Integer
- `MinAttendance` – Integer

## 9. Program Logic

The program follows these steps:

1. Start the program.
2. Ask the user to enter the student's name.
3. Request the student's attendance percentage.
4. Validate the attendance percentage.
5. If the percentage is outside the range of 0–100, request another entry.
6. Compare the valid attendance percentage with the 80% threshold.
7. Determine whether the student needs attendance support or has good attendance.
8. Display the student's name, attendance percentage, and attendance status.
9. Ask the user whether they want to check another student.
10. If the user enters YES, repeat the process.
11. If the user enters NO, end the program.

## 10. Expected Outputs and Test Scenarios

The following examples demonstrate how the system is expected to respond to different inputs.

| Student Name | Attendance | Expected Result |
|---|---:|---|
| John | 87% | Attendance is good |
| Mary | 65% | Needs attendance support |
| Peter | 80% | Attendance is good |
| Sarah | 45% | Needs attendance support |
| David | 100% | Attendance is good |

### Input Validation Tests

| Input | Expected Behaviour |
|---|---|
| 120 | Rejected because it is above 100. |
| -5 | Rejected because it is below 0. |
| 75 | Accepted as a valid attendance percentage. |
| 0 | Accepted as a valid attendance percentage. |
| 100 | Accepted as a valid attendance percentage. |

### Repeat and Exit Tests

| User Response | Expected Behaviour |
|---|---|
| YES | The program checks another student. |
| yes | The program checks another student. |
| NO | The program ends. |
| no | The program ends. |
| Maybe | The program displays an invalid-response message and requests another response. |

The program accepts the uppercase and lowercase forms shown above. Other mixed-case forms are not included in the current validation rules.

## 11. Validation Rules

The system uses validation to improve the accuracy of the information entered.

**Attendance validation:**
- Attendance must not be less than 0.
- Attendance must not be greater than 100.
- Invalid attendance values are rejected.
- The user is asked to enter the attendance percentage again until a valid value is provided.

**Repeat response validation:**
- YES or yes allows the user to check another student.
- NO or no ends the program.
- Any other response is treated as invalid and the user is asked again.

## 12. How to Run the Program

1. Download or locate the SASS Flowgorithm project file from the repository.
2. Open Flowgorithm on your computer.
3. Open the SASS `.fprg` file.
4. Review the flowchart if necessary.
5. Click the Run button to execute the program.
6. Enter the student's name when requested.
7. Enter the student's attendance percentage.
8. Follow the displayed instructions.
9. Enter YES to check another student or NO to end the program.

## 13. Repository Structure

The repository contains the project documentation and supporting assignment files.

The expected organisation is:

```text
PROG101_Assignment1_AnsuTucker_905006550/
│
├── README.md
├── Report(4).docx
├── Pseudocode.txt
├── SASS_Flowchart.png
└── SASS.fprg
```

**Note:** The filenames and folders shown above are an example. They should be adjusted to match the actual files uploaded to the GitHub repository.

## 14. Connection to Sustainable Development Goal 4

The Student Attendance Support System relates to **United Nations Sustainable Development Goal 4 (Quality Education)**.

SDG 4 focuses on ensuring inclusive and equitable quality education and promoting lifelong learning opportunities for all.

Regular attendance is important because students need opportunities to participate in lessons and learning activities. By identifying students whose attendance falls below the selected threshold, the system can help teachers recognise possible attendance concerns and consider appropriate support.

The project therefore demonstrates how a simple digital solution can contribute to efforts that support educational participation.

## 15. Open Source and Digital Public Goods

This project is shared through GitHub to demonstrate the use of open-source development practices and version control.

Making the project available in a repository allows other people to view its documentation, understand its logic, and learn from its design.

The system is a small educational project that demonstrates how programming can be used to address a practical school-related problem. It is not claimed to be an officially recognised or certified Digital Public Good.

## 16. Limitations and Privacy

Although the Student Attendance Support System provides basic attendance checking, it has some limitations:

- It checks one student's attendance at a time.
- It does not permanently store student information or attendance records.
- It does not connect to a school's official attendance database.
- It does not automatically send notifications to students, parents, or teachers.
- It does not generate monthly or yearly attendance reports.
- The 80% minimum attendance threshold is a design choice for this academic project and is not presented as an official national attendance policy.

The project uses sample information for demonstration. Real student personal information should not be uploaded to a public GitHub repository.

## 17. Conclusion

The Student Attendance Support System demonstrates how programming logic can be used to address a practical attendance-monitoring problem.

Through the use of functions, input validation, decision structures, and loops, the program checks students' attendance percentages and identifies those who may need attendance support.

The project also demonstrates the importance of modular programming, problem-solving, documentation, and version control when developing a simple software solution.
## 17. References

1. United Nations. (n.d.). *Goal 4: Ensure inclusive and equitable quality education and promote lifelong learning opportunities for all.*  
   https://sdgs.un.org/goals/goal4

2. Flowgorithm. (n.d.). *Flowgorithm – Flowchart programming language.*  
   http://www.flowgorithm.org/

3. GitHub. (n.d.). *GitHub documentation.*  
   https://docs.github.com/

4. United Nations Educational, Scientific and Cultural Organization (UNESCO). (n.d.). *Education.*  
   https://www.unesco.org/en/education
   Ministry of Basic and Senior Secondary Education(MBSSE)

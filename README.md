# Student Attendance Support System (SASS)

## Project Overview
The Student Attendance Support System (SASS) is a simple program designed to help identify student whose monthly attendance is below the project's minimum attendance target of 80%.

The program asks for a student's name and monthly attendance percentage. It then checks the percentage and displays an appropriate message. The user can repeat the process for another learner.

## Problem Being Addressed
Low attendance can make it harder for Student to keep up with their studies. SASS provides a simple way to identify learners whose attendance may need attention so that support can be considered.

This project is a basic demonstration. It does not connect to a school database or automatically contact learners.

## How the Program Works
1. Start the program.
2. Enter the student's name.
3. Enter the student's monthly attendance percentage.
4. Check that the percentage is between 0 and 100.
5. If the percentage is below 80%, display **Needs attendance support**.
6. If the percentage is 80% or above, display **Attendance is good**.
7. Ask whether the user wants to check another student.
8. If the answer is yes, repeat the process. Otherwise, end the program.

## Attendance Rule
- Below 80%: **Needs attendance support**
- 80% or above: **Attendance is good**

The 80% threshold is the rule selected for this project. It is not presented as a universal or official attendance policy.

## Example
| Learner name | Monthly attendance | Result |
|---|---:|---|
| Mariama | 65% | Needs attendance support |
| Ibrahim | 80% | Attendance is good |
| Abdul | 92% | Attendance is good |

A value below 0% or above 100% should be rejected as invalid.

## Functional Modules
- The Student Attendance Support System (SASS) is organised into five logical modules. Each module is responsible for a particular task within the program. In my Flowgorithm design, these tasks are performed inside one main function called `Main`, rather than being created as separate functions.

### 1. Main Control Module
**Purpose:** Controls the overall operation of the system. It displays the welcome message, declares the required variables, sets the minimum attendance threshold to 80%, starts the repetition process and displays the goodbye message when the user finishes.

### 2. Input Module
**Purpose:** Collects the information required from the user. It asks for the student's name and monthly attendance percentage. It also receives the user's response when asked whether another student's attendance should be checked.

### 3. Validation Module
**Purpose:** Checks whether the attendance percentage entered by the user is valid. The system accepts values from 0 to 100. If the user enters a value below 0 or above 100, an error message is displayed and the user is asked to enter the percentage again.

### 4. Decision Module
**Purpose:** Compares the student's valid attendance percentage with the minimum attendance threshold of 80%. If the attendance is below 80%, the system displays **"Needs attendance support"**. If the attendance is 80% or above, it displays **"Attendance is good"**.

### 5. Output Module
**Purpose:** Displays the information and results produced by the system. It shows the student's name, attendance percentage and attendance status. It also displays the welcome, invalid-input and goodbye messages where necessary.

**Note:** These five modules describe the logical responsibilities of the program. They are not five separate programming functions; all operations are carried out within the original `Main` function.

These are the logical modules used to organize the solution. They should correspond to the actual functions or processes shown in the submitted design.

## Computational Thinking
- **Decomposition:** The problem is divided into smaller tasks such as collecting input, validating data, checking attendance, and displaying a result.
- **Pattern recognition:** The same attendance-checking steps are repeated for each learner.
- **Abstraction:** The program focuses on the learner's name and monthly attendance percentage.
- **Algorithm design:** The steps are arranged in a clear order, with decisions and repetition.

## Sustainable Development Goal
The project relates to **United Nations Sustainable Development Goal 4: Quality Education**. Identifying learners who may need attendance support can contribute to efforts to help learners participate in education.

## Open-Source Software and Digital Public Goods
This project can be shared publicly so that others can inspect, learn from, and improve its design. A project being publicly available does not automatically make it open-source; an appropriate open-source licence must be selected and included.

Digital Public Goods are resources that meet the relevant Digital Public Goods Standard. This student project discusses the idea of accessible digital resources but should not be described as an officially recognized Digital Public Good.

## Tools
- Flowgorithm: for designing and testing the algorithm and flowchart.
- GitHub: for storing and sharing the project files.
## Conclusion

The Student Attendance Support System (SASS) was developed to demonstrate how programming logic can be used to address student attendance challenges. The system collects student information, validates attendance percentages, and compares each student's attendance against the minimum threshold of 80%.

Students with attendance below 80% are identified as needing attendance support, while those with attendance of 80% or above are considered to have good attendance.

Through this project, I gained practical experience in using input, validation, conditional statements, loops, pseudocode, and flowcharts to develop a logical solution to a real-world educational problem.

Overall, this project demonstrates how a simple computer-based system can help identify students who may need additional attendance support.
## Suggested Repository Contents
- `README.md` — project description and instructions.
-Pseudcode.
- Flowchart image or PDF — exported diagram, if required.
- Assignment report — final report, if permitted by the course instructions.

## Scope and Limitations
- The program uses a manually entered learner name and attendance percentage.
- It processes one learner at a time.
- It does not store records permanently.
- It does not use a school database, calculate attendance from daily registers, or send notifications.
- The attendance threshold is fixed at 80% for this project.

## Author
- Student name: Ansu Tucker
- Student ID: 905006550
- Course: PROG101
- Institution: Limkokwing University of Creative Technology, Sierra Leone

## References

- United Nations. Sustainable Development Goal 4: Quality Education. https://sdgs.un.org/goals/goal4
- Open Source Initiative. The Open Source Definition. https://opensource.org/osd
- Digital Public Goods Alliance. Digital Public Goods Standard. https://digitalpublicgoods.net/standard/


# LAB02: Domain-Specific Modeling

## Overview
This school management system is designed to represent a university and the various entities within university classes. It provides a detailed composition of how university classes are structured, encompassing both students and lecturers.

## Features
- **University Representation**: The system models the structure of a university, highlighting the interaction between students and lecturers in various classes.
- **Students**: This feature represents students enrolled in different courses within a university class. Courses include Computer Science, Information Technology, and Engineering.
- **Lecturers**: Lecturers are responsible for teaching students. The system models the relationship where each lecturer can teach a specific course, while students may enroll in multiple courses.

## Model Design Diagram
![Picture1](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/68c02629-15ca-4080-a5af-6e2a0a14fb94)

## The Resulting Network Diagram
![Picture1](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/4ccef5cd-5e11-4e70-a863-841c49ee5d3d)

## Text Generation Results
![Picture1](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/3fe78566-7a91-4af2-ad39-19c31735cb27)

## Task 4: Plugin Building and Testing
![Picture1](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/d2b20b4b-bce2-4cb5-8664-0892ec173642)
![Picture1](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/88cc9de2-a89b-468c-baf6-18d32f125fdd)


### Plugin Testing
**Error Encountered**: In the fourth task of the project, an error was encountered related to the DSL.UI folder. Despite successful completion of the first three tasks, this issue arose during plugin export and testing. The linked documentation provided insufficient instructions for resolving this issue, leading to challenges in accurately addressing the problem.
![Picture1](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/26a5bdcd-ac94-4ff9-9796-76d27589dbe4)

## Challenges and Problem-Solving

### Impact on Project Delivery
The cumulative effect of the compatibility issues with Java updates and the Java distribution misstep had a significant impact on project timelines. These technical challenges, coupled with the time spent troubleshooting, meant that I fell behind schedule. Consequently, I had to scale back my ambitions for the project and focus on delivering a simpler version within the remaining time. This experience, while frustrating, has underscored the importance of factoring in potential setbacks when planning project milestones.

### Compatibility Issue with Java Update
![WechatIMG317](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/12f9a07d-aa83-45cd-b527-05fd14bc80d7)

After updating my Mac's Java to version 21.0.1, I encountered a compatibility problem with the RM2PT tool, which requires Java 17. The newer Java version caused an error indicating that the JVM shared library lacked the `JNI_CreateJavaVM` symbol, essential for the RM2PT tool's operation.

### Java Distribution Misstep
<img width="336" alt="Screenshot 2023-11-12 at 10 21 54 PM" src="https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/ea022303-5782-4172-aa04-47c0dbbdad51">

In an effort to correct the compatibility issue, I removed the JDK from my environment and installed Java version 17. However, I mistakenly downloaded the Oracle version of Java instead of the Eclipse Adoptium version required by the RM2PT tool. This oversight added to the delays, as I had to locate, download, and install the correct version of Java.

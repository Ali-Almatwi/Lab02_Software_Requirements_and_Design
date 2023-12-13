# LAB02: Domain-Specific Modeling

## Overview
In this laboratory, I attempted to simulate various models, yet none were completed successfully. The initial model was a university management system, while the second was a vehicle. Each model was crafted to mirror real-life scenarios, focusing on the diverse entities within the models' classes. This approach offers a comprehensive view of the classes' structure, detailing how This approach offers a comprehensive view of the classes' structure, detailing how different components interact and integrate within each model. The university management system, for instance, includes modules for student registration, course management, and faculty administration, highlighting the intricate relationships and processes within an educational institution. On the other hand, the vehicle model delves into the mechanical and operational aspects, encompassing elements like engine performance, safety features, and user interface. Both models, though incomplete, aimed to provide an in-depth understanding of their respective systems, offering insights into the complexities and dynamics of real-world applications.

## Model 1 ( University )
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


## Model 2 ( Vehicle )

## Features 

#  Vehicle 16 Classes
- **Vehicle Model**: The foundational class capturing the name and specifications of the vehicle.
- **Means of Transportation**: Encapsulates the vehicle's entire functionality and purpose as a mode of transportation.
- **Drive**: A pivotal class showing the mechanisms responsible for propelling the vehicle forward, representing the type of fuel used.
- **Lounge Area**: Signifies the designated space within the vehicle devoted to comfort and relaxation for passengers.
- **Chassis**: The structural backbone providing support and housing critical components, defining the vehicle's structural integrity.
- **Wheel**: Essential for mobility, facilitating the vehicle's movement with various design elements for optimal performance.
- **Brake**: Ensuring safety and control, this class represents the braking system, a pivotal component in every vehicle.
- **Support Element**: The support structure encompassing various elements crucial for stability and functionality.
- **Luggage Range**: Designed for storage and cargo, this class represents the designated area for luggage and additional items.
- **Window**: Transparent elements allowing visibility, ventilation, and aesthetic appeal, forming a crucial part of the vehicle's exterior. The number of windows determines the vehicle type.
- **Door**: Entry and exit points representing the access mechanisms for passengers. The number of doors determines the vehicle type.
- **Control Element**: Encompassing various controls such as steering, pedals, and switches, facilitating interaction between the driver and the vehicle.
- **Person**: This class represents occupants, emphasizing the human aspect of vehicular transportation.
- **Power Transmission**: Crucial for converting and transmitting power from the engine to the wheels, ensuring dynamic motion.
- **Information Facility**: Enabling connectivity and information dissemination within the vehicle, embracing modern technological features.
- **Seat**: Providing comfort and ergonomic support, this class represents the seating arrangement for passengers.

## Target DSL EMF Metamodel
- Creation of vehicle classes showing parts of a vehicle including its model, chassis type, and 16 other classes.

<img width="468" alt="image" src="https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/29de8e1f-cd2d-4dc9-8d40-5b373b397623">


## Target DSL Eclipse Sirius Graphical Modeling

I created nodes and edges  for the following classes in this step


<img width="357" alt="image" src="https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/1e6f35c7-7d58-40b6-85ae-06664fee493c">

When generating the network diagram, the classes apart from the means of transportation could not appear until I changed the node types definition into bordered nodes, which means having the chassis node, for example, somehow inside the means of transportation node and others under them as the hierarchy appears in the diagram above. This was the resulting diagram after definition of nodes and edges. The edges did not show up at all in the diagram. Defining the create node worked perfectly.

<img width="425" alt="image" src="https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/73a08e66-871d-4581-a520-a44141fcf92b">

## Targeted DSL Eclipse Xtext Modeling
- Issues encountered with generating Xtext using the RM2PT developer option.

<img width="394" alt="image" src="https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/213f36cd-d0fb-4996-a41f-d260f9721a5f">


## Target DSL Test

Since I could not generate the Xtext in the step above, there was no way to run this step successfully. While I tried several other alternatives with many classes and features, many classes were not appearing after defining them in nodes and adding their edges. This seems to be mostly related to the kind of relationships that are chosen for the model either supertype, reference or composition relationships. Only a combination of supertype, reference and composition relationships that seem to work perfectly and have all the nodes together with connecting edges show in the final diagram.


## Challenges and Problem-Solving

### Impact on Project Delivery
The cumulative effect of the compatibility issues with Java updates and the Java distribution misstep had a significant impact on project timelines. These technical challenges, coupled with the time spent troubleshooting, meant that I fell behind schedule. Consequently, I had to scale back my ambitions for the project and focus on delivering a simpler version within the remaining time. This experience, while frustrating, has underscored the importance of factoring in potential setbacks when planning project milestones.

### Compatibility Issue with Java Update
![WechatIMG317](https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/12f9a07d-aa83-45cd-b527-05fd14bc80d7)

After updating my Mac's Java to version 21.0.1, I encountered a compatibility problem with the RM2PT tool, which requires Java 17. The newer Java version caused an error indicating that the JVM shared library lacked the `JNI_CreateJavaVM` symbol, essential for the RM2PT tool's operation.

### Java Distribution Misstep
<img width="336" alt="Screenshot 2023-11-12 at 10 21 54 PM" src="https://github.com/Ali-Almatwi/Lab02_Software_Requirements_and_Design/assets/148684334/ea022303-5782-4172-aa04-47c0dbbdad51">

In an effort to correct the compatibility issue, I removed the JDK from my environment and installed Java version 17. However, I mistakenly downloaded the Oracle version of Java instead of the Eclipse Adoptium version required by the RM2PT tool. This oversight added to the delays, as I had to locate, download, and install the correct version of Java.

# Elevator_Project 
![image](https://images.unsplash.com/photo-1624342057927-64d60f69b94d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1932&q=80)

# Project Title <img src="https://cdn-icons-png.flaticon.com/512/2800/2800015.png" width="60" height="60">


EFFICIENT USAGE OF ELEVATORS DURING PEAK HOURS IN CHRIST UNIVERSITY

# Inspiration <img src="https://user-images.githubusercontent.com/72274851/222214323-923a3fe7-56e9-4ba0-abff-162681500702.png" width="60" height="60">

The students always tend to have the issue of figuring out which elevator to use to reach their class floor at the peak hours. But to choose the optimal elevator could be worrisome and time consuming. But with the use of this AI/ML model that can figure out which elevator to take to reach the desired floor in a fastest and an optimal way. 

# What it does  <img src="https://user-images.githubusercontent.com/72274851/222216353-58874ba5-d9cc-4298-baab-4255bbdb0193.png" width="60" height="60"> 

This project aims to optimise elevator traffic in a university or college setting, with the goal of improving the experience for students. The problem addressed is the issue of elevators becoming overcrowded, leading to long wait times and a frustrating experience for students. By using machine learning and artificial intelligence techniques, we propose to develop a system that can predict elevator usage patterns. The proposed system has the potential to greatly improve the student experience in university or college buildings by reducing wait times and improving elevator traffic flow.

This model takes the queue quantity and your desired floor as input where  queue quantity is taken from the cameras which is using AI and ML tools to find the number of people standing in the queue as head counts and then the floor number is given by the users as per the floor they need to reach, with that we have formulated a logic to find out the average time every elevator is going to take to reach that particular floor and the elevator taking the least time to reach the desired floor is the output.	


# How we made it <img src="https://user-images.githubusercontent.com/72274851/222215141-6ced575e-414b-4088-bd99-d78921f80f66.png" width="60" height="60"> 


✅ Data was collected for the time taken by each elevator to reach a particular floor for all floors in different scenarios.

✅ The data was collected with diverse circumstances such like when the elevator has a long queue in the morning or people rushing in after the lunch hour .

✅ Average timings were noted and calculated for each elevator to complete one cycle to reach back to the starting floor.

✅ The data was then processed to find average time taken by each elevator to reach a certain floor for all floors.

✅ Along with the average timings of each elevator we consider the queue size in front of each elevator and average capacity of a elevator to calculate which elevator is the most efficient to reach a certain floor. 

✅ The model takes the queue quantity in front of each elevator and the destination floor as the input and provides the elevator option to take, which is calculated with a formulae.

✅ We have used video frame processing to take the count of people in the queue.

✅ Optimized the execution using intel oneAPI

# Conditions Followed for Recording Data <img src="https://camo.githubusercontent.com/012932956a1c252e20a2e296e01ef7463b9d9d33cd00f6a33d77ad88c18c646c/68747470733a2f2f636f6e646974696f6e2d616c7068612e636f6d2f736f6674776172652f696d616765732f676974757365722e706e67" width="60" height="60"> 

🤺 In total there are 'six' elevators available in the central block of "Christ University". Abiding by the rules for the elevator, "elevator A and B" start from "floor 0", "elevator C and D" start from "floor -1", and "elevator E and F" start from "floor 0".

🤺 Elevator A,B,C and D, all have have a limit of '9' floors. Elevator E and F have a limit of '10' floors.

🤺 Elevator A and C are limited to visit only the even floors i.e. 2, 4, 6 and 8. Elevator B and C are limited to visit only the odd floors i.e. 1, 3, 5, 7. Elevator E and F visit all the floors. All the elevators visit the 9th floor.

🤺 Elevator E and F have higher capacity than all the elevators.

🤺 All the elevators at least have to visit the 1st floor in accordance with their rules.

🤺 The queue quantity was recorded by counting the number of people standing in front of the person recording the data. As we had an average timing taken by each elevator for completing one cycle, it was assured that while recording the data, queue quantity was always less than the elevator capacity.

🤺 Every time the data was recorded when the elevator started from its designated starting floor.


# Logical Implementation <img src="https://repository-images.githubusercontent.com/273951747/c2380780-b3f6-11ea-99c3-21c2dcc9ba2c" width="60" height="60"> 

🔧 Number of people standing in queue in front of each elevator is taken as first set of input and then the target floor is used as second input.

🔧 Based on the data in dataset, average time of each elevator to reach the target floor is calculated by finding the mean of timings where the floor was the target floor.

🔧 Based on the elevator capacity of each particular elevator in different circumstances, average capacity of each elevator is calculated.

🔧 Based on different circumstances (like stopping on different floors) average time taken for an elevator to complete one cycle i.e. time taken by the elevator to start from the elevator's starting floor and reaching back to the same floor, is calculated.

🔧 If the queue size for a particular elevator is more than the average capacity of a elevator, the average time taken by an elevator to reach a particular floor is added to the average tome for the elevator to complete one elevator cycle.

🔧 The average timings of the designated elevators for the particular floor is then compared and the elevator with the least timing is selected and told to be as the preferred elevator.


# Dependencies <img src="https://user-images.githubusercontent.com/72274851/222215296-64d3a566-02c2-4ff9-9b8f-9ec5096f5799.png" width="60" height="60"> 


This project requires the following dependencies:

✅ Python 3.7 or higher

✅ Pandas

✅ Cetroidtracker.py

✅ Config.py

✅ Mailer.py

✅ Thread.py

✅Trackableobject.py





# How to Install and Run the Project <img src="https://user-images.githubusercontent.com/72274851/222215440-158ffdc1-8a23-4c7f-81c2-44e864d6d043.png" width="60" height="60"> 
To run the project, follow these steps:

To run the project, follow these steps:

✅ Clone this repository to your local machine.

✅ Install the dependencies listed above.

✅ Open a terminal and navigate to the project directory.

✅ Run the elevator_count.ipynb Jupyter notebook count the number of people standing in the queue in front of the elevator .

✅ Now run elevator_calculation to  find the most efficient elevator that will take the least time to reach the perticular floor .


# Usage <img src="https://user-images.githubusercontent.com/72274851/222215440-158ffdc1-8a23-4c7f-81c2-44e864d6d043.png" width="60" height="60"> 
To run the project, follow these steps:

The user has to enter the floor he/she has to reach and it will show the most efficient elevator and least time taking elevator to reach that floor .

Please Note:Sometimes there can be an error while using jupyter notebook therefore a file named "Run.py" is attached so that the project can be executed through the same.








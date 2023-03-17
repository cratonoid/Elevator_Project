# Elevator_Project 
![image](https://images.unsplash.com/photo-1624342057927-64d60f69b94d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1932&q=80)

# Project Title <img src="https://cdn-icons-png.flaticon.com/512/2800/2800015.png" width="60" height="60">


Analysis of the most efficient elevator in Christ at the peak hours .

# Inspiration <img src="https://user-images.githubusercontent.com/72274851/222214323-923a3fe7-56e9-4ba0-abff-162681500702.png" width="60" height="60">

The students always tend to have the issue of figuring out which lift to use to reach their class floor at the peak hours. But to choose the optimal elevator could be worrisome and time consuming. But with the use of this AI/ML model that can figure out which lift to take to reach the desired floor in a fastest and an optimal way. 

# What it does  <img src="https://user-images.githubusercontent.com/72274851/222216353-58874ba5-d9cc-4298-baab-4255bbdb0193.png" width="60" height="60"> 

This project aims to optimise elevator traffic in a university or college setting, with the goal of improving the experience for students. The problem addressed is the issue of elevators becoming overcrowded, leading to long wait times and a frustrating experience for students. By using machine learning and artificial intelligence techniques, we propose to develop a system that can predict elevator usage patterns. The proposed system has the potential to greatly improve the student experience in university or college buildings by reducing wait times and improving elevator traffic flow.

This model takes the queue quantity and your desired floor as input where  queue quantity is taken from the cameras which is using AI and ML tools to find the number of people standing in the queue  as head counts and then the floor number is given by the users as per the floor they need to reach,with that we have formulated a logic to find out the time every lift is going to take to reach that particular floor and the lift taking the least time to reach the desired floor is the output .`	


# How we made it <img src="https://user-images.githubusercontent.com/72274851/222215141-6ced575e-414b-4088-bd99-d78921f80f66.png" width="60" height="60"> 


✅ Collected data of the time taken by each lift to reach each floor in different scenarios

✅ We collected datas of each elevator going to all the different floors in different circumstances like when the lift has a long queue in the morning or people rushing in after the lunch hour .

✅ Also took different readings for each elevator to complete one cycle in all different situations.

✅ Then processed the data to find average time taken by the lifts to reach each certain floors and also the average time taken to complete one cycle .

✅ Along with the average timings of each lift we consider the queue size in front of each elevator and average capacity of a lift to calculate which elevator is the     most efficient to reach a certain floor. 

✅ The model takes the queue quantity in front of each elevator and the destination floor as the input and provides the elevator option to take, which is calculated       based on the above formulae.

✅ We have used queue image processing to take the count of people in the queue.

✅ Train and Test the model using intel oneAPI


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

The user has to enter the floor he/she has to reach and it will show the most efficient lift and least time taking lift to reach that floor .
Please Note:Sometimes there can be an error while using jupyter notebook therefore a file named "Run.py" is attached so that the project can be executed through the same.








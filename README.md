# UAV Task Assignment and Visualization

This application enables users to assign tasks to UAVs using a genetic algorithm and visualize the flight paths. The app is built with Streamlit and allows task assignment based on specific constraints and parameters.

## Prerequisites
- Python 3.x
- Random 
- matplotlib (Required for plot)
- Pandas (Required for upload excel)
- [Streamlit](https://streamlit.io/)
- [ImageMagick](https://imagemagick.org/) (Required for save gif)
  
## Two ways to manipulate the app
### Just click the link :
### OR Open it from your comand propmpt (cmd) so you can adjust the webpage and code simultaneously
- pip install streamlit if you do not have
- Then use cd/d turn to the location of the file. Run `streamlit run app.py` and open the app in your browser.

## Usage  
1. **Input**
   1.1 ** Configure Tasks and UAVs**
       Use the `Task number` and `UAV number` input fields to adjust the Number of Tasks and Number of UAVs to match the requirements of your assignment scenario.
       For task, optionally, could upload an Excel file with task data to automatically populate the task table.
       In our example you could upload the `task_and_plan.xlsx` for task. And For UAV you could put into 6 into sidebars. 
   1.2 **Input Task Details**:
       For each task, specify the Location X, Location Y, Type, Duration, and Deadline in the Task Inputs panel.
       For each UAV, specify the Location X, Location Y, Type, Speed in the UAV Inputs panel.
       Task inputs can be manually adjusted or derived from the uploaded file.
       In the example when you upload the `task_and_plan.xlsx`,task details will be changed automatically. And we suggest you put into these infos:
       UAV1 speed 45 Type X; UAV2 speed 50 Type Y; UAV3 speed 55 Type Z; UAV4 speed 45 Type X; UAV5 speed 50 Type Y; UAV6 speed 55 Type Z;
       And their location X and Y is zero.
2.**Run Algorithm**
   Just click the button `Run Algorithm` in the sidebar.
3.**Out Put**
   3.1 **Best Solution Task Allocation**
       Displays the optimism task assignment to each UAV.
   3.2 ** Fitness History Chart**
       The line chart displays the fitness progression over the algorithm’s iterations.
       A higher fitness value indicates a more efficient task allocation.
   3.3 ** UAV Task Assignment and Paths Visualization**
       You could see a gif of each UAV assignment that you can get a macro understanding of the overall UAVs trajectory.
   3.4 **UAV Data and Inputs**
       You can see the current coordinates of the UAVs, and you can continue to assign tasks based on that. 


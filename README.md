# UAV Task Assignment and Visualization

This application enables users to assign tasks to UAVs using a genetic algorithm and visualize the flight paths. The app is built with Streamlit and allows task assignment based on specific constraints and parameters.

## Prerequisites
- Python 3.x
- Random 
- matplotlib (Required for plot)
- Pandas (Required for upload excel)
- [Streamlit](https://streamlit.io/)
- [ImageMagick](https://imagemagick.org/) (Required for save gif)
  
## Two Ways to Manipulate the App
1. **Click the Link**: Access the app directly by following the link.
2. **Open it from Command Prompt (cmd)**: This method allows you to adjust the webpage and code simultaneously.
   - Run `pip install streamlit` if you do not have it installed.
   - Navigate to the location of the file using `cd` or `cd/d`, then run:
     ```bash
     streamlit run app.py
     ```
   - Open the app in your browser.

## Usage  

### 1. **Input**
#### 1.1 **Configure Tasks and UAVs**
- Use the `Task number` and `UAV number` input fields to adjust the number of tasks and UAVs to fit your assignment scenario.
- For tasks, you can optionally upload an Excel file with task data to populate the task table automatically.
- For example, you could upload `task_and_plan.xlsx` for tasks. In the sidebar, enter `6` for UAVs.

#### 1.2 **Input Task Details**
- For each task, specify the following in the **Task Inputs** panel:
  - **Location X** and **Location Y**
  - **Type**
  - **Duration**
  - **Deadline**
- For each UAV, specify the following in the **UAV Inputs** panel:
  - **Location X** and **Location Y**
  - **Type**
  - **Speed**

  *Note*: Task inputs can be manually adjusted or derived from the uploaded file. In the example, uploading `task_and_plan.xlsx` will automatically update task details. Suggested UAV settings:
  - UAV1: Speed 45, Type X
  - UAV2: Speed 50, Type Y
  - UAV3: Speed 55, Type Z
  - UAV4: Speed 45, Type X
  - UAV5: Speed 50, Type Y
  - UAV6: Speed 55, Type Z
  - Set the Location X and Y for all UAVs to zero.

### 2. **Run Algorithm**
   - Click the `Run Algorithm` button in the sidebar.

### 3. **Output**
#### 3.1 **Best Solution Task Allocation**
   - Displays the optimal task assignment to each UAV.

#### 3.2 **Fitness History Chart**
   - A line chart shows the fitness progression over the algorithm’s iterations.
   - Higher fitness values indicate a more efficient task allocation.

#### 3.3 **UAV Task Assignment and Paths Visualization**
   - View a GIF of each UAV assignment to get a macro view of the overall UAVs' trajectories.

#### 3.4 **UAV Data and Inputs**
   - Shows the current coordinates of the UAVs.
   - You can continue to assign tasks based on these updated coordinates.


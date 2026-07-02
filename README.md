# Client_Server-Development
Interactive Dashboard using MongoDB, Python, and Dash

## Grazioso Salvare Dashboard – README

### Overview

This project is a web-based interactive dashboard developed for Grazioso Salvare, an organization that identifies and trains rescue dogs for life-saving operations. The application allows users to filter and analyze animal shelter data from the Austin Animal Center dataset to identify dogs suitable for different types of rescue training. The dashboard provides an intuitive interface that enables users to explore data without needing technical knowledge of databases or query languages.

### Functionality
The dashboard allows users to filter animals based on rescue type:
- Water Rescue
- Mountain or Wilderness Rescue
- Disaster or Individual Tracking
- Reset
When a filter is selected, the dashboard dynamically updates the data table with filtered results, updates the pie chart to display the breed distribution corresponding with the filtered data, and update the geolocation map displaying selected animal locations. This ensures users can quickly identify suitable dogs based on breed, age, and sex criteria defined by Grazioso Salvare.

### Screenshots
The following screenshots demonstrate full functionality of the dashboard:
1.	Default dashboard view
2.	Water Rescue filter applied 
3.	Mountain/Wilderness Rescue filter applied 
4.	Disaster/Individual Tracking filter applied 
5.	Reset view showing all data

**Main Dashboard**
<img width="1207" height="606" alt="image" src="https://github.com/user-attachments/assets/9dd33b66-d0c8-4bc6-80e7-2c74e072b932" />
<img width="1080" height="377" alt="image" src="https://github.com/user-attachments/assets/469bc8fb-83d2-46ec-899d-a9b1af265b7a" />

**Mountain/Wilderness**
<img width="975" height="441" alt="image" src="https://github.com/user-attachments/assets/36c1a1ba-1a60-4286-acc7-3263f7211a26" />
<img width="975" height="368" alt="image" src="https://github.com/user-attachments/assets/2c3e09fa-8ebc-4dac-8a9d-20376264c3f2" />

**Disaster Rescue**
<img width="975" height="439" alt="image" src="https://github.com/user-attachments/assets/02667e5c-603f-4527-8278-bd4d5d430ebe" />
<img width="975" height="367" alt="image" src="https://github.com/user-attachments/assets/2dd212bc-6dab-4ad4-8b7b-258cf0888112" />

**Main Dashboard (Reset View)**
<img width="975" height="442" alt="image" src="https://github.com/user-attachments/assets/2b674861-dddc-4f99-ab2a-590511f31da3" />
<img width="975" height="370" alt="image" src="https://github.com/user-attachments/assets/f02ca0b4-e472-4b6c-91e9-12c5e3f1bfe0" />

### Tools and Technologies Used
### MongoDB
MongoDB was used as the database system because it is a NoSQL database that stores data in flexible document format. This makes it well-suited for handling varying animal record fields and allows efficient querying through Python. It also integrates easily with the CRUD module used in this project.

### Python
Python was used to implement backend logic, data manipulation, and database interaction. A custom CRUD module was used to perform create, read, update, and delete operations on the MongoDB database.

### Dash Framework
Dash was used to build the interactive web dashboard. It allows Python developers to create web applications with interactive components such as buttons, tables, and graphs without needing JavaScript. Dash callbacks were used to connect user input to dynamic updates in the dashboard.

### Plotly
Plotly Express was used to generate visualizations, specifically a pie chart showing the distribution of dog breeds based on the selected filter.

### Dash Leaflet
Dash Leaflet was used to display animal location data on an interactive map using latitude and longitude coordinates from the dataset.


### Project Development Steps
1.	Imported and cleaned the Austin Animal Center dataset into MongoDB. 
2.	Created a reusable CRUD Python module to connect Python with MongoDB. 
3.	Built a Dash application layout including a data table, filters, chart, and map. 
4.	Implemented interactive radio button filters for rescue categories. 
5.	Developed MongoDB queries to filter data by breed, sex, and age range. 
6.	Connected filters to dashboard components using Dash callbacks. 
7.	Added visual components including a pie chart and geolocation map. 
8.	Tested each filter to ensure proper updates across all dashboard components. 
9.	Captured screenshots demonstrating full functionality. 

### How to Run the Project
1.	Ensure MongoDB is installed and running locally. 
2.	Load the Austin Animal Center dataset into the aac database. 
3.	Install required Python packages:
   ``` pip install dash jupyter-dash dash-leaflet pandas plotly ```
4.	Update database credentials in the code:
  ```
Python:
  username = "yourusername"
  password = "yourpassword"
  HOST = 'localhost' 
  PORT = 27017 
  DB = 'yourdb' 
  COL = 'yourcol'
```
5.	Run the Jupyter Notebook: ProjectTwoDashboard.ipynb
6.	Open the dashboard in the browser and interact with the filters. 


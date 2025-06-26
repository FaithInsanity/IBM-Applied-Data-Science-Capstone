# IBM-Applied-Data-Science-Capstone
SpaceX Launch Success Dashboard

Overview

This repository contains the IBM Applied Data Science Capstone Project, which develops an interactive dashboard to visualize SpaceX launch data. The dashboard, built using Python, Dash, and Plotly, allows users to explore launch success rates and payload correlations across different launch sites. The project demonstrates skills in data processing, visualization, and web application development.

Features





Launch Site Selection: A dropdown menu to select specific SpaceX launch sites or view data for all sites.



Success Rate Pie Chart: Displays the total successful launches for all sites or success vs. failure counts for a selected site.



Payload Range Slider: Filters data by payload mass (in kilograms) to analyze specific payload ranges.



Payload-Success Scatter Chart: Visualizes the correlation between payload mass and launch success, with color-coded booster versions.

Repository Contents





spacex-dash-app.py: The main Python script for the Dash application.



spacex_launch_dash.csv: The dataset containing SpaceX launch records (must be in the same directory as the script).



Final_Presentation_Capstone.pdf: The presentation summarizing the project, methodology, and insights.



Jupyter notebooks (if applicable): Additional analysis or preprocessing steps (update with specific notebook names if included).

Prerequisites





Python 3.11 or later



Required Python libraries:

pip install pandas dash plotly



The spacex_launch_dash.csv dataset, which includes columns: Launch Site, Payload Mass (kg), class, and Booster Version Category.

Installation





Clone the repository:

git clone https://github.com/FaithInsanity/IBM-Applied-Data-Science-Capstone.git
cd IBM-Applied-Data-Science-Capstone



Install dependencies:

pip install -r requirements.txt

Or manually install:

pip install pandas dash plotly



Ensure spacex_launch_dash.csv is in the project directory.

Running the Dashboard





Navigate to the project directory:

cd IBM-Applied-Data-Science-Capstone



Run the Dash app:

python3.11 spacex-dash-app.py



Open a web browser and go to http://127.0.0.1:8050 to view the dashboard.

Dataset

The spacex_launch_dash.csv dataset contains SpaceX launch records with the following key columns:





Launch Site: The launch site (e.g., CCAFS LC-40, VAFB SLC-4E).



Payload Mass (kg): The payload mass in kilograms.



class: Launch outcome (1 = Success, 0 = Failure).



Booster Version Category: The category of the booster used.

Project Structure





Data Processing: Uses pandas to load and filter the dataset based on user inputs.



Visualization: Plotly Express creates interactive pie and scatter charts.



Web App: Dash powers the interactive dashboard with a responsive layout.



Presentation: The Final_Presentation_Capstone.pdf file summarizes the project, including methodology, results, and insights.

Usage





Select a launch site from the dropdown to filter data or choose "All Sites" for an overview.



Use the payload range slider to filter launches by payload mass.



View the pie chart for success rates and the scatter chart for payload-success correlations.

Notes





Ensure the CSV file is in the project directory, or update the file path in spacex-dash-app.py if needed.



If port 8050 is in use, modify the port in app.run(port=8050) to another value (e.g., 8051).



The dashboard assumes the dataset has the required columns. Verify the CSV structure if errors occur.

Acknowledgments

This project was completed as part of the IBM Applied Data Science Capstone on Coursera. The dataset is sourced from publicly available SpaceX launch records.

License

This project is licensed under the MIT License. See the LICENSE file for details.

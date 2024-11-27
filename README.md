# Data_Cleaning_Assignment2
Here’s a **README file** that provides an overview of the dataset, the steps you took to clean it, and how to use it in Tableau for analysis:

---

# **Factory Survey Feedback - README**

## **Overview**
This dataset contains feedback collected from workers in a factory, where each worker provides multiple responses within a **5-minute maximum time frame**. The feedback focuses on various aspects of the factory environment, worker conditions, and worker rights. The dataset consists of multiple queries (questions) and responses, capturing the worker's experiences and satisfaction.

### **Dataset Structure**
- **Queries (Query 1 - Query 14)**: These columns represent the questions asked to the workers, covering topics such as working hours, availability to join unions, and worker welfare.
- **Responses (Response 1 - Response 14)**: These columns contain the workers' answers to the respective queries.
- **Worker ID**: A unique identifier for each worker participating in the survey.
- **Date/Time**: Timestamp of when the feedback was collected.
- **Duration**: The time spent by the worker while providing feedback (in minutes).

### **Key Features**
- Each worker can provide **multiple feedback responses** across different sessions, ensuring that data reflects diverse experiences.
- **Time Constraints**: Feedback sessions are restricted to a **5-minute maximum** to ensure consistency in data collection.
- The dataset has been **cleaned and transformed** to ensure consistency and correctness.

## **Data Cleaning & Transformation**
1. **Removal of Invalid Data**: Rows with invalid or missing **worker ID** or entries with a `0` value in the ID field were removed.
2. **Null Value Handling**: 
   - `NULL` values were replaced with default values like `"N/A"` in specific columns when needed.
   - Data synchronization ensured that empty values in one field (e.g., Query 3) were reflected in the corresponding fields (e.g., Response 3).
3. **Data Splitting & Merging**:
   - **Query 8** and **Query 9** were split into two distinct queries to maintain clarity and accuracy in analysis.
   - **Query 14** and **Response 14** were created by merging relevant queries and responses from **Query 8** and **Query 9**, consolidating answers into a single column.
4. **Text Clean-up**: Specific strings were replaced or trimmed to standardize responses and improve consistency (e.g., fixing "press '1'" to "Press '1'").

## **How to Use This Dataset**
1. **Load the Data**: Import the dataset into Tableau or any other tool for analysis.
2. **Create Visualizations**: Use the cleaned fields to create interactive visualizations in Tableau, such as bar charts, line graphs, and heatmaps.
3. **Analyze Worker Feedback**: Identify trends and insights regarding worker satisfaction, working hours, and the availability of unions or welfare committees.

## **Notes**
- The data is structured for ease of analysis, with separate columns for each query and response.
- The dataset is ready for analysis, with clean and well-organized data fields.
- This data can help identify key trends in worker experiences and factory conditions, enabling actionable insights for improving the factory environment.

---

Let me know if you need any further modifications to the README file!

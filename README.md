# Workshop 01: ETL Process

## Objective

This workshop demonstrates the **Extract, Transform, Load (ETL)** process using a dataset of job candidates. The goal is to extract data, transform it for analysis, and load it into a database for visualization.

## Dataset Overview

The dataset contains information about job candidates, including:

- **First Name**
- **Last Name**
- **Email**
- **Application Date**
- **Country**
- **Years of Experience (YoE)**
- **Seniority Level**
- **Technology Specialization**
- **Code Challenge Score**
- **Technical Interview Score**

## Tools and Environment

To run this workshop, you'll need:

- **Python**
- **Jupyter Notebook**
- **PostgreSQL**
- **Power BI**

## Setup Instructions

1. **Clone the Repository**

   Open your terminal and run:

   ```bash
   git clone https://github.com/Jakcobo/workshop_01.git
   #Go to root in workshop_01
   cd workshop_01
   ```

2. **Set Up a Virtual Environment**

   Create and activate a virtual environment:

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**

   Install the required:

   ```bash
   pip install -r requirements.txt
   pip install python
   pip install psycopg2
   ```

4. **Configure the Database Connection**

   In the `env/.env` file, set your PostgreSQL database credentials:

   ```python
    PG_HOST=localhost
    PG_PORT=5432
    PG_USER=your_user
    PG_PASSWORD=your_password
    PG_DATABASE=your_nameDATABASE
   ```

5. **Run the Jupyter Notebooks**

   Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

   Open and execute the notebooks in the following order:

   - `001_loadData.ipynb`: Loads the dataset into the PostgreSQL database.
   - `002_EDA.ipynb`: Performs Exploratory Data Analysis.
   - `003_cleanData.ipynb`: Cleans and transforms the data.

6. **Visualize Data in Power BI**


     - **Pie Chart**: Hires by technology.
     - **Bar Chart**: Hires by year.
     - **Bar Chart**: Hires by seniority.
     - **Line Chart**: Hires by country over years (focus on USA, Brazil, Colombia, and Ecuador).

## Conclusion

1. **Software Engineering and Automation & DevOps are the most in-demand fields.** These areas have the highest number of hires, indicating a focus on technical expertise.
2. **Hiring peaked in 2019 and 2020 but decreased in 2021 and 2022.** This may be due to economic constraints or a shift in hiring strategies.
3. **USA leads in hiring growth, while Ecuador has seen a decline.** This suggests a regional hiring preference or economic factors affecting hiring in certain countries.
4. **Interns, Juniors, and Trainees make up most of the hires.** This suggests a strategy focused on training and internal growth rather than hiring senior professionals.
5. **Only 13% of applicants are hired, showing a competitive selection process.** The high rejection rate indicates either a large applicant pool or a strict evaluation process.

By following this workshop, you will understand the ETL process and how to visualize data effectively using Power BI.

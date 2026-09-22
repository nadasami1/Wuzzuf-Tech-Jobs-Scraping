# Wuzzuf Tech Jobs Web Scraping

## 📌 Project Overview

This project uses **Selenium and Python** to scrape technology-related job opportunities from **Wuzzuf**, one of the popular job platforms in Egypt.

The project searches for different technology positions, collects important information about the available jobs, and stores the results in a CSV file for further analysis.

---

## 🎯 Project Objectives

The main objectives of this project are to:

* Automate job searching using Selenium.
* Collect job information from Wuzzuf.
* Search for multiple technology-related positions.
* Extract useful job details.
* Store the collected data in a structured CSV file.
* Prepare the data for further analysis and visualization.

---

## 🔎 Job Positions

The project searches for the following positions:

* Data Engineer
* Data Science
* AI Developer
* Machine Learning Engineer

---

## 📊 Data Collected

For each job, the following information is collected:

| Column       | Description                     |
| ------------ | ------------------------------- |
| `position`   | The position used in the search |
| `title`      | Job title                       |
| `company`    | Company offering the job        |
| `location`   | Job location                    |
| `job_type`   | Type of employment              |
| `experience` | Required years of experience    |
| `url`        | URL of the job posting          |

---

## 🛠️ Technologies Used

* **Python**
* **Selenium**
* **Pandas**
* **Chrome WebDriver**
* **Jupyter Notebook**

### Python Libraries

```python
selenium
pandas
time
```

---

## ⚙️ How the Project Works

The scraping process follows these steps:

### 1. Open Wuzzuf

Selenium opens the Wuzzuf jobs page.

### 2. Search for Job Positions

The program searches for each position from the predefined list:

```python
Positions = [
    "Data Engineer",
    "Data Science",
    "AI Developer",
    "Machine Learning Engineer"
]
```

### 3. Extract Job Information

For each job listing, the scraper extracts:

* Job title
* Company
* Location
* Job type
* Required experience
* Job URL

### 4. Navigate Through Job Pages

The scraper attempts to move to the next page and collect additional job listings.

### 5. Store the Data

All collected jobs are stored in a Pandas DataFrame:

```python
jobs_df = pd.DataFrame(all_jobs)
```

### 6. Export the Dataset

The final dataset is saved as a CSV file:

```python
jobs_df.to_csv(
    "SampleOfwazzuf_tech_jobs.csv",
    index=False,
    encoding="utf-8-sig"
)
```

---

## 📁 Project Structure

```text
Wuzzuf-Tech-Jobs-Scraping/
│
├── Wuzzuf_Jobs_Scraping.ipynb
│
├── SampleOfwazzuf_tech_jobs.csv
│
└── README.md
```

---

## 🚀 Installation

Make sure Python is installed on your computer.

Install the required libraries using:

```bash
pip install selenium pandas
```

You also need **Google Chrome** installed because the project uses Chrome WebDriver.

---

## ▶️ How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <(https://github.com/nadasami1/Wuzzuf-Tech-Jobs-Scraping)>
```

### Step 2: Open the Project

Open the project folder using **VS Code** or **Jupyter Notebook**.

### Step 3: Install Dependencies

```bash
pip install selenium pandas
```

### Step 4: Run the Notebook

Open:

```text
Wuzzuf_Jobs_Scraping.ipynb
```

and run the cells.

### Step 5: Get the Dataset

After the scraping process finishes, the collected data will be saved as:

```text
SampleOfwazzuf_tech_jobs.csv
```

---

## 📦 Output

The output is a CSV dataset containing the scraped technology job opportunities.

Example structure:

```text
position,title,company,location,job_type,experience,url
Data Engineer,Data Engineer,...,...,...,...,...
AI Developer,AI Developer,...,...,...,...,...
Machine Learning Engineer,ML Engineer,...,...,...,...,...
```

---

## 📈 Possible Future Improvements

This project can be extended by:

* Scraping more job pages.
* Adding more job positions.
* Collecting job posting dates.
* Collecting salary information when available.
* Extracting job descriptions.
* Removing duplicate job listings.
* Cleaning and preprocessing the scraped data.
* Performing exploratory data analysis (EDA).
* Creating visualizations using Matplotlib or Power BI.
* Analyzing the most requested skills in technology jobs.
* Analyzing job opportunities by location and experience level.

---

## ⚠️ Notes

The project depends on the current structure of the Wuzzuf website. If the website changes its HTML structure or CSS classes, some Selenium selectors may need to be updated.

The scraping process should also be used responsibly and in accordance with the website's terms and applicable policies.

---

## 👩‍💻 Author

**Nada Sami**

AI Student | Data Analysis & Machine Learning Enthusiast

### Skills Used in This Project

* Python
* Selenium
* Pandas
* Web Scraping
* Data Collection
* Data Preparation

---

## ⭐ Project Purpose

This project was developed as a practical application of **Python Web Scraping**, demonstrating how Selenium can be used to automate browser interaction, collect structured data, and prepare it for further analysis.

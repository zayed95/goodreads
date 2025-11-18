# 🍃 Goodreads Data Pipeline Project 

## 📖 Project Overview

In this project, I exported my own data from Goodreads to work on a personal project that allowed me to explore my reading patterns across the years using tools like Python and PowerBI.
---

## 🛠️ Steps in the Pipeline

### **1. Export Goodreads Data**

* Goodreads allows users to export their reading history in CSV format.
* This dataset typically includes information such as book title, author, rating, date read, and more.
* The exported CSV serves as the raw input for this project.

---

### **2. Clean the Data with Python**

Using Python (pandas), the dataset was processed to:

* Remove unnecessary columns
* Handle missing values
* Normalize book titles and author names
* Prepare the text fields for language model ingestion

This ensures that the data is structured and ready for enrichment.

---

### **3. Extract Language and Genre Using LangChain**

A LangChain pipeline was built to automatically infer:

* **Book language**
* **Book genre**

Using the title and author as model inputs, the pipeline:

1. Sends a prompt to a language model
2. Parses the model's output
3. Appends the extracted attributes as new columns in the dataframe

This adds valuable metadata that Goodreads does not provide by default.

---

### **4. Export the Enriched Data and Build a Power BI Dashboard**

The final dataframe was exported back to CSV.

A Power BI dashboard was then created to visualize:

* Reading patterns
* Genre distribution
* Language diversity
* Ratings and trends over time

This dashboard provides clear insights and an interactive way to explore reading habits.

---

## 📦 Tech Stack

* **Python** (pandas, LangChain)
* **Large Language Model** (via LangChain)
* **Power BI** (visualization)
* **Goodreads CSV Export**

---

## 🚀 How to Run the Project

1. **Export data from Goodreads** as CSV.
2. Place it in the `data/` folder.
3. Run the Python notebook or script to clean and enrich the data.
4. Export the enriched CSV.
5. Load the CSV into Power BI.
6. Build your dashboard visuals.

---

## 📊 Final Output

* A clean, enriched dataset of your reading history
* Automatically extracted genres and languages
* A full Power BI dashboard with interactive insights

---

##

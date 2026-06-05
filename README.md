# Autocomplete and Autocorrect Data Analytics

## Project Overview

This project explores the efficiency and accuracy of autocomplete and autocorrect algorithms using Natural Language Processing (NLP). Built as part of a remote internship project (Level 2 - Project 5), it analyzes real-world datasets to implement intelligent text prediction and spelling correction systems.

---

## Datasets Used

| Dataset | Description |
|--------|-------------|
| `menu.csv` | McDonald's menu items with categories and nutritional info |
| `retail_sales_dataset.csv` | Retail sales transactions with product categories, quantity, and amount |

---

## Technologies Used

- **Python** — Core programming language
- **Google Colab** — Cloud-based notebook environment
- **Pandas** — Data loading and manipulation
- **NLTK** — Natural Language Processing and text preprocessing
- **TextBlob** — Autocorrect implementation
- **Matplotlib** — Data visualization
- **Seaborn** — Advanced chart styling
- **Collections (Counter)** — Word frequency analysis

---

## Project Steps

### Step 1 — Data Collection and Upload
Uploaded both datasets into Google Colab using the files upload method and extracted them from zip archives.

### Step 2 — NLP Preprocessing
- Converted all text to lowercase
- Removed special characters, numbers, and symbols using regex
- Extracted item names and product categories from both datasets
- Combined into a single cleaned text corpus

### Step 3 — Autocomplete System
Built a word frequency based autocomplete engine using Python's Counter and a prefix matching algorithm. When a user types a prefix like "ch", the system suggests the most frequently occurring words starting with those letters — similar to how Google Search suggests queries.

### Step 4 — Autocorrect System
Implemented autocorrect using the TextBlob library which compares misspelled words against a built-in English dictionary and returns the closest correct word — similar to smartphone keyboard correction.

### Step 5 — Performance Metrics
Tested both systems with sample inputs and calculated correction accuracy as a percentage score.

### Step 6 — Algorithm Comparison
Compared prefix-based autocomplete suggestions across multiple test inputs to evaluate prediction relevance.

### Step 7 — Data Visualization
Generated two charts:
- **Top 15 Most Frequent Words** — Bar chart showing the most repeated words across both datasets
- **Total Sales by Product Category** — Bar chart comparing total revenue across Beauty, Clothing, and Electronics

---

## Key Results

- Autocomplete successfully predicted relevant words from dataset vocabulary
- Autocorrect accurately fixed common spelling errors like "brakfast" → "breakfast", "retial" → "retail"
- Clothing and Electronics had the highest total sales (~150,000 each)
- Most frequent words matched real-world product and food categories

---

## How to Run

1. Open [Google Colab](https://colab.research.google.com)
2. Create a new notebook
3. Upload `menu.csv` and `retail_sales_dataset.csv`
4. Run each cell in order
5. View autocomplete suggestions, autocorrect results, and graphs

---

## What I Learned

- How NLP preprocessing works in real projects
- How autocomplete is built using word frequency and prefix matching
- How autocorrect uses dictionary-based spell checking
- How to visualize text data using Python libraries
- How to work with real-world CSV datasets end to end

---

## Project Structure

```
autocomplete-autocorrect-analytics/
│
├── menu.csv                  # McDonald's menu dataset
├── retail_sales_dataset.csv  # Retail sales dataset
├── autocomplete_autocorrect.ipynb  # Main Colab notebook
└── README.md                 # Project documentation
```

---

## Author

**Anandhu A Unnithan**  
BTech Student | Remote Intern  
Project 5 — Level 2 | Data Analytics

---

## Acknowledgements

- Dataset sourced from Kaggle
- Project assigned as part of remote internship program
- Built and tested on Google Colab


# Netflix Dataset Analysis

![Netflix Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/0/08/Netflix_2015_logo.svg/2560px-Netflix_2015_logo.svg.png)

## 📊 Project Overview

A comprehensive **Exploratory Data Analysis (EDA)** project that delves into Netflix's extensive content library. This analysis provides valuable insights into Netflix's content strategy, distribution patterns, and catalog composition using Python's powerful data analysis toolkit.

## 🎯 Key Objectives

- **Data Quality Assessment**: Identify and handle data inconsistencies, missing values, and duplicates
- **Content Analysis**: Explore the distribution between movies and TV shows across different regions
- **Trend Identification**: Analyze release patterns, duration trends, and rating distributions
- **Actionable Insights**: Extract meaningful business intelligence from the content catalog

## 🛠️ Technical Implementation

### Technologies Used
- **Python 3** - Core programming language
- **Pandas** - Data manipulation and analysis
- **Seaborn** - Advanced data visualization
- **Jupyter Notebook** - Interactive development environment

### Dataset Specifications
- **Original Size**: 7,789 entries × 11 columns
- **Cleaned Size**: 7,787 entries × 11 columns
- **Time Period**: Content available up to 2021
- **Source**: Flixable (Third-party Netflix search engine) via Kaggle

### Data Columns Analyzed
- `Show_Id`, `Category`, `Title`
- `Director`, `Cast`, `Country`
- `Release_Date`, `Rating`, `Duration`
- `Type` (Genres), `Description`

## 🔍 Analytical Approach

### Phase 1: Data Quality & Preparation
- **Duplicate Management**: Identified and removed 2 duplicate records
- **Missing Value Analysis**: Comprehensive assessment using `isnull().sum()` and heatmap visualization
- **Data Integrity**: Ensured dataset consistency and reliability

### Phase 2: Exploratory Analysis
- **Statistical Summaries**: Used `.describe()`, `.info()`, and `.shape` for data understanding
- **Data Structure**: Analyzed data types and memory usage optimization
- **Pattern Recognition**: Identified content distribution patterns

### Phase 3: Advanced Queries
- **Targeted Filtering**: Implemented `isin()` method for specific content queries
- **Content Retrieval**: Successfully extracted information for "House of Cards" and other titles
- **Relationship Mapping**: Explored connections between directors, countries, and content types

## 📈 Key Findings

### Data Quality Insights
- **Director Information**: Significant number of missing values (2,388 entries)
- **Cast Details**: Moderate missing data (718 entries)
- **Country Information**: Regional data gaps (507 entries)
- **Rating & Release Date**: Minimal missing values, indicating good temporal data quality

### Content Analysis Highlights
- **Diverse Catalog**: Extensive collection of international and domestic content
- **Genre Variety**: Wide range of content types from dramas to documentaries
- **Global Reach**: Content sourced from multiple countries including US, Brazil, India, and more

## 🚀 Getting Started

### Prerequisites
```bash
python >= 3.8
pandas >= 1.3.0
seaborn >= 0.11.0
jupyter >= 1.0.0

# Clone repository
git clone https://github.com/yourusername/netflix-data-analysis.git

# Navigate to project directory
cd netflix-data-analysis

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook "Netflix Analysis.ipynb"

# 📚 Book Sales & Ratings Exploratory Data Analysis

---

## 🗂️ Table of Contents

- [Project Overview](#-project-overview)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Key Visualizations](#-key-visualizations)
- [Main Insights](#-main-insights)
- [Installation & Usage](#-installation--usage)
- [Tech Stack](#-tech-stack)
- [Author](#-author)

---

## 🔍 Project Overview

This project is an **Exploratory Data Analysis (EDA)** conducted on a book sales dataset. The goal is to understand publishing market dynamics through three main perspectives:

| Axis | Description |
|------|------------|
| 📈 **Market Analysis** | Identify top-performing genres, authors, and time periods |
| 🖊️ **Author Performance** | Evaluate the impact of an author’s reputation on sales and ratings |
| 🔎 **Trend Analysis** | Detect evolving reading preferences and publishing patterns |

---

## 📦 Dataset

> **Source:** [Kaggle — Books Sales and Ratings](https://www.kaggle.com/)

The dataset contains detailed information about thousands of books:

| Column | Description |
|--------|------------|
| `Publishing Year` | Year of publication |
| `Book Name` | Title of the book |
| `Author` | Author’s name |
| `Author_Rating` | Author level (Novice / Intermediate / Famous / Excellent) |
| `Book_average_rating` | Average rating given by readers |
| `Book_ratings_count` | Number of ratings received |
| `genre` | Literary genre (fiction, nonfiction, children, genre fiction) |
| `gross sales` | Total gross sales |
| `publisher revenue` | Publisher revenue |
| `sale price` | Selling price |
| `sales rank` | Sales ranking |
| `units sold` | Number of copies sold |

---

## 🗃️ Project Structure

```
📁 book-sales-eda/
│
├── 📓 Book_Sale_EDA.ipynb        # Main notebook — complete EDA
│
├── 📁 output/
│   ├── book_ratings_distribution.png
│   ├── correlation_heatmap.png
│   ├── books_per_year.png
│   ├── reviews_vs_rating.png
│   ├── author_rating_vs_book_rating.png
│   ├── ratings_by_genre.png
│   ├── price_vs_units_sold.png
│   ├── revenue_by_genre.png
│   └── top_authors_units_sold.png
│
└── 📄 README.md
```

---

## 📊 Key Visualizations

<table>
  <tr>
    <td align="center"><b>Ratings Distribution</b><br><img src="output/book_ratings_distribution.png" width="380"/></td>
    <td align="center"><b>Correlation Heatmap</b><br><img src="output/correlation_heatmap.png" width="380"/></td>
  </tr>
  <tr>
    <td align="center"><b>Publications per Year</b><br><img src="output/books_per_year.png" width="380"/></td>
    <td align="center"><b>Revenue by Genre</b><br><img src="output/revenue_by_genre.png" width="380"/></td>
  </tr>
  <tr>
    <td align="center"><b>Top 10 Authors</b><br><img src="output/top_authors_units_sold.png" width="380"/></td>
    <td align="center"><b>Price vs Units Sold</b><br><img src="output/price_vs_units_sold.png" width="380"/></td>
  </tr>
</table>

---

## 💡 Main Insights

### 🏆 Genre fiction dominates the market  
Genre fiction alone generates over **1.6 million in gross sales**, more than 7× higher than nonfiction (second place). Inventory and marketing strategies should prioritize this segment.

### 💰 Low prices = high volume  
Books priced below **€10** account for the vast majority of high sales volumes (30,000–60,000 units). Above €15, sales drop sharply. Affordable pricing is a key driver of volume.

### ⭐ Average rating does not predict sales  
Despite nearly zero correlation between `Book_average_rating` and `units sold`, most books cluster around **4.0/5**. Visibility and author reputation are more influential than perceived quality alone.

### 📖 Series build loyalty and drive sales  
The top 10 authors are dominated by creators of **long-running series** (Stephen King, Janet Evanovich, Jim Butcher, Robert Jordan). Series-based engagement is a structural competitive advantage in the publishing industry.

### 📅 Publishing boom since the 2000s  
The number of annual publications has grown **exponentially** since the 2000s, peaking around 2010–2015. This increased competition makes data-driven decision-making more critical than ever for publishers.

---

## ⚙️ Installation & Usage

### 1. Clone the repository

```bash
git clone https://github.com/your-username/book-sales-eda.git
cd book-sales-eda
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

> **Main dependencies:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `jupyter`

### 4. Run the notebook

```bash
jupyter notebook Book_Sale_EDA.ipynb
```

---

## 🛠️ Tech Stack

| Tool | Usage |
|------|------|
| **Python 3.12** | Main programming language |
| **Pandas** | Data manipulation and cleaning |
| **NumPy** | Numerical computations |
| **Matplotlib** | Static visualizations |
| **Seaborn** | Advanced statistical visualizations |
| **Jupyter Notebook** | Interactive analysis environment |

---

## 👤 Author: Cedric Konkobo

<div align="center">

**Project carried out as part of personal learning**

*Feel free to ⭐ the repo if you found this project useful!*

</div>

---

<div align="center">
<sub>📚 Book Sales & Ratings EDA — Exploratory analysis of the publishing market</sub>
</div>



# 📚 Amazon Bestseller Books Web Scraper

This project scrapes the **Amazon Bestseller Books** page and extracts book data such as **title, author, rating, and price**, then saves it into a CSV file using Python.

---

## 🔍 Features

✅ Scrapes:
- 📖 Book Title  
- ✍️ Author  
- ⭐ Rating  
- 💰 Price  

✅ Stores:
- Data is stored in a **CSV file (`amazon_products.csv`)**.

✅ User Friendly:
- Uses polite time delay between requests (`time.sleep(3)`)  
- Handles missing data gracefully  
- Shows how many books were found per page  

---

## 🧰 Tools & Libraries

- `pandas` – for data storage and CSV creation  
- `requests` – to fetch HTML content  
- `BeautifulSoup` – to parse and extract elements from HTML  
- `re`, `warnings`, `time` – for cleaning, handling delays, and suppressing warnings

---

## 📦 Files

| File                     | Description                          |
|--------------------------|--------------------------------------|
| `amazon_scraper.py`      | Main scraping script                 |
| `amazon_products.csv`    | Output file with book data           |
| `README.md`              | Project documentation                |

---

## 🛠 How It Works

1. The script sends a request to Amazon's Bestseller Books page.
2. Parses the HTML content using BeautifulSoup.
3. Extracts details for each book (Title, Author, Rating, Price).
4. Loops through multiple pages (`no_pages = 2` by default).
5. Saves the result into `amazon_products.csv`.
6. Displays the first 18 rows as a preview.

---

## ▶️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/amazon-books-scraper.git
cd amazon-books-scraper

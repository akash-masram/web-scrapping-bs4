# 🕸️ Web Scraping with BeautifulSoup — Anime Products Scraper

This project demonstrates how to **scrape product data** from [ImageAnime.com](https://www.imageanime.com) using **BeautifulSoup**, and how to **push the Colab notebook directly to GitHub**.

---

## 📌 Project Overview

The script extracts:

- ✅ Product Name  
- ✅ Original Price  
- ✅ Sale Price  
- ✅ Product Image URL  

All the data is saved into a **CSV file** named `products.csv`.

---

## 📦 Technologies Used

- Python
- BeautifulSoup (`bs4`)
- pandas
- requests
- Google Colab
- GitHub

---

## 🚀 Workflow

1. Data is scraped from [https://www.imageanime.com](https://www.imageanime.com) using BeautifulSoup.
2. The extracted data is stored in a pandas DataFrame.
3. The DataFrame is exported to a local CSV file (`products.csv`).
4. The notebook is uploaded to GitHub **directly from Google Colab**.

---

## ☁️ Uploading to GitHub from Google Colab

To push your Colab notebook directly to GitHub:

1. Open the notebook in Google Colab.
2. Go to `File > Save a copy in GitHub`.
3. Choose your repository (e.g., `latest-web-scrapping-bs4`).
4. Add a commit message and click **OK**.
5. ✅ Your `.ipynb` file will now appear in your GitHub repo.

---

## ❗ Why the CSV File Isn’t Uploaded Automatically

> Colab runs in a **temporary virtual environment**.

- When you save a CSV using `df.to_csv("products.csv", index=False)`, it’s created in that session's **ephemeral storage**.
- The GitHub integration in Colab only pushes the notebook file, not any files saved in the session like CSVs or images.

---

## 📤 How to Upload the CSV to GitHub

To include your `products.csv` file in the repo:

### Step 1: Download CSV from Colab
```python
from google.colab import files
files.download('products.csv')

```

##  Step 2: Manually Upload to GitHub


1. Go to your GitHub repository.
2. Click on **“Add file”** → **“Upload files”**.
3. Drag and drop the downloaded `products.csv`.
4. Add a commit message.
5. Click **“Commit changes”**.



## 📬 Contact

If you have suggestions or issues, feel free to **open an issue** or **fork this repo**.  
🎉 Happy scraping!

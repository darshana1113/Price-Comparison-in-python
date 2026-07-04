<div align="center">

# 🛒 Amazon & Flipkart Price Checker

A simple desktop GUI application built with **Python (Tkinter)** that lets you search for a product and compare its title and price across **Amazon India** and **Flipkart** side by side.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-orange)
![BeautifulSoup](https://img.shields.io/badge/Scraping-BeautifulSoup4-green)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

</div>

---

## 📑 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Screenshots](#-screenshots)
- [Troubleshooting](#-troubleshooting)
- [Notes & Disclaimer](#-notes--disclaimer)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

## ✨ Features

- 🔍 Search any product by name
- 📊 View top 10 results from Amazon and Flipkart in separate tables
- 🖥️ Clean and simple Tkinter-based GUI
- 🧹 Clear All button to reset search and results
- 🌐 Uses `requests` and `BeautifulSoup` for web scraping

## 🧰 Tech Stack

| Component | Purpose |
|---|---|
| **Python 3** | Core language |
| **Tkinter** | GUI |
| **Requests** | HTTP requests |
| **BeautifulSoup4** | HTML parsing |

## ⚙️ Installation

<details>
<summary><b>Click to expand setup steps</b></summary>

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. Install the required dependencies
   ```bash
   pip install requests beautifulsoup4
   ```

3. Run the application
   ```bash
   python main.py
   ```
   *(replace `main.py` with your actual script filename)*

</details>

## ▶️ Usage

1. Launch the application.
2. Enter the product name in the input field.
3. Click **Search** to fetch and display results from Amazon and Flipkart.
4. Click **Clear All** to reset the input field and tables.

## 📸 Screenshots

<details>
<summary><b>Click to view app screenshot</b></summary>

![App Screenshot](screenshot.png)

*(Replace `screenshot.png` with an actual screenshot of your app, placed in the repo root)*

</details>

## 🛠️ Troubleshooting

<details>
<summary><b>Search returns empty results</b></summary>

Amazon/Flipkart frequently change their HTML class names. If scraping breaks:
- Inspect the page manually (right-click → Inspect) on a product search page
- Update the `class`/`id` selectors in `get_title_amazon`, `get_price_amazon`, `get_title_flipkart`, and `get_price_flipkart`

</details>

<details>
<summary><b>Requests are blocked or return errors</b></summary>

- Avoid sending too many requests too quickly
- Make sure the `User-Agent` header is set (already included in the script)
- Try again after some time if temporarily rate-limited

</details>

## 📝 Notes & Disclaimer

> [!WARNING]
> This project scrapes publicly visible HTML from Amazon and Flipkart search results. Website structures change frequently, so selectors used in this script may need periodic updates if scraping stops working. Web scraping may be against the Terms of Service of some websites — use this project for **educational purposes only**.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](../../issues) if you want to contribute.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

<div align="center">

Made by(https://github.com/darshana1113)

</div>

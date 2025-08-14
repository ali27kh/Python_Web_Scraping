# 📊 Enterprise Data Scraping and Email Validation

## 📌 Project Overview
This project automates the collection of enterprise-related data from multiple sources using **Python** and **Selenium** for web scraping. It includes validating email addresses, extracting comments from a Facebook post, and gathering enterprise information (e.g., name, address, SIREN) from two French business directories. The scraped data is saved as CSV files for further analysis.

---

## 📂 Data Sources
- **Email Validation**: [VerifyEmailAddress.org](https://www.verifyemailaddress.org) to check email validity.
- **Facebook Comments**: Extracted from a specific post on [MBI Network](https://www.facebook.com/MBI.NETWORK/photos/a.644456839037406/2125335377616204/).
- **Enterprise Info**:
  - [Le Figaro Entreprises](https://entreprises.lefigaro.fr)
  - [Manageo](https://www.manageo.fr/entreprises)

---

### ** Chrome Setup**
Configure and initialize Chrome WebDriver for scraping.

```python
from selenium import webdriver
from selenium.webdriver.chrome.service import Service
from selenium.webdriver.chrome.options import Options
from webdriver_manager.chrome import ChromeDriverManager

chrome_options = Options()
chrome_options.add_argument("--start-maximized")
driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), options=chrome_options)
```

---

## 📦 Requirements
```bash
pip install selenium webdriver-manager pandas requests
```

---

## ▶️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/ali27kh/Python_Web_Scraping.git
   cd Python_Web_Scraping
   ```
2. Install dependencies.
3. Run the scraping script.

---

## 📌 Key Insights
- Email validation ensures reliable contact information using VerifyEmailAddress.org.
- Facebook comment scraping from posts.
- Le Figaro and Manageo provide complementary enterprise data.
- Selenium automation ensures robust handling of dynamic web content.

---

## 📜 License
MIT License

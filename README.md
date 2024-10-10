# Bangbet Web Scraper with Python: Automate Betting Data Extraction

This Python script automates the extraction of soccer betting data from **Bangbet**. It scrapes match times, team names, and betting odds (home, draw, away) from the Bangbet website, providing a quick and efficient way to gather betting data for further analysis.

## 📌 Features

- **Automated Betting Data Scraping**: Extracts match times, teams, and odds from Bangbet’s soccer section.
- **CSV Output**: Saves the data into a CSV file for easy access and analysis.
- **Headless Browser**: Runs in a headless mode (no GUI), making the scraping process more efficient.
- **Handles Pagination**: Automatically scrolls and loads more matches, ensuring complete data collection.
- **Duplicate Removal**: Detects and removes duplicate records to maintain clean datasets.

## 🚀 How It Works

The scraper visits the Bangbet sports betting page, extracts soccer match details, and saves the data in a structured CSV format. The script scrolls through the available matches and loads additional data by clicking the "Load More" button, ensuring all available matches are scraped.

### Key Steps:

1. **Headless Browser Setup**: The script uses a headless Selenium browser to navigate the Bangbet website.
2. **Click and Scroll**: It clicks the "Today" section to load today's matches and scrolls through pages to capture all match data.
3. **Data Scraping**: Using `lxml`, the script extracts match times, home/away teams, and betting odds.
4. **Data Storage**: The scraped data is saved as a CSV file for easy access and analysis.
5. **Duplicate Handling**: Ensures no duplicate records in the final output file.

## 🛠️ Requirements

Before running the script, ensure the following packages are installed:

- **Python 3.x**
- **Selenium**
- **BeautifulSoup4**
- **lxml**
- **pandas**
- **ChromeDriver** (or the appropriate driver for your browser)

Install the required packages using pip:
```bash
pip install selenium beautifulsoup4 lxml pandas

  
**🏃 How to Run the Script**
**Clone the Repository:**
  git clone https://github.com/YourUsername/Bangbet-Web-Scraper.gitSet up ChromeDriver:
Download and install ChromeDriver for your browser. Ensure the ChromeDriver is in your system path.

**Run the Python Script:**
  python bangbet_scraper.py

**View Result**s:
The scraped data will be saved as BANGBET.csv in the specified directory.

**📁 Output**
The output CSV file (BANGBET.csv) contains the following fields:

**TIME: The match time.
HOME TEAM: The home team in the match.
AWAY TEAM: The away team in the match.
HOME ODD: Odds for the home team to win.
DRAW ODD: Odds for a draw.
AWAY ODD: Odds for the away team to win.
BOOKMAKER: The bookmaker name (Bangbet).**

**🔧 Future Improvements**
Expand to Other Sports: Scrape data from other sports like basketball or tennis.
**Error Handling**: Add more robust error handling for page load issues or website changes.
**Enhance Efficiency:** Improve the script’s speed by optimizing scrolling and data extraction techniques.
**📝 License**
This project is licensed under the MIT License. See the LICENSE file for more details.
**
🤝 Contributing**
Feel free to contribute by opening issues, suggesting improvements, or submitting pull requests. All feedback is welcome!

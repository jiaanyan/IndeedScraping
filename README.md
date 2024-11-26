# Indeed.com Web Scraper

A Python-based web scraper for Indeed.com that handles CAPTCHA detection and provides robust job data collection capabilities.

## 🎓 Academic Attribution

This code is inspired by University of Toronto, MIE 1624, Assignment 3.

## 🔧 Test Environment

- Operating System: Windows 11
- Python Version: 3.9.20
- Browser: Firefox

## ✨ Features

- Automated job posting data collection from Indeed.com
- CAPTCHA detection and handling
- Robust error management
- Data export to CSV format
- Human behavior simulation to avoid scraping detection

## 🚀 Getting Started

### Prerequisites

- Python 3.9.x
- Firefox Browser
- Required Python packages (listed in requirements.txt)

### Usage

1. Download the code to your local computer

2. Open the Jupyter notebook

3. Modify only the first code block with your desired parameters:

   ```python
   # 1.job position
   position = "director of analytics"
   
   # 2.job location
   locations = "Toronto, ON"
   
   # 3.Number of postings to scrape (200 is recommended)
   postings = 200
   ```

> **Note**: It's recommended to keep `postings` around 200 each time. Larger values may lead to errors.

## 🛡️ Anti-CAPTCHA Innovation

This scraper implements innovative CAPTCHA handling mechanisms:

- Automatic CAPTCHA detection
- Built-in retry rules
- Session management
- IP address monitoring

### IP Address Management

If you encounter an `IpIsBlockedError`, it means Indeed.com has temporarily or permanently flagged your IP address as a bot. Solutions include:

- Using proxy tools to change your IP address
- Using Residential IP addresses for better scraping experience
- Avoiding Datacenter IPs when possible

### Performance Notes

Based on testing:

- VPS broadcast IPs can typically scrape 1000+ rows before being banned
- CAPTCHA triggers are automatically handled by the program
- The script uses `time.sleep()` to simulate human behavior
- Sleep intervals can be adjusted to balance speed and detection risk

## ⚠️ Limitations

### Time Consumption

- Processing time scales with the number of postings
- Example: 30 postings ≈ 5 minutes
- Larger datasets will require proportionally more time
- The script prioritizes reliability over speed

## 📝 Notes

- The program includes deliberate delays to mimic human behavior
- Sleep intervals can be adjusted in the code
- Always respect Indeed.com's terms of service and rate limits
- Consider using this tool for educational purposes only

## ⚖️ Legal Disclaimer

This tool is for educational purposes only. Users are responsible for ensuring compliance with Indeed.com's terms of service and applicable laws regarding web scraping.

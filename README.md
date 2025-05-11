# 🏠 Mini Project Data Engineering: Analysis of Popular Topics in Kompas.com and Tribunnews.com

This project aims to analyze the most frequently reported news topics on May 6, 7, and 8, 2025 from two popular news portals in Indonesia: Kompas.com and Tribunnews.com. The goal is to see the tendency or focus of each media on certain issues.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg) ![License](https://img.shields.io/badge/license-MIT-green.svg)

## Installation

To install the necessary packages, run the following command:

```bash
pip install requests beautifulsoup4 pandas matplotlib
```

## 🛠 Tech

- Python - to perform web scraping from the website
- Requests & BeautifulSoup - library to scrapping data
- Pandas - data manipulation
- Matplotlib - data visualization

## Usage/Examples

Here's a basic example of how to use this project:

```python
import requests
from bs4 import BeautifulSoup

url = 'https://www.kompas.com/'
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')

# Example of extracting headlines
headlines = soup.find_all('h2')
for headline in headlines:
    print(headline.text)
```

## Contributing

We welcome contributions! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

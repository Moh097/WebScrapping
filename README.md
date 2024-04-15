# Top 100 Movies Scraper

## Overview
This Python script extracts a list of the "100 Greatest Movies" from a static snapshot of Empire Online's article, hosted on the Wayback Machine. The list is then saved in a text file, ordered from the best to the 100th movie.

## Features
- **Web Scraping**: Fetches data from an archived webpage.
- **Data Parsing**: Uses BeautifulSoup to parse HTML content efficiently.
- **Data Storage**: Saves the structured data into a plain text file.

## Prerequisites
Before you run this script, you need to install Python and some packages. Here's how you can prepare your environment:

### Python Installation
Ensure that Python (version 3.x) is installed on your machine. You can download it from [python.org](https://www.python.org/downloads/).

### Dependencies
This project uses `requests` and `BeautifulSoup` for web scraping. Install them using pip:

```bash
pip install requests beautifulsoup4
```

## Project Files
- **`main.py`**: The main Python script that performs the web scraping.
- **`movies.txt`**: The output file where the movie titles are saved.

## Usage
To run this script, navigate to the project directory in your terminal, and execute the following command:

```bash
python main.py
```

### Output
After running the script, the `movies.txt` file will be populated with the top 100 movies, listed from the best to the 100th. Each title will be on a new line.

## How It Works
1. **Fetching Web Content**: The script sends a HTTP request to retrieve the HTML content of the archived Empire Online page.
2. **HTML Parsing**: BeautifulSoup is used to parse the HTML document and extract elements containing movie titles.
3. **Data Extraction**: Movie titles are extracted from the specified HTML tags and attributes.
4. **Data Manipulation**: The list of movies is reversed to correct the order from 1 to 100.
5. **File Writing**: The script writes each movie title to the `movies.txt` file.

## Error Handling
The script includes basic error handling for HTTP errors and file I/O issues, ensuring any problems are reported clearly.

## Contributions
Contributions are welcome. If you wish to contribute, please fork the repository and propose your changes via a pull request.

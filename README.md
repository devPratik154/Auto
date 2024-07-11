Instagram Automation Tool
Overview
This tool allows you to log in to your Instagram account and scrape the likes and comments from any specified Instagram post URL. The scraped data is output in JSON or CSV format.

Features
Secure login to Instagram
Scrape likes and comments from a specified post
Output data in JSON or CSV format

Prerequisites
Python 3.x
Google Chrome Browser
ChromeDriver (ensure it matches your Chrome browser version)

Installation
1.Clone the Repository

git clone https://github.com/yourusername/instagram-automation-tool.git
cd instagram-automation-tool

2.Create a Virtual Environment

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install Required Packages

pip install -r requirements.txt

Download ChromeDriver

1.Download the ChromeDriver that matches your version of Chrome from here.
2.Place the chromedriver executable in your project directory or ensure it's in your PATH.

Usage
Run the Script

python instagram_automation.py

2.Input Your Instagram Credentials

The script will prompt you to enter your Instagram username and password.
Enter the Instagram Post URL

Provide the URL of the Instagram post you wish to scrape.
Choose Output Format

The script will output the scraped data in JSON format by default. To output in CSV, modify the output_data function in the script.
Script Breakdown
instagram_login(username, password): Logs into Instagram using the provided credentials.
validate_url(url): Validates the provided Instagram post URL.
scrape_post_data(driver, post_url): Scrapes likes and comments from the specified post URL.
output_data(data, output_format): Outputs the scraped data in the specified format (JSON or CSV).

Example
Here's a simple example of how to run the tool:

Start the script:

python instagram_automation.py
Input your credentials and post URL:

Enter Instagram username: your_username
Enter Instagram password: your_password
Enter Instagram post URL: https://www.instagram.com/p/POST_ID/
The script will log in, scrape the data, and save it to instagram_data.json (or instagram_likes.csv and instagram_comments.csv if CSV format is selected).


---

# Stock News Notifier

This Python script utilizes stock and news APIs to fetch stock price information and relevant news articles. It monitors the stock prices and sends an SMS notification via Twilio if there's a significant increase or decrease in the stock price of a specified company.

## Project Overview

The script performs the following steps:

1. Fetches daily stock data using the Alpha Vantage API to compare yesterday's closing price with the day before yesterday's closing price.
2. Calculates the percentage difference between the two closing prices and determines if the stock price has increased or decreased significantly.
3. Retrieves news articles related to a specified company from the News API when there is a substantial change in stock price.
4. Sends SMS notifications via Twilio, containing the headlines and descriptions of the fetched news articles.

## Setup Instructions

1. Clone or download this repository to your local machine.

2. Install required Python packages:
   ```bash
   pip install requests twilio
   ```

3. Update the following variables in the Python script `stock_news_notifier.py`:
   - `STOCK_NAME`: The stock symbol you want to monitor (e.g., TSLA for Tesla Inc).
   - `COMPANY_NAME`: The name of the company to fetch news articles for.
   - `STOCK_API_KEY`: Your API key from Alpha Vantage.
   - `NEWS_API_KEY`: Your API key from News API.
   - `TWILIO_SID`: Your Twilio account SID.
   - `TWILIO_AUTH_TOKEN`: Your Twilio authentication token.
   - `VIRTUAL_TWILIO_NUMBER`: Your virtual Twilio number.
   - `VERIFIED_NUMBER`: Your verified phone number with Twilio.

4. Run the Python script:
   ```bash
   python stock_news_notifier.py
   ```

## Dependencies

- `requests`: Used for making HTTP requests to APIs.
- `twilio`: Twilio's Python library for sending SMS notifications.

## Contributions

Contributions to improve this project are welcome! Feel free to fork the repository, make changes, and create pull requests.

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to tailor the content to add more details or instructions as needed for your project.

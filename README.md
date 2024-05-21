# Forex Trading Bot and Back-testing System

This project is an end-semester AI-based forex trading system that includes a back-testing module, a web dashboard, and a smart trading bot. The system fetches historical data from OANDA, performs technical analysis, displays data in a web interface, and autonomously executes trades based on predefined strategies.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Setup Guide](#setup-guide)
   - [Requirements](#requirements)
   - [Installation](#installation)
   - [Running the Project](#running-the-project)
3. [Modules](#modules)
   - [Module 1: Fetching Data and Back-testing](#module-1-fetching-data-and-back-testing)
   - [Module 2: Web Dashboard](#module-2-web-dashboard)
   - [Module 3: Smart Bot](#module-3-smart-bot)
4. [Future Prospects](#future-prospects)
5. [References](#references)

## Project Overview
The project involves developing a Forex trading system that includes:
- A module to fetch historical data, perform back-testing, and analyze various trading strategies.
- A web dashboard to visualize trading data and patterns in real-time.
- A smart bot to autonomously execute trades based on technical analysis and predefined strategies.

## Setup Guide

### Requirements
- Python 3.7+
- Flask
- Vue.js
- Pandas
- NumPy
- Matplotlib
- OANDA API Access
- Requests

### Installation

1. **Clone the Repository**
   ```sh
   git clone https://github.com/fatehmehmood123/TradingOANDA.git
   cd TradingOANDA
   ```

2. **Set Up a Virtual Environment**
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. **Setup defs.py**
   Get Api key and Account id from OANDA Account

4. **Access the Dashboard**
   ```sh
   cd Webdashboard
   pip install -r requirements.txt
   python app.py
   flask run
   http://localhost:5000
   ```

3. **Running the bot**
   ```sh
   cd TradingBot
   pip install -r requirements.txt
   python bot.py
   ```


## Modules

### Module 1: Fetching Data and Back-testing
- **Fetching Data**: Uses the OANDA API to get historical data for various trading pairs.
- **Technical Analysis**: Implements indicators like moving averages, Bollinger Bands, MACD, and candlestick patterns such as Marubozu, Doji, Hammer, Spinning Top, Engulfing, and Piercing Line.
- **Back-testing**: Applies strategies such as moving average crossovers and inside bar patterns to historical data to evaluate their effectiveness.

### Module 2: Web Dashboard
- **Frontend**: Built using HTML, CSS, JavaScript, and Vue.js.
- **Backend**: Flask API serves trading data.
- **Features**: Displays real-time trading data, candlestick patterns, and allows for interactive exploration of trading pairs.

### Module 3: Smart Bot
- **Autonomous Trading**: Executes trades based on predefined strategies like moving average crossovers.
- **User Inputs**: Accepts stop-loss and take-profit levels.
- **Logging**: Logs all trades and reflects them in the OANDA dashboard.

## Future Prospects
- **Admin App**: To control parameters, monitor profits, and manage trading strategies.
- **Machine Learning**: Implement predictive models using historical data.
- **Web Scraper**: Fetch and analyze market news for additional trading signals.
- **Multiple Bots**: Deploy bots across different time frames using multithreading.
- **Bot Deployment**: Ensure stable and scalable deployment of trading bots.

## References
- Project inspired by tutorials from BlueFeverSoft on YouTube.
- [Youtube Playlist](https://www.youtube.com/watch?v=zKk2iuuNJO0&list=PLZ1QII7yudbecO6a-zAI6cuGP1LLnmW8e&index=1)
- [OANDA API Documentation](https://www.oanda.com/)
- [GitHub Repository](https://github.com/fatehmehmood123/TradingOANDA)
- [Medium Article](https://medium.com/@fatehmehmood/revolutionizing-forex-trading-a-comprehensive-overview-of-ai-driven-back-testing-system-web-b9662db21aa9)

Thank you for exploring this project! For any questions or further information, feel free to reach out or connect on LinkedIn. Follow me on Medium for more insights and updates.
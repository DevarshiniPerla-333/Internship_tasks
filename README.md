# INTERNSHIP _ TASKS 

COMPANY: CODETECH IT SOLUTIONS

NAME: PERLA DEVARSHINI

INTERN ID: CT08ICG

DOMAIN : PYTHON PROGRAMMING

DATE OF DURATION : DECEMBER 30TH 2024 TO JANUARY 30TH 2025

MENTOR NAME : NEELA SANTOSH

# API INTEGRATION AND DATA VISUALIZATION

Project Overview: Weather Data Fetching and Visualization This project involves fetching weather data for a specific city from the OpenWeatherMap API, processing it, and visualizing it using Plotly. The goal is to retrieve a 5-day weather forecast, extract important details such as temperature, humidity, and pressure, and then present the data in both tabular form and as an interactive graph.

Key Objectives:

Weather Data Fetching: The script fetches weather data using the OpenWeatherMap API. The endpoint provides a 5-day weather forecast for a given city, including details about temperature, humidity, pressure, and weather description at various time intervals.

Data Processing: The data returned by the API is parsed, and a pandas DataFrame is created to store the relevant information: Datetime: The date and time of the forecast. Temperature: The temperature in Celsius. Humidity: The humidity percentage. Pressure: The atmospheric pressure. Weather Description: A brief description of the weather (e.g., clear sky, few clouds, etc.).

Data Visualization: The script visualizes the temperature data using Plotly. A line chart is created to show how the temperature changes over the forecasted time period, with markers for each data point. The chart is interactive, allowing users to hover over points to see detailed information about the temperature at each time.

Workflow: API Call: The script makes a request to the OpenWeatherMap API with the provided city name and API key. It fetches the 5-day forecast data, which includes weather information for every 3-hour interval.

Data Extraction: The script parses the JSON response from the API and extracts the relevant fields: Datetime: When the forecast is for. Temperature, Humidity, Pressure: For each time point. Weather Description: A brief
description of the weather.

Data Display: The weather data is displayed in a pandas DataFrame for the user to see the raw data.

Chart Visualization: A Plotly chart is generated to visualize the temperature over the next 5 days. The x-axis represents the date and time, while the y-axis shows the temperature in Celsius. The chart uses a line graph with markers for each time point.

Technologies Used:

Python Libraries:

Requests: To make HTTP requests to the OpenWeatherMap API. Pandas: For data manipulation and storage in DataFrame format. Plotly: For creating interactive charts and visualizations. OpenWeatherMap API: Used to fetch weather data for a specified city, including the 5-day forecast. Visualization: The data is visualized using Plotly, which provides a flexible and interactive way to present the data.

# AUTOMATED-REPORT-GENERATION

Project Overview: Automated Sales Report Generation This project involves creating an automated report generation system using Python, which reads data from a CSV file, processes the data, generates a bar chart, and compiles everything into a PDF report.

Key Objectives:

Data Handling: The script reads sales data from a CSV file (sales_data.csv), which contains sales data by product, and processes it to summarize the total revenue by product.

Data Visualization: A bar chart is generated to visually represent the revenue of different products. The chart is saved as an image file (bar_chart.png).

PDF Report Generation: The report is created using the FPDF library in Python. It includes: A title. The generated bar chart. A summary of revenue by product. The report is saved as a PDF file (sales_summary_report.pdf).

Workflow:

CSV File: The script loads the CSV file, which contains two columns: Product and Revenue. Data Processing: The script groups the data by Product and calculates the sum of the Revenue for each product. Chart Generation: A bar chart is generated using the Matplotlib library, displaying the total revenue for each product. PDF Creation: A PDF report is generated using the FPDF library. The bar chart is inserted into the report, followed by a list of revenue summaries for each product.

Final Output: The output includes two files: bar_chart.png – The visual chart. sales_summary_report.pdf – The comprehensive PDF report with the summary and chart.

Technologies Used: Python Libraries: Pandas: To read and process the CSV data. Matplotlib: To create the bar chart for visual representation. FPDF: To generate the PDF report.

File Formats: CSV: Used to store the raw data. PNG: Used for saving the chart image. PDF: Used for creating the final report.

# AI CHATBOT WITH NLP

What is NLP? Natural Language Processing (NLP) is a field of artificial intelligence that focuses on the interaction between computers and human language. It involves tasks like language understanding, sentiment analysis, and text classification.
Libraries like NLTK and spaCy are designed to make it easier to implement NLP tasks in Python. NLTK (Natural Language Toolkit) and spaCy provide tools to tokenize, lemmatize, and process text efficiently, making them ideal for building chatbots.

Setting Up the Environment To build a chatbot, you'll need to install some basic dependencies such as spaCy and NLTK. You can do this via pip: bash Copy code pip install nltk spacy You'll also need to install spaCy’s English language model: bash Copy code python -m spacy download en_core_web_sm

Building the Chatbot The chatbot can follow a simple rule-based approach, where the user’s input is matched with predefined patterns or keywords. Use spaCy or NLTK for text preprocessing, such as tokenization and lemmatization. You can create a dictionary of common responses and match the user's query with the most appropriate response based on the input.

Basic Implementation Flow Text Processing: Convert user input to lowercase, tokenize, and remove stop words using spaCy or NLTK. Keyword Matching: Look for specific words or phrases in the user’s input and return predefined responses. Default Response: If no match is found, provide a default response (e.g., "I'm sorry, I didn't understand that.").

Handling Errors and Dependencies You encountered an installation error when trying to install spaCy. The error is related to missing build tools required for compiling packages like numpy, which is used by spaCy and other dependencies. The error log also suggests that you're missing Visual Studio build tools on Windows, which are needed for compiling C extensions. Steps to resolve errors:

Install Visual Studio Build Tools for C++ (required for compiling dependencies). Upgrade pip to the latest version (pip install --upgrade pip). Install numpy separately (pip install numpy) before trying to install spaCy. If errors persist, try installing a precompiled version of spaCy.

Enhancements After setting up the basic chatbot, you can enhance it by: Adding more advanced NLP models for better understanding. Training a classifier to identify user intents for more dynamic responses. Storing context to handle multi-turn conversations (e.g., remembering the user’s previous questions or requests).

Example Code Walkthrough You can create a basic keyword-based chatbot using the following steps: Use spaCy to preprocess user input (e.g., tokenization, lemmatization). Match the processed input with predefined keywords. Return a response based on matched keywords

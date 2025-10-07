# 🌤️ Historical Weather Data Scraper & Visualizer

## 📌 Assignment Details

- **Assignment:** Historical Climate Data Collection
- **Student Name:** Sanchi Madaan
- **Student ID:** 0395260
- **Email:** smadaan2@academic.rrc.ca
- **Section:** 261247
- **Date Created:** 27 March, 2025

---

## 📖 Project Overview

This project is a full-fledged Python application that scrapes **daily historical weather data** for **Winnipeg** from the official [Environment Canada](https://climate.weather.gc.ca) website, stores it in a local **SQLite database**, and enables interactive data analysis and visualization through a **modern Tkinter GUI interface**.

From raw data scraping to querying and visualization — the entire weather processing workflow is encapsulated in this easy-to-use app.

---

## ⚙️ Features

- 🌐 **Scrape historical daily temperature data** (Max, Min, Mean) using `HTMLParser`
- 📆 **Month-by-month scraping** until no more data is available
- 🧵 **Multithreaded scraping** for faster performance
- 💽 **SQLite-backed database** for efficient storage and querying
- 📈 Generate **boxplots** and **line plots** via `matplotlib`
- 🖼️ **Modern GUI built with Tkinter** — mobile-sized window, hover effects, scrollable layout
- 🤖 Integrated **Chatbot assistant** for quick yearly queries
- 🪵 Comprehensive logging in `scrape.log`

---

## 📂 GUI Application (`weather_tkinter_app.py`)

### 🔹 Highlights

- 🎨 **Interactive & user-friendly layout**
- 🔄 **Buttons to scrape or update data** (historical or current month)
- 📊 **Visualize data easily**:
  - Boxplot for temperature trends (by year range)
  - Line plot for daily mean temperatures (specific month/year)
- 💬 Built-in **chatbot assistant** (type a year to see mean temperature samples)
- 🖱️ Mouse-scroll and touchpad friendly
- 🧼 Clear and Exit buttons included for full control

### 💡 How to Use

1. Launch the GUI: `python weather_tkinter_app.py`
2. Use buttons to scrape or update data
3. Enter start and end years to generate a **boxplot**
4. Enter year and month to generate a **line plot**
5. Click the 💬 icon to chat with the **WeatherBot**
   - Type a year (e.g., `2022`) to get mean temperature samples
   - Use `clear` to reset, or `exit` to close the chatbot

---

## 🧠 Chatbot Assistant (`chatbot.py`)

A simple Tkinter-based chatbot that integrates with the main GUI.

- Prompts user for a **year** to fetch weather records
- Displays 5 sample records with **mean temperatures**
- Supports commands: `exit` (close), `clear` (reset)
- Styled using `ScrolledText`, modern fonts, and emoji responses

---

## 🧰 Technologies Used

| Purpose          | Libraries Used                    |
|------------------|-----------------------------------|
| Web Scraping     | `html.parser`, `urllib.request`   |
| Data Storage     | `sqlite3`                         |
| Visualization    | `matplotlib`                      |
| GUI Framework    | `tkinter`, `PIL`, `ttk`, `ScrolledText` |
| Logging          | `logging`                         |

---

## 🗂️ Module Overview

| File                     | Description                                              |
|--------------------------|----------------------------------------------------------|
| `scrape_weather.py`      | Scrapes and parses HTML data from Environment Canada     |
| `db_operations.py`       | Initializes and manages SQLite DB operations             |
| `plot_operations.py`     | Generates boxplots and line plots using matplotlib       |
| `weather_tkinter_app.py` | Tkinter-based GUI interface for users                   |
| `chatbot.py`             | Chatbot interface for year-specific queries              |

---

## 🪪 License

This project is licensed under the **MIT License**. See [LICENSE](./LICENSE) for details.

---

## 🙌 Acknowledgements

Huge thanks to [Environment Canada](https://climate.weather.gc.ca) for their open access to historical climate datasets.

> Designed and developed with 💡 and ❤️ by **Sanchi Madaan**

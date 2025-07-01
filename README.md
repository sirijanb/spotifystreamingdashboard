# 🎧 Spotify Streaming History Dashboard (Excel)

This project analyzes personal Spotify streaming data using **Microsoft Excel** and presents insights through an interactive, visually appealing dashboard. The goal is to uncover listening habits, track preferences, user behavior, and engagement patterns.

---

## 📊 Dashboard Features

The Excel dashboard includes the following KPIs and visualizations:

### 🔹 Key Performance Indicators (KPIs)
- **🎧 Total Listening Time (hrs)**
- **🔁 Shuffle Usage (%)**
- **⏩ Skip Rate (%)**
- **👨‍🎤 Top Artist**
- **🎶 Top Track**
- **💻 Most Used Platform**

### 📈 Visual Charts
- **Daily Listening Trend** (Line chart)
- **Listening by Hour of Day** (Column chart)
- **Top Tracks by Playback Time**
- **Top Artists by Playback Time**
- **Platform Usage Breakdown**
- **Skip vs Non-Skip Analysis (Pie Chart)**

### 🎛️ Interactive Elements
- **Slicers** for filtering data by:
  - Date/Year
  - Platform
  - Weekeday/Weekend

---

## 📂 Data Description

The dataset contains Spotify streaming history with the following fields:

| Field | Description |
|-------|-------------|
| `spotify_track_uri` | Unique Spotify URI |
| `ts` | Timestamp when the track stopped playing (UTC) |
| `platform` | Platform used (mobile, desktop, etc.) |
| `ms_played` | Milliseconds the track was played |
| `track_name` | Track title |
| `artist_name` | Artist name |
| `album_name` | Album name |
| `reason_start` | Why the track started |
| `reason_end` | Why the track ended |
| `shuffle` | Whether shuffle was enabled (TRUE/FALSE) |
| `skipped` | Whether the track was skipped (TRUE/FALSE) |

---

## ⚙️ Methods & Calculations

- **Datetime Handling**: Converted `ts` from UTC to local time using Excel formulas, extracted date, hour, and day of week.
- **Listening Time**: Aggregated `ms_played` into hours for readable KPIs.
- **Pivot Tables**: Used to compute top artists, tracks, platform usage, and behavior metrics.
- **Dynamic Formulas**: Used `GETPIVOTDATA`, `COUNTIF`, `IFERROR`, and `TEXT()` for KPI calculations and safe division.
- **Interactive Slicers**: Enabled filtering across all charts and metrics for deep exploration.

---

## 🧠 Learnings

- Worked with time-series data and UTC conversion in Excel.
- Designed interactive dashboards using PivotTables and slicers.
- Learned how to handle missing or one-sided Boolean values (`shuffle`, `skipped`) gracefully.
- Applied Excel’s data visualization tools to tell a data-driven story.
- Improved skills in using `GETPIVOTDATA`, dynamic labels, and conditional formatting.

---

## 📝 License

This project is for educational and personal use only. Data is sourced from [Maven Analytics](https://mavenanalytics.io/data-playground).

---

If you found this project interesting, feel free to ⭐️ the repo or reach out for collaboration!

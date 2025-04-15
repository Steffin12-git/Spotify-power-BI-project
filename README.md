# Spotify Advanced Data Analysis Project

This repository showcases an end-to-end data analysis project focused on **Spotify streaming behavior**, analyzing user interactions with tracks, albums, and artists. The goal is to extract meaningful insights from listening data and make it easily accessible for visualization tools.

## 📌 Project Objectives

The project explores how users engage with music content on Spotify over time and across different platforms. Key business questions include:

- What are the most played tracks, albums, and artists?
- How does listening behavior vary across weekdays and weekends?
- What is the trend in music engagement over the years?
- When are users most actively listening (hourly patterns)?
- What content do users skip, and what do they play most completely?

---

## 🗂️ Data Overview

| Field Name        | Description |
|-------------------|-------------|
| `spotify_track_uri` | Unique Spotify identifier for each track |
| `ts`               | Timestamp when track stopped playing |
| `platform`         | Device used (desktop, mobile, web, smart speaker) |
| `ms_played`        | Duration (in ms) the track was played |
| `track_name`       | Name of the track |
| `artist_name`      | Performing artist |
| `album_name`       | Album containing the track |
| `reason_start`     | Why the track started (e.g. autoplay, play button) |
| `reason_end`       | Why the track ended (e.g. skipped, completed) |
| `shuffle`          | Whether shuffle mode was enabled |
| `skipped`          | Whether the track was skipped |

---

## 🧠 Analysis Topics

### 🎵 Albums
- Total albums played over time
- Albums played by year (min/max)
- Weekday vs weekend album listening trends
- Top 5 albums by frequency
- Year-over-Year album engagement trends

### 🎤 Artists
- Total artists played over time
- Artist diversity by year
- Weekday vs weekend listening patterns
- Top 5 artists
- LY vs PY and YoY growth for artist engagement

### 🎧 Tracks
- Total track plays over time
- Track diversity by year
- Top 5 tracks by plays
- Skip analysis (via `reason_end` and `skipped`)
- Weekly vs weekend trends

### ⏰ Listening Patterns
- Listening heatmap by hour and weekday
- Average listening time vs track frequency (Quadrant Scatter Plot)

### 📊 Grid View & Interactivity
- Drill-through to detailed data by album, artist, or track
- Grid shows key fields like track name, artist, album, duration
- Exportable to CSV
- Hierarchical drill-down and drill-up support

---

## 🛠️ Tools & Technologies

- **Power BI**: For interactive dashboards and drillthrough views
- **SQL**: For data modeling, cleaning, and transformation
- **Excel/CSV**: Raw data formats
- **DAX**: For metrics like LY vs PY, YoY Growth, engagement scoring

---

## 🚀 How to Use

1. Load the raw Spotify dataset into SQL or Power BI.
2. Use provided SQL scripts to clean and transform the data.
3. Open the Power BI dashboard and connect to the processed data.
4. Explore insights by using filters, drillthrough, and time-based slicers.

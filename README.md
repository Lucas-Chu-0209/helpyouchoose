# ☕ 選擇障礙終結者 (Decision Helper)

A LINE Bot designed to help users quickly decide where to grab a coffee. By combining location-based services, Google APIs, and automated data collection, the bot recommends nearby cafes based on distance and ratings, helping users overcome decision fatigue.

---

## 📌 Project Overview

"選擇障礙終結者" was developed as a project for the Coding 101 Competition.

The goal of this project is to simplify the decision-making process when choosing a café. Users can interact with the LINE Bot and receive personalized recommendations based on their current location and nearby café information.

The system integrates Google Geocoding APIs, web data collection, and recommendation logic to provide users with convenient and practical suggestions.

---

## 🚀 Features

### 1. 咖啡廳輪盤 (Cafe Roulette)

Can't decide where to go?

The bot randomly selects **three nearby cafés** and displays:

* Cafe Name
* Cafe Image
* Google Rating
* Google Maps Link

Users can compare options and make a quick decision.

---

### 2. 隨便啦 (Just Pick One)

For users who really don't want to choose.

The bot automatically selects **one random café** from nearby candidates and immediately returns:

* Cafe Name
* Cafe Image
* Rating
* Google Maps Navigation Link

---

### 3. 附近店家 (Nearest Cafe)

For users who prioritize convenience.

The bot calculates the distance between the user's location and nearby cafés, then recommends the closest option available.

Returned information includes:

* Cafe Name
* Distance
* Rating
* Google Maps Link

---

## 🏗️ System Architecture

User
↓
LINE Bot
↓
Python Backend
↓
Google Geocoding API
↓
Location Processing
↓
Cafe Data Collection
↓
Recommendation Engine
↓
LINE Response

---

## 🛠️ Technologies Used

### Programming Language

* Python

### APIs

* Google Geocoding API

### Deployment

* Heroku

### Libraries

* Flask
* Requests
* BeautifulSoup
* Line Bot SDK

### Data Processing

* JSON
* RESTful API Integration

---

## 🔍 Recommendation Logic

The recommendation engine evaluates nearby cafes using:

* User location
* Geographic distance
* Google ratings

Different recommendation modes apply different weighting strategies:

| Mode          | Selection Strategy             |
| ------------- | ------------------------------ |
| Cafe Roulette | Randomly choose 3 nearby cafes |
| Just Pick One | Randomly choose 1 nearby cafe  |
| Nearest Cafe  | Sort by distance               |

---

## 📈 Challenges & Solutions

### Location-Based Recommendation

Challenge:

Converting user location information into meaningful nearby cafe recommendations.

Solution:

Integrated Google Geocoding API to transform coordinates into searchable geographic information and calculate relative distances.

---

### Data Collection & Processing

Challenge:

Gathering and organizing cafe information from multiple sources.

Solution:

Implemented automated data collection workflows using Python, Requests, and BeautifulSoup, then standardized the results into structured formats for recommendation.

---

### LINE Bot Integration

Challenge:

Providing real-time responses with minimal latency.

Solution:

Deployed the backend service on Heroku and optimized API requests to ensure stable communication between LINE Messaging API and backend services.

---

## 🎯 Key Takeaways

* Backend Development with Python
* API Integration
* Web Scraping
* Location-Based Services
* Recommendation System Design
* Cloud Deployment with Heroku
* LINE Bot Development

---

## 👨‍💻 Author

Lucas Chu

Coding 101 Finalist Project



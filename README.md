# Recipe Suggestion Microservice

A Flask microservice that suggests recipes based on ingredients you have.

**Purpose:** Learning Flask and API integration with heavy AI assistance.

![Image unavailbe](result.png)

## What It Does

Enter ingredients you have, get recipe suggestions ranked by how many 
of your ingredients they use.

## How It Works

1. User enters ingredients (e.g., "egg, cheese, milk")
2. System checks local recipe database
3. System queries Spoonacular API for more recipes
4. Returns ranked results by ingredient match percentage
5. Shows which ingredients matched and which are missing

## What I Learned

### 1. Flask Basics
- How to create routes and handle requests
- Serving HTML templates
- Basic request/response handling

### 2. API Integration
- How to call external APIs (Spoonacular)
- Handling API responses
- Graceful fallback when API is unavailable

### 3. Matching Algorithm
- Percentage-based scoring (not just counting matches)
- Why "recipes using 1 of 8 ingredients" shouldn't rank high
- Adaptive thresholds based on input size

## About This Project

**My role:** Came up with the idea, guided the direction

**AI role:** Built most of the code

**My understanding:** I understand the overall flow and main concepts 
(Flask routes, API calls, matching logic). Some parts I'm less clear on.

**Note:** I relied too heavily on AI for this one - it was a learning 
experience about balancing AI help with actually coding myself.

## Tech Stack

- Flask (Python backend)
- Spoonacular API (external recipes)
- HTML/CSS/JavaScript (frontend)

## How to Run
```bash
pip install -r requirements.txt
python main.py
# Visit http://localhost:5000/interface
```

## Limitations

- Limited local recipe database (just for testing)
- Matching algorithm is basic (percentage-based only)
- No user preferences or learning
- Depends on Spoonacular API availability

## What I'd Do Differently

If I built this again, I would:
- Code more of it myself instead of relying on AI
- Better understand each decision before implementing
- Start with a clearer architecture plan
- Document my own learning as I went




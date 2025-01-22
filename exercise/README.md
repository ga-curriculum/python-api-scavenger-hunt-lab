<h1>
  <span class="headline">Python API Scavenger Hunt Lab</span>
  <span class="subhead">Exercise</span>
</h1>

## Overview

Welcome to the Python API Scavenger Hunt Lab! In this lab, you'll work collaboratively in groups to explore various public APIs and answer challenge questions using data retrieved from these APIs. This hands-on experience will enhance your skills in making HTTP requests, parsing responses, and integrating API data into your applications.

## Objectives

- Practice making HTTP requests using Python's requests library.
- Explore and interact with a variety of public APIs.
- Parse and handle different types of API responses (JSON, XML, etc.).
- Collaborate with peers to solve challenges using API data.
- Enhance problem-solving skills by integrating data into practical applications

## Instructions

Use any API from the list provided below to answer as many of the challenge questions as possible. Many of these APIs are open and do not require additional signups.

- [Public APIs](https://github.com/public-apis/public-apis)

## Getting Started

Follow these steps to begin the API Scavenger Hunt Lab:

### 1. Install requests Library:

Ensure you have the requests library installed to your pip modules. You can install it using `pip` Python command:

```bash
pip install requests
```

### 2. Choose an API:

Browse the [Public APIs Repository](https://github.com/public-apis/public-apis) and select an API that interests you or that you think will help answer one of the challenge questions.

### 3. Make Your First Request:

In your lab directory, inside `main.py` use `requests.get()` to make a simple HTTP GET request to the API's endpoint.

```python
import requests

address = '<your-api-endpoint>'
timeout = '10'
response = requests.get(address, timeout)

response = requests.get(address)

if response.status_code == 200:
    data = response.json()
    print(data)
else:
    print(f"Error {response.status_code}: {response.reason} for {response.url}")

```

## 4. Handle API Responses:

- Examine the structure of the API response (ex: JSON, XML).
- Use Python to parse the response and extract the data needed.
- Handle exceptions and errors gracefully.

## 5. Challenges

Work together with your group to solve as many of the following challenges as you can. Use the data retrieved from the APIs to answer the questions.

Challenge 1: London Underground

- Find real-time data on all the active tube lines in the London Underground.

Challenge 2: International Space Station Position

- Find the current position (latitude and longitude) of the International Space Station (ISS)

Challenge 3: Word Definitions

- What does "epistemology" mean? Use a dictionary API to display the definition.

Challenge 4: Pokémon Abilities

- Find and print all of Pikachu's abilities.

Challenge 5: Crypto Prices

- Find the current price of Bitcoin in your local currency.

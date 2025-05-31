# 🎬 TMDB PROJECT - Postman Collection

This repository contains a **Postman collection** with basic test cases and request examples for working with **The Movie Database (TMDB)** API.

## 🧪 Contents

- ✅ **Postman collection file**  
- 🧾 **Test scenarios**  
- ⚠️ **Possible error codes and their explanations**  
- 🔑 **Steps to obtain a TMDB API Key**

---

## 🚀 Getting Started

### 1. Create a TMDB Account & Get API Key

1. Visit [https://www.themoviedb.org/](https://www.themoviedb.org/)
2. Click on the **"Join TMDB"** button and fill out the registration form.
3. Verify your email address.
4. After logging in, go to your profile and click the **"API"** tab.
5. Under the "Request an API Key" section, select **Developer** type and complete the request form.
6. You will receive your **API Key** and **Read Access Token**.

➡️ [See the full API key registration instructions (PDF)](TMDB%20Login%20and%20API%20Key.pdf)

---

### 2. How to Use the Postman Collection

1. Open the Postman app.
2. Go to `File > Import` and select the `TMDB Project.postman_collection.json` file from this repository.
3. Insert your **own API key**, **access token**, and other required parameters to run the tests.

---

## ✅ Key Test Scenarios

| No | Test Case                     | Endpoint                                                  | Method |
|----|-------------------------------|------------------------------------------------------------|--------|
| 1  | Valid Login                   | `POST /login`                                              | POST   |
| 2  | Invalid Login                 | `POST /login`                                              | POST   |
| 3  | Get Account Details           | `/account`                                                 | GET    |
| 4  | Add Movie to Favorites        | `/account/{account_id}/favorite`                           | POST   |
| 5  | Get Favorite Movies           | `/account/{account_id}/favorite/movies`                    | GET    |
| 6  | Get Watchlist Movies          | `/account/{account_id}/watchlist/movies`                   | GET    |
| 7  | Get Movie Genres              | `/genre/movie/list`                                        | GET    |
| 8  | Get Now Playing Movies        | `/movie/now_playing`                                       | GET    |
| 9  | Get Popular Movies            | `/movie/popular`                                           | GET    |
| 10 | Add Movie Rating              | `/movie/{movie_id}/rating`                                 | POST   |
| 11 | Delete Movie Rating           | `/movie/{movie_id}/rating`                                 | DELETE |
| 12 | Unauthorized Access (Test)    | `/list/{list_id}/add_item?session_id=INVALID`              | POST   |


---

## ⚠️ Common TMDB Error Codes

| Code | HTTP | Message                                             |
|------|------|------------------------------------------------------|
| 7    | 401  | Authentication failed: Invalid API key              |
| 3    | 401  | Permission denied                                    |
| 5    | 422  | Invalid parameters                                   |
| 34   | 404  | Resource not found                                   |
| 25   | 429  | Rate limit exceeded                                  |
| 11   | 500  | Internal server error                                |

➡️ [See the complete error code list (PDF)](TMDB%20Errors%20Code.pdf)

---
## 👥 Contributors

| 👤 Name | 🛠️ Role |
|:--------|:--------|
| [Baris Saydam](https://github.com/BarisSaydam) | QA Tester |
| [Diyar Olmez](https://github.com/diyarolmezz) | QA Tester |
| [Erdem Ozkan](https://github.com/ErdemOzkann) | QA Tester |
| [Omer Boncuk](https://github.com/palanque92) | QA Tester |
| [Atilla Toros Avci](https://github.com/AtillaTorosAvci) | QA Tester |
| [Gamze Batmaz](https://github.com/GAMZE3845) | QA Tester |

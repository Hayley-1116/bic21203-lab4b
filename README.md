# BIC21203 Lab 4b – Client-Side Scripting (JSON and jQuery)

**Name:** Cheah Tian Xin
**Student ID:** AI240180

## Overview
This lab uses JSON, the native `fetch()` API and jQuery.
- **Q1:** `books.json` – a valid JSON dataset with a top-level `books` array of two book objects.
- **Q2:** `books.html` – loads `books.json` with `fetch()` and displays the first book's title, the second book's author and the genres of both books. It shows a friendly error message if loading fails.
- **Q3:** `jquery-dom.html` – uses jQuery 4.0.0 (`.text()`, `.addClass()`, `.on("click", ...)`) to do the same DOM tasks as native JavaScript.

## Files
| File | Description |
|------|-------------|
| `books.json` | Book data (title, author, publicationYear, genres) |
| `books.html` | Fetches and displays the JSON data |
| `jquery-dom.html` | jQuery equivalents of three DOM operations |
| `screenshots/` | Output screenshots |

## Setup and how to run
1. Clone or download this repository.
2. **Q1:** Open `books.json` in a code editor to view it.
3. **Q2:** `fetch()` needs a local server, so do not open the file by double-clicking.
   - In VS Code, install the **Live Server** extension, right-click `books.html` and choose **Open with Live Server**.
   - Or run `python -m http.server` in the folder and open `http://localhost:8000/books.html`.
4. **Q3:** Open `jquery-dom.html` in a browser. It needs an internet connection to load jQuery from the CDN.

## Screenshots
### Q1 – books.json
![books.json]<img width="410" height="252" alt="Screenshot 2026-11-17 111219" src="https://github.com/user-attachments/assets/e702c7a7-ae23-4031-ab91-3ed584f677c1" />


### Q2 – books.html output
![Q2 output]<img width="347" height="230" alt="Screenshot 2026-11-17 110709" src="https://github.com/user-attachments/assets/8b9240bc-200b-482c-ba84-6c6f8ad15b0b" />

Error handling (when `books.json` cannot be loaded):
![Q2 error]<img width="267" height="131" alt="Screenshot 2026-11-17 110145" src="https://github.com/user-attachments/assets/7c28db5a-c48f-4e63-a715-4598c7c2fa0d" />

### Q3 – jquery-dom.html
![Q3 output]<img width="248" height="284" alt="Screenshot 2026-11-17 110728" src="https://github.com/user-attachments/assets/803d7755-91ba-41dd-bc66-2168e0447d5b" />
<img width="422" height="216" alt="Screenshot 2026-11-17 110734" src="https://github.com/user-attachments/assets/b388d1ce-9af9-404b-80b5-98c63f1f41f8" />

## Native JavaScript vs jQuery
- **Advantage of native JavaScript:** no extra library to download, so the page loads faster and has fewer dependencies.
- **Why a project may still use jQuery:** older projects and plugins already depend on it, and rewriting them would cost more than it gains.

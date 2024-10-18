# Jina AI Reader

## Reader_Jina.py
This Python script is designed to take input as either a URL or a search query. Depending on the input type, it performs one of two operations:

- **URL Input**: If the user provides a URL, the script fetches the content of the page and stores it in a text file (`response.txt`).
- **Search Query Input**: If the user provides a search query, the script returns the top search results along with their content, and stores the results in a JSON file (`response.json`).

1. The script prompts the user to choose between two modes:
   - `'r'` for reading a URL.
   - `'s'` for searching a query.

2. Based on the user's choice:
   - If the user selects `'r'`, they are prompted to enter a URL. The script then fetches the page content using the Jina AI API and stores the raw HTML content in a file called `response.txt`.
   - If the user selects `'s'`, they are prompted to enter a search query. The script sends the query to the Jina AI API and stores the search results and their respective page contents in `response.json` in a structured format.

### Output Files
-`response.txt`: Contains the HTML content of the page fetched from the provided URL.
-`response.json`: Contains the top search results and content in a JSON format based on the search query.


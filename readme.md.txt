Approach:
- I used Google Colab to process 147 URLs from Input.xlsx.
- Scraped each URL’s title and text using BeautifulSoup, saving them as individual .txt files named by URL_ID.
- Analyzed each text file for 13 metrics (e.g., positive/negative scores, readability) using NLTK and custom word lists from StopWords and MasterDictionary.
- Combined results into output.csv with URL_ID, URL, and all metrics.

How to Run the .py File:
1. Open Google Colab at colab.research.google.com and create a new notebook.
2. Upload three files to Colab: Input.xlsx, StopWords-20250325T135103Z-001.zip, and MasterDictionary-20250325T135116Z-001.zip.
3. Unzip the folders by running these commands in a cell:
   !unzip /content/StopWords-20250325T135103Z-001.zip -d /content/
   !unzip /content/MasterDictionary-20250325T135116Z-001.zip -d /content/
4. Upload solution.py to Colab via the Files sidebar (click the folder icon, then the upload button).
5. Open solution.py in Colab, then click the play button (or press Ctrl+Enter) to run it.
6. After it finishes, download output.csv from the Files sidebar.

Dependencies:
- Pre-installed in Colab: pandas, requests
- Installed by the script: beautifulsoup4, nltk
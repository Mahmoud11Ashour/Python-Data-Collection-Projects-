# Python Data Collection Portfolio

Three practical Python data-collection and preparation projects, illustrating work with a public dataset, web scraping, and an API. The examples include source scripts, Jupyter notebooks, and sample data outputs.

## Projects

| Project | Data source | Main tools | Dataset size |
| --- | --- | --- | ---: |
| [IMDb Dataset Preparation](01-IMDb-Dataset-Preparation/) | Existing IMDb movie CSV dataset | Python, Pandas, NumPy, scikit-learn | 1,000 movie records |
| [Noon Web Scraping](02-Noon-Web-Scraping/) | Noon e-commerce product pages | Python, Requests, BeautifulSoup, Pandas | 1,000 raw product records; 989 processed records |
| [Reddit API Collection](03-Reddit-API-Collection/) | r/programming via Reddit API | Python, PRAW, Pandas | 750 post records in the original analysis |

## What these projects demonstrate

- Collecting structured information from public data files, HTML pages, and APIs.
- Inspecting, cleaning and transforming data with Pandas and NumPy.
- Handling missing values and preparing data for analysis.
- Exporting analysis outputs to CSV.
- Basic exploratory analysis and visualizations.

## Repository contents

Each project has a `.py` script and a `.ipynb` notebook. IMDb and Noon examples also include input/output CSV files. The Reddit example includes an anonymized metrics-only CSV; post text, account names, IDs and URLs are intentionally excluded from this public portfolio copy.

## Running the notebooks or scripts

1. Install Python 3 and packages: `python -m pip install -r requirements.txt`.
2. Open the desired project folder and run the corresponding Python script or Jupyter notebook from that folder (for example, `cd 02-Noon-Web-Scraping` then `python dataset2.py`).
3. For the Reddit collector, configure the `REDDIT_CLIENT_ID` and `REDDIT_CLIENT_SECRET` environment variables locally and optionally set `REDDIT_USER_AGENT`. Never commit those values.

**Notes:** The source files were originally written for Google Colab and their file paths have been adapted to be relative for this portfolio copy. Web scraping depends on the website's current structure and permission/rate limits; selectors may need updates if the site changes. The code has been syntax-checked but live website and API requests have not been re-run in this environment. The IMDb dataset's original hosting URL is not documented in the supplied project materials.

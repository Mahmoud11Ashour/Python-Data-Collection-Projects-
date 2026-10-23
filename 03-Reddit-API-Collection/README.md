# Reddit Data Collection with PRAW

- **Data source:** Reddit API, including an analysis of posts from `r/programming`.
- **Code:** `dataset3.py` and `DataSet3.ipynb`.
- **Tools:** PRAW, Pandas, NumPy.
- **Original data size:** 750 Reddit post records in the supplied project output.
- **Public demo data:** `reddit_posts_anonymized_metrics.csv` (750 rows). This intentionally omits post texts, usernames, IDs, URLs, and titles.

## API configuration

Create your own Reddit API application/credentials (subject to Reddit developer terms) and provide them using environment variables on your own device:

- `REDDIT_CLIENT_ID`
- `REDDIT_CLIENT_SECRET`
- `REDDIT_USER_AGENT` (optional)

For example, in a PowerShell terminal:

```powershell
$env:REDDIT_CLIENT_ID = 'your-client-id'
$env:REDDIT_CLIENT_SECRET = 'your-client-secret'
$env:REDDIT_USER_AGENT = 'data-collection-portfolio/1.0'
python dataset3.py
```

Do not put real API credentials into source files, notebooks, or GitHub. The portfolio code has been sanitized; the original supplied archive was not modified. API behavior and policy can change over time.

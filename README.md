# Traffic Accident Analytics Dashboard

A deployable Streamlit dashboard for the Big Data Traffic Accident Analysis project.

## Run locally
1. Install Python 3.10+.
2. Open a terminal in this folder.
3. Install dependencies:
   `pip install -r requirements.txt`
4. Start the dashboard:
   `streamlit run app.py`
5. Open the local URL printed in the terminal (usually http://localhost:8501).

## Host online with Streamlit Community Cloud
1. Create a GitHub repository and upload `app.py` and `requirements.txt`.
2. Go to https://share.streamlit.io/ and sign in with GitHub.
3. Select **Create app**, choose your repository, branch, and `app.py`.
4. Click **Deploy**. Streamlit will install packages from `requirements.txt`.
5. The app fetches the public NYC Open Data API at runtime; it needs outbound internet access.

## Data source
NYC Open Data — Motor Vehicle Collisions (Crashes):
https://data.cityofnewyork.us/resource/h9gi-nx95.json

## Notes
- This is a dashboard front end using pandas for interactive display. The companion notebook demonstrates PySpark and MapReduce analysis.
- It downloads a configurable sample (5,000–50,000 records), caches it for one hour, and lets users filter boroughs and reported contributing factors.
- The dashboard uses NYC data and should not be presented as a national traffic accident dataset.
- A dashboard/API request can fail temporarily; use the refresh button to retry.

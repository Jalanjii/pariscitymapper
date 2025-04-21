# citymapper

A citymapper-like app for Paris transportation system developed with Jean-Philipp MAMBILA.

![app screenshot](.\app_icon\parismap.png)

## Setup


- Make sure to install the necessary Python packages: `pip install -r requirements.txt`
- Set up your Postgres server, include your username, password, database name (postgres by default), and host (localhost by default) in the `\modules\params.json`
- Run the parser inside the `parse` directory: `python parse.py`
- Run the main program: `python main.py`


## Data Reference 

https://www.nature.com/articles/sdata201889#Tab5


git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch ' \data\network_temporal_day.csv
  --prune-empty --tag-name-filter cat -- --all
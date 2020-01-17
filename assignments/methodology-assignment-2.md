# Methodology Assignment 2

## Data Ingestion

### Due Friday Jan 24 11:59 PM

Using a configuration file, you will scrape [NFL football team
schedule tables](https://www.pro-football-reference.com/teams/sdg/2016.htm) from various years, and save them to a data folder. We are interested in the second table of these web pages.

To download tables for the San Diego Chargers in 2014,
2015, 2016, your configuration file can look like:

```
{
    "teams": ["sdg"],
    "years": [2014, 2015, 2016]
}
```

Turn in:
- a 'data-params.json' configuration file for the 49ers ('sfo') and Packers ('gnb') between 2012 and 2019 (inclusive)
- 'get_data.py' that, using your configuration file, saves the schedule tables to a data folder

You may find the following functions useful:
  - `pd.read_html`
  - `json.load`
  - `os.mkdir`
  - `os.path.exists`

You will not be getting starter code for this HW, however, the Gradescope assignments will run visible tests to check the basics of your work.

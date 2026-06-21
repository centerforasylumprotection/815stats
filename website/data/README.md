# Data sources

Data sources are CSV files that must be pulled manually. Go to the [UNHCR Refugee Data Finder](https://www.unhcr.org/refugee-statistics) and download the following:

## Download new data
### Population

- **Dataset group**: Forced displacement
- **Dataset**: Population figures
- **Display type**: Totals
- **Population figures**: All
- **Year** 1951-latest (drag the sliders to the left and right)
- **Country of Origin**: All countries
- **Country of Asylum**: Thailand

The click `Download` > `Query data`. You get a file, `download.zip`, which contains `persons_of_concern.csv`. Upload this to `centerforasylumprotection/815stats/website/data/`.

### Asylum applications

- **Dataset group**: Forced displacement
- **Dataset**: Population figures
- **Population figures**: All
- **Year** 1951-latest (drag the sliders to the left and right)
- **Country of Origin**: All countries
- **Country of Asylum**: Thailand

The click `Download` > `Query data`. You get a file, `download.zip`, which contains `asylum_applications.csv`. Upload this to `centerforasylumprotection/815stats/website/data/`.

### Asylum decisions

- **Dataset group**: Forced displacement
- **Dataset**: Population figures
- **Population figures**: All
- **Year** 1951-latest (drag the sliders to the left and right)
- **Country of Origin**: All countries
- **Country of Asylum**: Thailand

The click `Download` > `Query data`. You get a file, `download.zip`, which contains `asylum_decisions.csv`. Upload this to `centerforasylumprotection/815stats/website/data/`.

### UNHCR-assisted refugee resettlement submissions 

- **Dataset group**: Solutions
- **Dataset**: UNHCR-assisted refugee resettlement submissions
- **Display type**: Totals
- **Population figures**: All
- **Year** 2003-latest (you have to manually select years)
- **Country of Origin**: All countries
- **Country of Asylum**: Thailand

The click `Download` > `Query data`. You get a file, `download.zip`, which contains `solutions_submissions.csv`. Upload this to `centerforasylumprotection/815stats/website/data/`.

### UNHCR-assisted refugee resettlement departures 

- **Dataset group**: Solutions
- **Dataset**: UNHCR-assisted refugee resettlement departures
- **Display type**: Totals
- **Population figures**: All
- **Year** 2003-latest (you have to manually select years)
- **Country of Origin**: All countries
- **Country of Asylum**: Thailand

The click `Download` > `Query data`. You get a file, `download.zip`, which contains `solutions_submissions.csv`. Upload this to `centerforasylumprotection/815stats/website/data/`.

## Updating data
Updating data consists in replacing the current CSV files with the ones you have downloaded. Do the following:

- Navigate to `centerforasylumprotection/815stats/website/data/`.
- Click `Add file` > `Upload files` in the upper-right corner above the file list.
- Drag and drop the files onto the page or select them with `choose your files`.
- Under **Commit changes**, add today's date in format `YYYY-MM-DD` and write a short message - e.g., `2027-06-20 - full-year statistics for 2026 available.`
- Click `Commit changes`.

Wait a few minutes, and go to [815stats](https://815stats.capthailand.org). You may have to force-reload the page with `CTRL`+`R` to see the updated figures.

## Update message in app

The app includes a "last updated" message which is added manually:
- Go to `centerforasylumprotection/815stats/website/`.
- Open `config.yaml`.
- Click the `Edit this file` icon - the **pen** in the upper-right corner.
- Find the **subtitle** key on line 19.
- Write a message that explains when you last updated the data and what period they cover:

**For example**
```
  subtitle: "Last updated: 21 June 2026. Figures are correct until the end of 2025."
```

*Please note: The two spaces in front of `  subtitle` are **very** important; without them the message will not be shown.*

Save the file by clicking `Commit changes` at the top of file and again `Commit changes` to save.


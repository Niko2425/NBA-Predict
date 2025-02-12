go to this directory in cmd prompt
type wsl
jupyter lab
done. (you need wsl to be able to use the playwright scraping library)

to scrape more data for current 2025 szn:

1. go to data>standings and delete any months you're ovewriting (i.e. if you last on feb 2nd, delete nba_2025_games-feb file to ovewrrite it with new results)

2. go into get_data.ipynb: run everything (it'll skip files that already exist)

3. go into parse_data.ipynb: run everything (it'll load current nba_games.csv, add in new games that have occured since last time you ran, and save again as nba_games.csv)

4. Can run predict.ipynb to get new predictions, don't need to re-run get_future_games unless new season since i just cut off by current date in predict file
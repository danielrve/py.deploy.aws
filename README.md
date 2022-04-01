# What the repo do

**Simple ETL process** for pulling game stats from the NHL website and then shaping the results in a database deploy in AWS S3 environment.

Garnering data for NHL API to have Game Scores

You should be able to follow the [Makefile] if your environment doesn't quite match.

Mostly Working Code -- given the run steps, the code should download data, format it, load it into the db and the final data marts be queryable.

**make step1** -- runs docker images in the foreground for convenience

Posgree Database Image
Min.io AWS S3 Emulator

**make step2** points_leaders -- loads and shapes data then queries the results. This should just print out the top 10 points leaders.

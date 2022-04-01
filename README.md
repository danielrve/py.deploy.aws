# What the repo do

**Simple ETL process** for pulling game stats from the NHL website and then shaping the results in a database deploy in AWS S3 environment.

Garnering data for NHL API to have Game Scores

You should be able to follow the [Makefile] if your environment doesn't quite match.

Mostly Working Code -- given the run steps, the code should download data, format it, load it into the db and the final data marts be queryable.

**make step1** -- runs docker images in the foreground for convenience

* **Posgree** Database Image
* **Min.io** AWS S3 Emulator using **BOTO3** and **awscli**

**make step2** points_leaders -- loads and shapes data then queries the results. This should just print out the top 10 points leaders.


## Prerequisites
We use Mac OS for development so if you have one and do any kind of development on it, you're probably good. Linux environments should work too, this was tested on an Ubuntu machine. Windows users will need to establish a complete workflow. (Sorry)

* Docker -- native for linux, Desktop for Mac and windows users
* docker-compose -- comes with desktop. Linux users may need an extra install.
* a functioning make -- if you don't/can't use this, the make file is just wrapping the steps necessary to run the code and should be easy to disect to run manually
* Python 3.7+ with a virtualenv -- This example won't create the virtualenv for you, but will help you install dependencies

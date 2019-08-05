# Log Analysis

## Prerequisites

1. `docker`
2. `docker-compose`

## To RUN:

1. Clone this repo: `git clone https://github.com/albertoivo/docker-fullstacknd.git`

2. Enter the directory: `cd log-analysis-docker-fullstacknd`

3. Run `docker-compose up`

It may take a while the first time because it will download an PostgreSQL image. But that's all! You will have a postgreSQL container populated with thousands of registers.

You should connect like the example below:
```python
psycopg2.connect(dbname='news', user='vagrant', host='localhost')
```

## To STOP:

1. `ctrl + z` - Puts the process in background (you can skip this step if you open another terminal window).
2. `docker-compose down` - Stops the container and image and removes the volumes created by `docker-compose up`.

To stop the docker it's important to run `docker-compose down` so it will drop the database and create a new one next time you run. It's important so we know the database is always new for every review.

**Never** stop the container with `ctrl + c`.

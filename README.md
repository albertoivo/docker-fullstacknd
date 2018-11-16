## Prerequisites

`docker` and `docker-compose`

## To RUN:

1. Clone this repo: `git https://github.com/albertoivo/log-analysis-docker-fullstacknd.git`

2. Enter the directory: `cd log-analysis-docker-fullstacknd`

3. Run `docker-compose up`

It ay take a while the first time because it will download an PostgreSQL image. But that's all! You will have a postgreSQL container with user=vagrant and a database=news populated with thousands of registers.

## To STOP:

1. `ctrol + z` - to put the process in backgroung (you can skip this step if you open another terminal windown)
2. `docker-compose down`

To stop the docker it's important to run `docker-compose down` so it will drop the database and create a new one next time you run. It's important so we know the database is always new for every review.

**Never** stop the container with `ctrl + c`.

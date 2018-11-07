# log-analysis-docker-fullstacknd


## To RUN:

If you downloaded `docker-compose.yml` and `newsdata.sql.gz`. You only need to run `docker-compose up`

But if you have only the `docker-compose.yml`, you should run these 3 following steps:

1 - Download `newsdata.zip` [here](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip) and extract in the same directory.

2 - Run `docker-compose up`

3 - In another terminal window (but inside the project directory), run `docker exec -i udacity-log-analysis psql -U vagrant -d news < newsdata.sql`


## To STOP:

To stop the docker it's important to run `docker-compose down` so it will drop the database and create a new one next time you run. It's important so we know the database is new for every review.

Never stop the container with `ctrl + c`. Only with `docker-compose down`.

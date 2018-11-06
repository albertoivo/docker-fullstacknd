# log-analysis-docker-fullstacknd

1 - Download `newsdata.zip` [here](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip) and extract in the same directory.

2 - Run `docker-compose up`

3 - In another terminal window, run `docker exec -i udacity-log-analysis psql -U vagrant -d news < newsdata.sql`

Obs.: To stop the docker it's important to run `docker-compose down`

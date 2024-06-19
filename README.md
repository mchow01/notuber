# Overview
* A ride sharing-clone written in Node.js + Express + MongoDB
* Warning: ~~potentially~~ vulnerable 😀

# To Run
1. `docker compose build`
2. `docker compose up`
3. Open up http://localhost:3000 to see web front end
4. Insert data via `curl` to HTTP POST route `/rides` (e.g., `curl --data "username=Encore&lat=36.126492&lng=-115.165741" http://localhost:3000/rides`)

# Documentation and References
* Need to downgrade mongo container to be under version 5: "WARNING: MongoDB 5.0+ requires a CPU with AVX support, and your current system does not appear to have that!"
* Now using `mongo` module, latest. No longer version 2.x.x. https://expressjs.com/en/guide/database-integration.html#mongodb
* "Dockerizing a Node.js web app" https://nodejs.org/de/docs/guides/nodejs-docker-webapp/

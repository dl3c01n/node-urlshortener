# Files 

**server.js** : Entry point of the app.

**views/index.ejs** : EJS formatter (like public/index.html in React)

**models/shortUrl.js** : Model of shortUrl to insert in mongodb.

**database/** : Connect to mongoDB atlas (cloud mongo database)

**Dockerfile** : Build the image and run the container


## How to run the projet ?

```$ npm i```

```$ npm start``` (using nodemon to update when saving modifications)

## How to build image and run container ?

- Install [Docker Desktop](https://www.docker.com/products/docker-desktop)

- Run ```docker build . -t {your-docker-username}/shortener```

- Run ```docker run -p 5050:5050 -d {your-docker-username}/shortener```

- Navigate to [localhost:5050](http://localhost:5050)

## Using this app as a Docker Image


- Run ```docker pull dl3c01n/shortener:latest```

- Run ```docker run -p 5050:5050 -d dl3c01n/shortener```

- Navigate to [localhost:5050](http://localhost:5050)
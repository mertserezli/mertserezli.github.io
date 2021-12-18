---
layout: post
title: Weather App Cache Update
categories: [Project]
---
Recently I added caching to my weather. It was simple. All I had to do was create a server to do the requests to the weather api and cache the result into redis db. Now the webapp does requests to my server instead of weather api. I am hosting the server on heroku. 

I tried to use the redis npm package but I couldn't make it work because to connect a redis server it requires both username and password but I only got password for it. I used redislabs's redis and they don't give username or I couldn't find it. So I used tedis to connect to it. 

Probably OpenWeather already does some caching in its side. I did this just to learn about caching and redis. 

I watched this tutorial: [https://youtu.be/jgpVdJB2sKQ](https://youtu.be/jgpVdJB2sKQ)  
Server repository: [https://github.com/mertserezli/weather-react-server](https://github.com/mertserezli/weather-react-server)  
Web app repository: [https://github.com/mertserezli/weather-react](https://github.com/mertserezli/weather-react)  
site url: [https://sharp-saha-8ae25a.netlify.app/](https://sharp-saha-8ae25a.netlify.app/)

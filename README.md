# netcoreapp
A sample dot net core app to experiment stuff.


docker build . -t rvtest:latest
docker run -it -p 8080:80 -e ASPNETCORE_ENVIRONMENT=Development  rvtest:latest

docker build --pull --rm -f "Dockerfile" -t netcoreapp:1.0 "."


docker compose up -d        

docker compose up -d --no-deps --build web


docker login -u rahulvermaforu
enter password (access token password from from docker hub)

docker push rahulvermaforu/netcoreapp:latest
docker push rahulvermaforu/netcoreapp:1.0

http://localhost:8080/swagger/index.html
http://localhost:8080/WeatherForecast
curl -X GET "http://localhost:8080/WeatherForecast" -H  "accept: text/plain"
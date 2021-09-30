# netcoreapp
A sample dot net core app to experiment stuff.


docker build . -t rvtest:latest

docker run -it -p 8080:80 -e ASPNETCORE_ENVIRONMENT=Development  rvtest:latest



docker compose up -d        

docker compose up -d --no-deps --build web:80
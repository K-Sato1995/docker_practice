# README

# Great resources to learn docker

- (Docker 101: Fundamentals & The Dockerfile)[https://medium.com/@paigen11/docker-101-fundamentals-the-dockerfile-b33b59d0f14b]
- (Docker 102: Docker-Compose)[https://medium.com/@paigen11/docker-102-docker-compose-6bec46f18a0e]
- (Developing a Ruby on Rails app with Docker Compose)[https://medium.com/firehydrant-io/developing-a-ruby-on-rails-app-with-docker-compose-d75b20334634]


## To start developing rails applications, you can simply follow the steps below.
※ I made the following steps based on (Developing a Ruby on Rails app with Docker Compose)[https://medium.com/firehydrant-io/developing-a-ruby-on-rails-app-with-docker-compose-d75b20334634]
.

 ```
 docker-compose build web
 docker-compose run web rails new --database=postgresql -J --skip-coffee .
 docker-compose run web rails g model Post
 docker-compose run web rails g controller posts
 docker-compose run --rm web rails db:create db:migrate
docker-compose up web
 ```

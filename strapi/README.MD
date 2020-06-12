docker run -it -p 1337:1337 -v `pwd`/project-name:/srv/app strapi/strapi


docker run -it \
  -e DATABASE_CLIENT=postgres \
  -e DATABASE_NAME=strapi \
  -e DATABASE_HOST=0.0.0.0 \
  -e DATABASE_PORT=5432 \
  -e DATABASE_USERNAME=strapi \
  -e DATABASE_PASSWORD=strapi \
  -p 1337:1337 \
  -v `pwd`/project-name:/srv/app \
  strapi/strapi


  for heroku 

  https://strapi.io/documentation/3.0.0-beta.x/deployment/heroku.html

  https://github.com/strapi/strapi-heroku-template

  https://github.com/strapi/strapi-heroku-cms-demo

  https://we2api.herokuapp.com/
  https://we2api.herokuapp.com/admin/



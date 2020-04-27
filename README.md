# Simple RoR REST API

This application makes RoR REST API

--api  give sove extra tools in app which you need for api
rails new simpleRoRRestAPI --api 

Use POSTMAN to check requests:

* check all articles
POSTMAN: GET postman http://localhost:3000/api/v1/articles

* check a particular article
POSTMAN:GET http://localhost:3000/api/v1/articles/1

* Create an article
POSTMAN POST http://localhost:3000/api/v1/articles/
Headers: Content-type application/json
Body(raw):
{
	"title": "Some title",
	"body":  "Some body"
}

* Update an article
POSTMAN PATCH http://localhost:3000/api/v1/articles/5
Headers: Content-type application/json
Body(raw):
{
	"title": "New title",
	"body":  ""
}

* Delete an article
POSTMAN DELETE http://localhost:3000/api/v1/articles/5

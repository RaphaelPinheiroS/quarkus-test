# quarkus-test

To Start Application:

`./mvnw clean compile quarkus:dev`

**Once Application Starts**

API Documentation is Available at:
http://localhost:8081/swagger-ui/


To List People:

`curl "http://localhost:8081/person"
      -H 'Content-Type: application/json'
`

To Add a Person:

`curl -X "POST" "http://localhost:8081/person" \
      -H 'Content-Type: application/json' \
      -d $'{
   "name": "Raphael",
   "addresses": [
     {
       "state": "SP",
       "country": "Brazil",
       "address1": "Avenida Paulista 2020"
     }
   ]
 }'`
 
 Get Person's Details:
 
 `
  curl "http://localhost:8081/person/1" 
       -H 'Content-Type: application/json'
`
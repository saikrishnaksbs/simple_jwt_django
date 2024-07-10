
CURD OPERATIONS

curl -X POST -H "Content-Type: application/json" -d '{"username": "testuser", "email": "testuser@ample.com", "password": "testpassword"}' http://127.0.0.1:8000/api/register/
curl -X POST -H "Content-Type: application/json" -d '{"email": "testuser@ample.com", "password": "testpassword"}' http://127.0.0.1:8000/api/login/
curl -X GET -H "Authorization: Bearer Token" http://127.0.0.1:8000/api/items/
curl -X GET -H "Authorization: Bearer Token" http://127.0.0.1:8000/api/user/ 
curl -X POST -H "Authorization: Bearer Token" -H "Content-Type: application/json" -d '{"name":"NewItem", "description": "New item description"}' http://127.0.0.1:8000/api/items/create/
curl -X PUT -H "Authorization: Bearer Token" -H "Content-Type: application/json" -d '{"name": "UpdatedItem", "description": "Updated item description"}' http://127.0.0.1:8000/api/items/update/1/
curl -X DELETE -H "Authorization: Bearer Token" http://127.0.0.1:8000/api/items/delete/1/

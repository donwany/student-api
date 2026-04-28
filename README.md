```bash

# Insert records
curl -X POST http://localhost:8000/v1/students \
-H "Content-Type: application/json" \
-d '{"name":"Alice","age":23,"course":"AI"}'

# GET Student by ID
curl -X GET 'http://localhost:8000/v1/students/69f11c84b9ac80396d2807a5' \
--header 'Content-Type: application/json' \
--data '{
    "name":"John",
    "age":99,
    "course":"AML"
}'

# Update Student
curl -X PUT 'http://localhost:8000/v1/students/69f11c84b9ac80396d2807a5' \
--header 'Content-Type: application/json' \
--data '{
    "name":"John",
    "age":99,
    "course":"Python"
}'


# Delete Student by ID
curl -X DELETE 'http://localhost:8000/v1/students/69f11c84b9ac80396d2807a5' \
--header 'Content-Type: application/json'

```

## Deploy
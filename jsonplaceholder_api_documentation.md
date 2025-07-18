# SAMPLE API DOCUMENTATION-JSON PLACEHOLDER (POSTS API)


## GET A POST USING JSON PLACEHOLDER API IN POSTMAN

### API - JSON Placeholder
### HTTP Method:
GET
### Overview:
This REST API is used mainly for learning purpose. It helps people in practicing API requests. GET request retrieves all data. 
### Base URL:
`https://jsonplaceholder.typicode.com`
### End Point:
/posts
### Full Request:
`https://jsonplaceholder.typicode.com/posts`
### Description:
- Get request retrieves data from the server. Here this API retrieves a list  of posts.
- This JSON placeholder  REST API is used mainly for learning purpose. 
- This returns a list of fake posts.
### Request:
**GET** https://jsonplaceholder.typicode.com/posts
### Response:
We get response in JSON format. 
  ```
  {
    "userId": 1,
    "id": 1,
    "title": "Sample title",
    "body": "Sample body"
  }
  ```

### Status Code and Message:
200 OK

## CREATE A NEW POST USING JSON PLACEHOLDER API IN POSTMAN

### API - JSON Placeholder
### HTTP Method:
POST
### Overview:
This REST API is used mainly for learning purpose. It helps people in practicing API requests. POST request is used for craeting a new resource.
### Base URL:
`https://jsonplaceholder.typicode.com`
### End Point:
posts/1
### Full Request:
`https://jsonplaceholder.typicode.com/posts/1`
### Body(JSON):
```
{
    "title": "New Post",
    "body": "Updated Content",
    "userId":1,
    "id" : 101
}
```

### Description:
- POST request is used for creating new resources. In this case it’s new post.
- The request requires a JSON body.
- Select Body as raw and file as JSON from dropdown. 
### Request:
**POST** https://jsonplaceholder.typicode.com/posts

### Response:
We get response in JSON format.
```
{
    "title": "New Post",
    "body": "Content",
    "userID": 1,
    "id": 101
}
```
### Status code and Message:
201 Created


## UPDATE A POST USING JSON PLACEHOLDER API IN POSTMAN

### API - JSON Placeholder
### HTTP Method:
### PUT
### Overview:
This REST API is used mainly for learning purposes. It helps people in practicing API requests. PUT request is used to update the existing resource.
### Base URL:
`https://jsonplaceholder.typicode.com`
### End Point:
posts/1
### Full Request:
`https://jsonplaceholder.typicode.com/posts/1`
### Body(JSON):
```
{
    "title": "New Post",
    "body": "Updated Content",
    "userId":1,
    "id" : 101
}
```
### Description:
- PUT request is used for updating existing resources. In this case it’s existing post with ID 1.
- 	Making changes to the already existing one and updating it
- The request requires a JSON body.
- Give the ID of the resource you want to update
- Select, Body as raw and file as JSON from the dropdown. 
### Request:
**PUT** https://jsonplaceholder.typicode.com/posts/1
### Response:
```
{
    "title": "New Post",
    "body": "Updated Content",
    "userId": 1,
    "id": 1
}
```
#### Status code and message:
200 OK

## DELETE A POST USING JSON PLACEHOLDER API IN POSTMAN

### API - JSON Placeholder
### HTTP Method:
DELETE
### Overview:
This REST API is used mainly for learning purposes. It helps people in practicing API requests. Delete request is used to remove the existing resource.
### Base URL:
`https://jsonplaceholder.typicode.com`
### End Point:
posts/1
### Full Request:
`https://jsonplaceholder.typicode.com/posts/1`
### Description:
- DELETE request is used for deleting existing resources. In this case it’s existing post with ID 1.
- Give the ID of the resource you want to delete
- No request body is required
### Request:
DELETE https://jsonplaceholder.typicode.com/posts/1
### Response:
```json
{}
### Status code and message:
200 OK or 204 No Content









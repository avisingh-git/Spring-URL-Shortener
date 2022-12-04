### Prerequisites
* Redis running locally
  * host: localhost
  * port: 6379

### Execution

```
java -jar spring-url-shortner.jar
```

### API Details

#### Create Short URL:
`http://localhost:8085/rest/url`

Request body:
```JSON
{
    "url": "https://www.gmail.com"
}
```
Response body:
```JSON
{
    "id": "94717296",
    "url": "https://www.gmail.com",
    "created": "2018-12-02T14:11:26.887"
}

#### Retrieve Original URL:
`http://localhost:8085/rest/url/{id}`

Response body:
```JSON
{
    "id": "94717296",
    "url": "https://www.gmail.com",
    "created": "2018-12-02T14:11:26.887"
}

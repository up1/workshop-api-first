# Workshop with Swagger


## Working with [Swagger-Codegen](https://github.com/swagger-api/swagger-codegen)
* Generate API document (HTML)
* Generate Mock/Stub API
* Generate code
  * Server-side
  * Client-side

Install
```
$brew install swagger-codegen
```

Generate API Document
```
$swagger-codegen generate -i api.yml -o html -l html
$swagger-codegen generate -i api.yml -o html -l dynamic-html
```

Better :: Generate Mock/Stub server + API Document
* NodeJS
```
$swagger-codegen generate -i api.yml -o nodejs -l nodejs-server
$cd nodejs
$npm start
```

* Access to API with `http://localhost:8080`
* Access to API Document with `http://localhost:8080/docs`


## Generate HTML with Redocly
```
$npm i -g @redocly/cli 
$redocly lint api.yml
```

## Mock server with OpenAPI Mocker
```
$npm i -g open-api-mocker
$open-api-mocker -s api.yml -w
```

Access to api from `http://localhost:5000`

